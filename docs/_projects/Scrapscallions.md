---
layout: project
title: Scrapscallions
description: A capstone project I developed as part of a talented team.
image: /Portfolio/assets/images/scrapscallions.png
gitlink: https://github.com/JeffcoatDesign/Scrapscallions
---

## Overview
Scrapscallions is a singleplayer game where players build and battle robots in an arena. It features a robust Goal-Oriented Action Planning implementation, a modular robot system, and a responsive UI to tie it all together. I developed it as part of a team of 3 over the span of six months. It was created in Unity and its assets were made using tools such as Maya, Substance Painter Photoshop.

The premise for the game was that players would play as a young scavenger looking to move up in the world. Due to the wasteful habits of the privileged upper city, there is a surplus of parts available to scavengers in the lower city, so long as they are willing to chance the mad robots protecting the trash heap. With these scavenged robots, scavengers can battle in the arena to gain fame and fortune.

In order to create this project, we tailored SCRUM to our needs and assigned roles based on each person's strengths. My role was centered around AI and system design, while the other two took on UI/UX and Art, respectively. While these were out focuses, we provided support to each other area as needed. I found myself debugging issues with UI/system integration and helping with technical art.

There were a few design decisions that we found were critical for this game. We chose to make the robots control themselves in order to offer the feeling that robots are separate entities from the player. The AI had to be capable of adapting to modular parts and had to have modifiable behavior. To fit these requirements, I researched game AI systems until I found one that would work. Ultimately the best choice for this was Goal-Oriented Action Planning (GOAP) with the implementation of steering behaviors. The GOAP system would perform the decision making, while the steering behaviors and part actions acted as different strategies that it could trigger. This system was costly to develop in terms of time, but was reactive, scalable, and highly customizable.