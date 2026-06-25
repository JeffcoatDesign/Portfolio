---
layout: project
title: Cast Forward
description: A interactive that boasts a dynamic procedural generation system and graph traversal.
image: /Portfolio/assets/images/CastForward.png
gitlink: https://github.com/JeffcoatDesign/Cast-Forward
playlink: https://jeffcoatdesign.github.io/Cast-Forward/
tags: [ Graphs, Procedural Generation, Unity ]
yturl: https://www.youtube.com/embed/CsDfHLd2knE?si=CZYogXk__hi3H4Gs
order: 2
---

## Overview
Cast Forward is a project that I created with the intention of learning more about creating digital environments. Over the course of three and a half months, I developed the application on my own following Agile practices with careful iteration. As I worked on it, I received regular feedback and user stories that influenced the design of each of its 8 releases. It boasts procedural generation powered by multiple algorithms and shape grammars. The user's experience was heavily dependent on a carefully-crafted state machine. I created most of the assets using software such as: Unity, Maya, Photoshop, Illustrator, and Substance Painter. I also used a few third-party assets to expedite the process.

### Procedural Level Generation w/ A*
Development for Cast Forward started with a hexagonal, grid-based level generation system. I chose to use hexagons knowing that they would pack together nicely while allowing more degrees of movement between cells. The level generator starts by generating a grid and selecting different points to connect. Those points are fed into a Delaunay triangulation algorithm implementation, where it finds the minimum spanning tree of those points. With that tree, the generator uses A* to generate paths between the selected points. Finally every point within the network is assigned a room tile. The furthest two points being the start and end of the level.

The process is:
1. Create a hexagonal grid.
2. Add noise to disincentivize A* from going through certain hexes and add randomness.
3. Select points at random.
4. Triangulate the selected points.
5. Find the minimum spanning tree.
6. Run A* using point pares the minimum spanning tree and the noise map in order to create the paths.
7. Place the correct tiles based on the shape grammar, influenced by neighboring cells.

### Iteration
As I introduced features, it was essential that they saw the polish necessary for my target user experience. To achieve this expereience, I performed user tests where I recorded user stories and checked them against the target experience. This led to steady improvement that would have been difficult to achieve on my own.