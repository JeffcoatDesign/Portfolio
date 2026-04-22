---
layout: project
title: Cast Forward
description: A fast-paced, spell-slinging gane that features procedural level generation.
image: /Portfolio/assets/images/CastForward.png
gitlink: https://github.com/JeffcoatDesign/Cast-Forward
tags: [ Graphs, Procedural Generation, Unity ]
yturl: https://www.youtube.com/watch?v=CsDfHLd2knE
---

## Overview
Cast Forward is a wizard game where the player has to escape through a portal. Over the course of three and a half months, I developed the game on my own following Agile practices such as Kanban. As I worked on it, I received regular feedback and user stories that influenced the design. It boasts procedural generation powered by multiple algorithms and shape grammars. I designed the gameplay to emphasize movement, so that players can quickly make their escape and explore the level. I created most of the assets using software such as: Unity, Maya, Photoshop, Illustrator, and Substance Painter. I also used a few third-party assets to expedite the process.

### Procedural Level Generation w/ A*
Development for this game started with a hexagonal, grid-based level generation system. I chose to use hexagons knowing that they would enable the player to move more freely than with squares. The level generator starts by generating a grid and selecting different points to connect. Those points are fed into a triangulation algorithm, where it finds the minimum spanning tree of those points. With that tree, the generator uses A* to generate paths between the selected points. Finally every point within the network is assigned a room tile. The furthest two points being the start and end of the level.

The process is:
1. Create the hexagonal grid.
2. Add noise to disincentivize A* from going through certain hexes.
3. Select random points to use to generate the paths.
4. Triangulate points and find the minimum spanning tree.
5. Run A* using the minimum spanning tree and noise map in order to crate the paths.
6. Place the correct prefabs based on which neighbors are paths.

### Movement
It was essential for me to get movement right for this game I began by creating test scene where I could build a first-person player controller following Shigeru Miyamoto's "miniature garden" design philosophy. As I created the player's state machine, I regularly tested each interaction the player might have.