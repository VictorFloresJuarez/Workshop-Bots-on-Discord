# Step 4: Activate bot

Create a new project in Replit, in the language select Python and give it a name. 

![captura9](https://github.com/VictorFloresJuarez/Workshop-Bots-on-Discord/blob/main/Resources/captura9.png?raw=true)
----------------------------------------------------------------------------------
Now in Discord Developer Portal, in the 'Bot' section copy the Token.

![captura10](https://github.com/VictorFloresJuarez/Workshop-Bots-on-Discord/blob/main/Resources/captura10.png?raw=true)
----------------------------------------------------------------------------------
Now, in the Replit project you just created go to the 'Secrets' section, in key enter 'TOKEN' and in value paste what you just copied. Then click on 'Add new secret'.

![captura12](https://github.com/VictorFloresJuarez/Workshop-Bots-on-Discord/blob/main/Resources/captura12.png?raw=true)
----------------------------------------------------------------------------------

Now we will work in the main.py file, we will add several things, please follow this order:
- Perform the discord import with this statement: import discord
- Perform the import to use secrets: import os
- Assign to a variable the value you saved with the key 'TOKEN': my_secret = os.environ['TOKEN']
- Add the following statement: client = discord.Client()

If you did everything correctly your main.py file should look like this:

![captura13](https://github.com/VictorFloresJuarez/Workshop-Bots-on-Discord/blob/main/Resources/captura13.png?raw=true)

Here is the code for you to copy and paste if you wish:

    import discord
    import os
    my_secret = os.environ['TOKEN']
    client = discord.Client()

Now please copy and paste this code (paste it at the end of the main file):

    @client.event
    async def on_ready():
        print('Se ha iniciado el {0.user}'.format(client))

Your main file should look like this:

![captura14](https://github.com/VictorFloresJuarez/Workshop-Bots-on-Discord/blob/main/Resources/captura14.png?raw=true)

Now paste this statement at the end of your code: 

    client.run(my_secret)

With this click on Run, for being the first time it will take a little time to run, but you will notice how, once it runs, your bot is now online.


![captura15](https://github.com/VictorFloresJuarez/Workshop-Bots-on-Discord/blob/main/Resources/captura15.png?raw=true)

![captura16](https://github.com/VictorFloresJuarez/Workshop-Bots-on-Discord/blob/main/Resources/captura16.png?raw=true)
