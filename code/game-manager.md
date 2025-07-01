---
title: Game Manager
layout: home
nav_order: 2
parent: Code
---

# Game States

What kind of structure the game follows:
* One level vs multiple stages
* Linear vs hub-based progression
* High score vs level-based goals

Explain game states:
* Main Menu
* Playing
* Paused
* Game Over
* Victory

Tips:
* Use a state machine or enum to manage flow in code
* In Godot: consider a GameManager autoload that tracks the current state
* Keep it readable and transition clearly between states