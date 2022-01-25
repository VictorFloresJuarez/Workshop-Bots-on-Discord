# Audio functions

To begin, we will follow the first 3 steps of the main project.
If you need help remembering those 3 steps, you can go back to the index of steps right [here](https://github.com/VictorFloresJuarez/Workshop-Bots-on-Discord/blob/main/Sections/Creation%20process/Index%20of%20steps.md)

## Step 4: Create your files: main.py and music.py on Replit
The first thing we're gonna is create our main.py and then import discord.py so we can work with discord commands.

![importdiscord](https://github.com/VictorFloresJuarez/Workshop-Bots-on-Discord/blob/main/Resources/paso4.%20importDiscord.png?raw=true)

 Then we're going to initialize our bot using commands and using our token. At this point, you should already know how to get your token but if you don't remember, you can check [here](https://github.com/VictorFloresJuarez/Workshop-Bots-on-Discord/blob/main/Sections/Creation%20process/%3EStep2+++/Step4.md). Your code should look like this:
 
![token](https://github.com/VictorFloresJuarez/Workshop-Bots-on-Discord/blob/main/Resources/paso4.token.png?raw=true)
 
 After this, we need to create a new file and we're going to call it music.py. On this file, we need to import discord.py again and also import youtube.dl, basically so we can work with youtube videos and music. If you want to read more about youtube.dl, you can search more information [here](https://en.wikipedia.org/wiki/Youtube-dl). Finally, your music.py file should look like this:
 
![music](https://github.com/VictorFloresJuarez/Workshop-Bots-on-Discord/blob/main/Resources/paso4.music.png?raw=true)

## Step 5: Start the coding
First, we need to create a class cog music and then, add the setup function as a cog.
// A cog is a file generation tool. It lets you use pieces of Python code as generators in your source files to generate whatever text you need!

![inicializar](https://github.com/VictorFloresJuarez/Workshop-Bots-on-Discord/blob/main/Resources/paso5.inicializar.png?raw=true)

Then we need to go back to the main.py and import music as a cog and create a list called music and include all the cogs we have.
// and setup the cogs (delete)

![cogs](https://github.com/VictorFloresJuarez/Workshop-Bots-on-Discord/blob/main/Resources/paso5.cogs.png?raw=true)

## Step 6: Bot Commands
Back in the class music, we need to add a JOIN COMMAND so the bot can join the voice channel, then we also need a DISCONNECT COMMAND so the bot can leave the voice channel. For both of this things, you'll need to write the following codding:

![joindisconnect](https://github.com/VictorFloresJuarez/Workshop-Bots-on-Discord/blob/main/Resources/paso6joindisconnect.png?raw=true)

Past that, we will add the PLAY COMMAND to play any song on youtube you want with a link. Something you need to know for the following coding:

FFMPEG_OPTIONS handles the streaming in discord.

YDL_OPTIONS makes the bot play each song in the best audio format posible.

The "with youtube_dl.YoutubeDL(YDL_OPTIONS) as ydl:" block works to create a String to play the audio.

![play](https://github.com/VictorFloresJuarez/Workshop-Bots-on-Discord/blob/main/Resources/paso6play.png?raw=true)

Finally, we just need to add the PAUSE & RESUME commands, you should already know why are they useful. This last 2 commands are very simple so you can easily work them on your own. It should look like this:

![pauseresume](https://github.com/VictorFloresJuarez/Workshop-Bots-on-Discord/blob/main/Resources/paso6.pauseresume.png?raw=true)

## Step 7: Fixing mistakes


