---
published: false
title: The Virtual Machine
layout: post
---
The game is essentially based on cars physic and road [procedurally generated](https://en.wikipedia.org/wiki/Procedural_generation).

The Virtual Machine works in harmony with the genetic algorithm, it is simply a big testbed.

- seed/reseed the world - *generate seeded procedural roads*
- spawn cars - *spawn an unlimited number of cars at the road start*
- execute one step - *update the world, ask cars's new acceleration/wheels rotation*

Cars are made of multiple parts:

- a rigid body - *all wheels will be fixed to this, can have different weights*
- some wheels - *with parameters like friction, clamped rotation...*
- road detection rays - *the eyes of the car, return the distance to road edges*

The road is infinite, each time a car needs a new stretch of road, the VM is capable of generating it. Road difficulty: curvature and width are adjustable and all parameters are based on a unique seed.

Each time a car needs instructions (wheels rotation, acceleration...), the genetic algorithm answer
The Virtual Machine can spawn an unlimited number of cars and evaluate them.