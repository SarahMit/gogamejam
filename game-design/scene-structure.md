---
title: Scene Structure
layout: home
nav_order: 3
parent: Game Design
---

# Scene and Menu Structure
What happens from the moment the game loads to when the player wins, dies, or quits? This section is about designing how scenes connect and how the game feels to navigate.

## Core scenes a typical jam game should have
* Title screen
* (Instructions or "How to Play")
* Main game
* Game over / win screen
* Credits or restart option

## Game Flow
```mermaid
graph TD;
    accTitle: the diamond pattern
    accDescr: a graph with four nodes: A points to B and C, while B and C both point to D
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```