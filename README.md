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

You're free to look into the code and modify the shape of the message the bot is looking for, but by default, havarti will notice when an emit ends with 'has arrived!'.

3) Set up a webhook in your discord server