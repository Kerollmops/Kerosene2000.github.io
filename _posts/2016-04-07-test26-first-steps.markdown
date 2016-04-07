---
published: true
title: Welcome to the Test26 devlog
layout: post
---
Genetic algorithms and neural networks, that's what leads us to be interested on the production of a race game.
But not a classic race game, it's is controlled by artificial intelligences.
But not classic AI, genetically trained AI with neural networks inside !

There is three parts in this project:

1. The Virtual Machine - *run all the physics steps for each cars at cpu speed !*
2. The Graphic - *display the buffered race at normal speed for a best debug comfort.*
3. The Genetic Algorithm - *answer the VM when asking movement for each car.*

Each cars have multiple rays to detect walls, this is the VM which returns hit distances for each ray at each tick of [nphysics](https://github.com/sebcrozet/nphysics).

### **Neuroevolution - Car learns to drive**
[![Neuroevolution - Car learns to drive](http://img.youtube.com/vi/5lJuEW-5vr8/0.jpg)](https://youtu.be/5lJuEW-5vr8? "Neuroevolution - Car learns to drive")