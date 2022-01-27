# Embed

An extra to give a better look to your bot messages is the use of Embed. This can be understood as aesthetically better messages. Its implementation is done in the following way:

Suppose you want to make a bot that responds to the '!reply' command, and you want the bot's response to look better. 

First, we assume that you already have a working bot, for this example we start with the following code: 

![capture23](https://github.com/VictorFloresJuarez/Workshop-Bots-on-Discord/blob/main/Resources/captura23.png?raw=true)

As you can see, the message that the bot will reply with is: 'I replied you', let's change this a bit.

First we need to assign to a variable the message we want to send. Use the following code example:

    mensaje = 'I replied you'

Now, you are going to create the Embed using the following statement:

    embed = discord.Embed(title= message)


Then place this statement:

    message= await message.channel.send(embed=embed)

Remember to replace the variables 'mensaje' and 'embed' if you renamed them.

Your code should now look like this:

![capture25](https://github.com/VictorFloresJuarez/Workshop-Bots-on-Discord/blob/main/Resources/captura25.png?raw=true)

And that's it, test your bot using the command to see the difference. 
