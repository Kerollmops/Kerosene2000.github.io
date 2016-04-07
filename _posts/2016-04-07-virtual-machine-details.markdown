---
published: false
title: Virtual Machine details
layout: post
---
The game is essentially based on car physics and road procedural generation.

Cars are made of multiple parts:

- a rigid body - *all wheels will be fixed to this*
- some wheels - *friction, ...*
- hit detection rays - *the eyes of the car, return the distance to walls*

Each car have multiple rays to detect walls, this is the VM which returns hit distances for each ray at each tick of [nphysics (the 2d physic engine)](https://github.com/sebcrozet/nphysics).
The GFX, if connected, receive cars informations (positions, rotations, wheels rotations, speed, acceleration...)