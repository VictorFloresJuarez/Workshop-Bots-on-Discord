# Step 6: Our first command

Please copy and paste the following code into your main.py file, it must be before the last two statements:

    @client.event
    async def on_message(message):
      if message.author == client.user:
        return

    if message.content.startswith('AMOGUS'):
      await message.channel.send('SUS')
  

## [Previous step](https://github.com/VictorFloresJuarez/Workshop-Bots-on-Discord/blob/main/Sections/Creation%20process/%3EStep2%2B%2B%2B/Step4.md)
