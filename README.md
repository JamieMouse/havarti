# havarti

This is a Furcadia bot based on the skeleton provided by FurgieV in kiwi-bot https://github.com/FergieV/kiwi-bot. Most of this code is still the original Kiwi-bot, all credit for it goes to FurgieV, thank you!.

## Features

* Integrate with discord and alert when a new arrival enters your dream

## Getting Started

1) Create a character to be the actor for your bot, bots are just like any other character on your account.
2) Add DS to your dream to emit a message whenever a furre joins

Something like:
    (0:9) When a furre arrives in the dream,     
    (5:204) emitloud message {[FURRE] has arrived!} to everyone on the map. 

You're free to look into the code and modify the shape of the message the bot is looking for, but by default, havarti will notice when an emit ends with '**has arrived!**'.

3) Set up a webhook in your discord server

Go into your Discord server settings, and select the integrations tab. Then click 'Create Webhook'
![image](https://github.com/JamieMouse/havarti/assets/155923040/3d641630-2166-411e-acc5-2c8f859bc6de)

This will create one with a randomized name. Open it, give it a fun name and copy the url. (Note, this url is a secret, you shouldn't share it with anyone)

![image](https://github.com/JamieMouse/havarti/assets/155923040/8a0bade5-b48d-42fa-b3ce-1ac3f18640fd)

I like to make a specific channel in my discord server for bots to post their messages. This way people can easily mute them if they don't want to see the notifications.

4) Download the Havarti bot package

https://github.com/JamieMouse/havarti/tree/main

If you're not comfortable with git, you can use the download zip button! Just remember to extract the files.
![image](https://github.com/JamieMouse/havarti/assets/155923040/0bb7e2fa-f463-4e9e-99ce-af80a639e7f6)

5) Configure the bot

Now you have everything you need to configure your bot! In the files you downloaded earlier, you should find one labelled bot.conf. This is where you'll configure all the information related to your bot!

Use the email associated with the character you made earlier, as well as the password. Fill in the character name, if it has a space in it, use a | instead. Like... 'Havarti|Dreams' instead of 'Havarti Dreams'. Colors and desc are asthetic only, but fill them in if you like! The owner allows you to assign a character as the bot owner, who can issue it commands.

Very importantly, the webhookurl is the url you copied earlier while creating your webhook. The bot won't know where to send the notifications if you don't fill this in.

## Running the bot

In the directory you extracted havarti into, open command prompt or terminal
Start the bot with the command **py kiwibot.py**

Your bot should log in to wherever you last logged out of it, now when the text {'furre name} has arrived!' appears in the dream your bot is in, it'll call the discord webhook and forward the notification to discord!

![image](https://github.com/JamieMouse/havarti/assets/155923040/da99faf9-3413-410d-a4c9-1ec3211db916)


## Troubleshooting

### ModuleNotFoundError: No module named 'requests'

You'll need to install the requests module, use the command **pip3 install requests**

