# Step 5: Keep our bot active and monitor it.



Now we are going to keep our bot active 24/7. 

First create a new file, the name of it doesn't matter, just make sure it's a .py file. 

![captura17](https://github.com/VictorFloresJuarez/Workshop-Bots-on-Discord/blob/main/Resources/captura17.png?raw=true)

Now copy and paste this code into the new file you created:

    from flask import Flask
    from threading import Thread

    app = Flask('')

    @app.route('/')
    def home():
      return "Hello, I am alive!"

    def run():
      app.run(host='0.0.0.0', port=8080)

    def keep_alive():
      t = Thread(target=run)
      t.start()

Now in your main.py file perform the following import:

    from 'filename' import keep_alive. 

Where is 'filename' enter the name you gave to your new file.

Now enter the following code in the penultimate line of code: 

    keep_alive()

Your main.py file should look like this:

![captura18](https://github.com/VictorFloresJuarez/Workshop-Bots-on-Discord/blob/main/Resources/captura18.png?raw=true)

Stop the bot execution and run it again, from now on the bot should not shut down, try closing the repl of your bot.

Now, to monitor if your bot is active [click here](https://github.com/VictorFloresJuarez/Workshop-Bots-on-Discord/blob/main/Sections/Creation%20process/%3EStep2%2B%2B%2B/Monitoring.md) (this is optional, does not affect the behavior of your bot)


## [Next step](https://github.com/VictorFloresJuarez/Workshop-Bots-on-Discord/blob/main/Sections/Creation%20process/%3EStep2%2B%2B%2B/Step6.md)
## [Previous step](https://github.com/VictorFloresJuarez/Workshop-Bots-on-Discord/blob/main/Sections/Creation%20process/%3EStep2%2B%2B%2B/Step4.md)
