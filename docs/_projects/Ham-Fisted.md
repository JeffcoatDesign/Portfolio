---
layout: project
title: Ham-Fisted
description: An application that supports realtime interaction built by a team of 2 developers.
image: /Portfolio/assets/images/hf key art.png
gitlink: https://github.com/JeffcoatDesign/Ham-Fisted-2.0
tags: [ Realtime Interaction, Netcode, Unity ]
order: 4
---

## Overview
Ham-Fisted is an online application where users interact with each other in realtime. It has seen 3 large iterations which are the basic prototype, a split-screen demo for the 2023 Game Developer's conference, and the WIP final commercial version. With the completion of the demo, I have been the sole developer for the project and have been making large technical contributions ever since.

### Concepts
The latest iteration includes
- Server authority
- Client prediction
- Steamworks API integration
- Data synchronization

![Improved Hit Animations](/Portfolio/assets/images/better hit.gif)

### Multi-User Support
Many multiplayer games find it satisfactory to either support online multiplayer or splitscreen multiplayer and not both due to the technical burden of integrating the two. For Ham-Fisted, that was not the case, as I have carefully worked to integrate both systems to allow more users to play alongside eachother on fewer machines. The simplictiy of the environments saves on processing power so that it can be applied to splitscreen. There was some complexity introduced by this decision that took some time to resolve. Rather than a single player object per client, I had to create a client object that synchronized multiple player objects across clients.

### Steam API
Valve offers its partners access to the Steamworks API when they pay to list an application on Steam. In Ham-Fisted, I used full advantage of this because I needed a free way to connect remote clients without any recurring charges. There are also a variety of features within the API that improve the quality of life for users, such as the ability to create lobbies, invite friends to game sessions through the Steam overlay, and Steam avatars.

### Tools
I have done everything from programming to art and design. The tools that I have used include:
- Unity 3D
- Visual Studio
- Git and GitHub
- Headus UV Layout
- Autodesk Maya
- Adobe Photoshop
- Adobe Illustrator
- Adobe Substance Painter