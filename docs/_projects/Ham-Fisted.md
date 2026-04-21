---
layout: project
title: Ham-Fisted
description: A multiplayer game designed with careful iteration.
image: /Portfolio/assets/images/ham-fisted.png
gitlink: https://github.com/JeffcoatDesign/Ham-Fisted-2.0
tags: [ Mulitplayer, Steam, Unity ]
---

## Overview
Ham-Fisted is an online multiplayer game where hamsters battle it out to see who comes out on top, inspired by the likes of Sega's Super Monkey Ball and Nintendo's Super Smash Bros. It features Steam integration, combined split-screen and online multiplayer, and robust controller integration. The Unity game was created in collaboration with one other as part of a school project, which it has since outgrown. I have been the main developer since the original project wrapped up, using it to develop my production skills.

During Ham-Fisted's development, I used numerous tools to perform every function necessary to create a game. The 3D modeling and animation was all created in Autodesk Maya, with the UV-unwrapping for the hamsters performed inside of Headus UVLayout. The UI and many of the object textures were created in Adobe Photoshop and Illustrator. The remaining textures were painted in Substance painter. The code was developed in Visual Studio with Copilot disabled, so I could focus on expanding my knowledge of C# and Unity. For version control, I used GitHub, Git, and GitHub desktop.

For a commercial version of the game, I wanted to have a scalable, low-cost way to connect players for online multiplayer. I found that by integrating Steamworks, I could use Valve's servers to connect players peer-to-peer. This was perfect, as the only financial cost was the one-time purchase of a Steam page. It did restrict my game from other marketplaces, however I had already planned on only releasing on Steam. Steamworks offered many advantages to the project that I believe any modern PC game must implement for a superior user experience.

As I developed the game, I encountered numerous programming challenges and overcame them to build each and every feature. One of my most difficult hurdles was integrating split-screen with online multiplayer. Each player needed to be created at the start of each round, and their properties needed to be synchronized. My solution was a data-oriented approach, where a data object is created for each player that joins and is later used to create a playable hamster at the start of the game. Another issue had to do with the hamsters themselves. Originally, the hamsters were static and lifeless, which made it difficult for players to connect with them. To fix this I created an animation rig for them and animated them idling, walking, running, sitting discombobulated, and celebrating. Still this wasn't enough, they still felt disconnected from the action, so I created an adaptive animation blending system allow them to react to being hit. This had a tremendous result, making the hamsters feel like an actual part of the world.

Currently my GitHub displays two public versions of the game, while I keep the commercial version private. These two versions are programmed at a lesser skill level than what I can do today. However, they display my growth as a developer and can give some idea as to where the latest version stands today. I can also say that I have learned many concepts such as the SOLID principles and iterative design.