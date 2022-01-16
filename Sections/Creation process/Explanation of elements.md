# In-depth explanation of elements

## In step 1, why create a new application?

By doing this you can understand it in the following way: the Discord database creates a new profile, which does not yet have a purpose however it already occupies a memory space in the database.

## In step 2, add Bot.... Why?

When doing this we are dictating the behavior that will have the application that we have just created, now Discord already knows that this application has the behavior of a bot.

## In step 3, permissions

To have a better idea of the available permissions please [click here](https://github.com/VictorFloresJuarez/Workshop-Bots-on-Discord/blob/main/Sections/Creation%20process/%3EStep2%2B%2B%2B/permissions.md)

## In step 4, the code.

All the code that is entered in that part is what activates our bot and allows us to make it work. With the exception of this code:

    @client.event
    async def on_ready():
        print('Se ha iniciado el {0.user}'.format(client))

This last line of code is where the magic happens:

    client.run(my_secret)

This is what makes the command to execute the bot.

## In step 5, keep active

All the code we add there makes our bot stay active 24 hours a day, as such in your main code the following statement is the one that does that:

    keep_alive()

## In step 6, events

The simplest way to explain events is that they represent a possible action, and basically when a client receives an event from Discord, it finds out what event it is and generates, or locates, the objects that were sent by the event. The client then sends the objects to the method that handles those events, but first you need to tell the client what those methods are. This is where event decorators come in. 

When you use the  

    @client.event

on your  

    on_message

what you are actually doing is saying 

    on_message = client.event(on_message)

You can find all the information related with discord.py if you [click here](https://discordpy.readthedocs.io/en/stable/)
