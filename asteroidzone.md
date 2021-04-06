---
layout: default
title: Asteroid Zone (WIP)
description: University of Bristol Year 3 - Team Games Project
is_project_page: true
is_public: false
giturl: https://github.com/Asteroid-Zone
---

Asteroid Zone is an online coop multiplayer game made using [Unity](https://unity.com/) and hosted on a site made using Razor Pages.  
It is controlled using only speech recognition voice commands.  

It can be played [**here**](https://asteroid-zone.herokuapp.com/).
Final release expected 18/05/2021.

## My Role
I am the Lead Programmer on this project so I am responsible for merging feature branches.  
I implemented the command recognition system which interprets what you said and performs the commands.  
If a command is not valid, I created a system which predicts what the most similar/most likely command would be.  
This helps make the game run smoother as you don't have to repeat commands as often if the [Web Speech API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Speech_API) doesn't recognise your voice properly.  
I also implemented a lot of the gameplay logic and some of the multiplayer synchronisation using [Photon Network](https://www.photonengine.com/pun).
I modelled and animated the space station using Autodesk Maya.

## Game Description
Players connect to the website (currently [https://asteroid-zone.herokuapp.com/Play](https://asteroid-zone.herokuapp.com/Play)). They enter their names and click "Start Game". After connecting, they take control of ships using only voice commands. They can turn, move forward and backward, move to a grid coordinate or move to an object such as the space station. If they are moving to a location (station or grid) the AI will automatically avoid obstacles in the path. One player is the commander and the others are miners. The commander is in charge of allocating resources to repair parts of the station and has a more complete overview of the game so they need to communicate with the other players to give them information.

The objective is to repair the hyperdrive on the space station and use it to escape the area, which can be done by activating the mining laser and mining asteroids. Then they can navigate to the station, and transfer the resources. The Station Commander can then use the resources to repair different station modules which enable different abilities once fully repaired (shield generator, engines, hyperdrive, etc.)

However, there are space pirates that will attack players and search for the space station to destroy it, at the moment everyone can see the whole map, but in future versions the station commander will need to communicate with the other players to warn them. Miners can shoot the pirates to defend themselves and the station. There is a lock-on system so they can track a nearby pirate or asteroid.

![Gameplay Screenshot](https://i.imgur.com/fesfAvB.png)
