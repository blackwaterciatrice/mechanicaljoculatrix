# mechanicaljoculatrix
This is the code for a discord bot that runs in a cloud server, using occasional pings from a third-party service to keep the server active; while active, the bot will make a few off-color comments and, when asked to tell you a joke, will either tell you a joke (pulled from an API) or quote you the current price of bitcoin in USD (pulled from an API). 
It's based off the bot here: https://www.freecodecamp.org/news/create-a-discord-bot-with-python/
The bot runs in the Replit environment, and hosts its own mini server which sends a little "hello world!" when connected. Replit usually shuts down programs when you close the tab, and shuts down development servers after an hour of inactivity. I set up an account at uptimerobot.com, which lets you monitor 50 different websites for free, and their service pings the bot's mini server every 40 minutes or so, causing it to reply, keeping it from becoming inactive.
I'm pretty sure that has some minor net negative carbon footprints, so uh, I hope this doesn't become viral; it was supposed to be just a fun project. Took me about 3 hours. 
You can pretty easily plug in whatever APIs or custom responses you want! Just do what I did and google whatever error message it spits out. If it works perfectly first time, great! 


If you want to actually set this up, you'll have to actually go over to Discord's Dev Console, log in using your discord account create a new application, convert that into a bot. If you want the bot to do stuff you have to give it permissions.
I uh, I didn't realize it could just give you an OAuth2 link on command, so I "built" mine by plugging in the client ID and permissions code to the example they gave. But you can just click "URL generator" and it will. generate you. a URL. doy. Feel a little stupid about that one uhh anyway
Click that URL and Discord will do the rest; that plugs your bot into the server, you should see it come online, Discord will announce it like a user. 
Then you'll want to go to the Bot tab on Discord's dev page, get the token, save that as an .env or a Secret or otherwise plug it into your program as "TOKEN", otherwise you won't be able to connect the stuff here that makes the bot go, to the stuff that makes the bot's Discord "account" work. But once you get that plugged in you should be all set. 

Stuff I learned doing this: 
Everything? I mean, I had done some Python work before, I know something about servers and networking, I'd used Spotify's API a few times, but I am now working with multiple different APIs. Really see the value of having shared libraries, too; this project pulls from 5 different python libraries, which VASTLY reduces the difficulty. Imagine if I had to code my own random number function just to pick either 0 or 1 each time you asked the bot to tell you a joke. 

This is my first github upload! Thanks for reading, whowever you are! Cheers! 
