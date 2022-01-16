# Step 5: Keep our bot active.


## [Next step](https://github.com/VictorFloresJuarez/Workshop-Bots-on-Discord/tree/main/Sections/Creation%20process/%3EStep2+++)
## [Previous step](https://github.com/VictorFloresJuarez/Workshop-Bots-on-Discord/blob/main/Sections/Creation%20process/%3EStep2%2B%2B%2B/Step4.md)

Now we are going to keep our bot active 24/7. 

First create a new file, the name of it doesn't matter, just make sure it's a .py file. 

![captura17](?raw=true)

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
