---
layout: default
title: Rogue Robots
modal-id: 2
date: 2022-02-02
imgThumbnail: RogueRobots/Thumbnail.jpg
img:
    - active: true
      link: "RogueRobots/image2.png"
    - link: "RogueRobots/image.png"
    - video: "RogueRobots/Rogue-Robots.mp4"
alt: image-alt
project-date: Q3-Q4 2022
category: Course project - Large Game Project
areas: Procedural Generation - Gameplay Programming - Blender Modelling
description: 
    - During the first term of my 5th year studying at BTH we were 10 people collaborating on a Large Game Project for 16 weeks. During the course of the project we used the Scrum methodology. For the project we had to develop everything from scratch, meaning no pre-made game engine was used.
    - The game we developed is called Rogue Robots, which is a Multiplayer Arcade First Person Shooter, where the player and their friends have to cooperate as mining corporation overseers to escape a cave system overrun by corrupt mining robots that the players were overseeing for the corporation. During the game players can find buffs, items, and weapon components that give the player's weapon unique effects to help fight off the hordes of enemies.
    - The engine was made in C++, using DirectX12 to create the rendering pipeline. The shaders (GPU code) were written in HLSL. We also used Lua for gameplay programming.
    - My responsibility and largest contribution to the project was the procedural generation of the levels used in the game. These levels are generated using the Wave Function Collapse algorithm and is used on the fly to generate levels during runtime. The generator uses CPU threads to quicker generate the level by generating all rooms at the same time, and then combining them into the final level.
    - I also took on the responsibility of making sure all our assets were properly made and looked good to be used in the game. I learned Blender where I adjusted the models that we outsourced for our specific needs. I created the terrain used in the procedural generation from scratch and, with help from a teacher at the University, created procedurally generated textures for the terrain.
    - I also implemented gameplay systems and features such as the weapon's component system, and I implemented the functionality of some of the items in the game.
languages: C++ - HLSL - Lua
github: https://github.com/DisorganizedGames/Rogue-Robots
---
