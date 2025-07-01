---
title: State Machines
layout: home
nav_order: 3
parent: Code
---

# State Machines
A state machine is a programming pattern that helps manage different modes of behavior in a game object.
You define a set of states (e.g., useful for the player, which could have the states IDLE, RUNNING, JUMPING) and switch between them based on conditions or inputs. Each state has its own logic.
This prevents spaghetti if/else chains. Works well for players, enemies, menus, or game phases.

---
## Pseudocode State Machine

```
STATE = "IDLE"

function update():
    if STATE == "IDLE":
        if input == "move":
            STATE = "RUN"
        elif input == "jump":
            STATE = "JUMP"

    elif STATE == "RUN":
        move_player()
        if input == "stop":
            STATE = "IDLE"
        elif input == "jump":
            STATE = "JUMP"

    elif STATE == "JUMP":
        apply_gravity()
        if on_ground():
            STATE = "IDLE"
```

*(Pseudocode generated with ChatGPT)*

---
## Common States in Games
* Player:
    * IDLE
    * RUN
    * JUMP
    * ATTACK
    * DEAD

* Enemy:
    * PATROL
    * CHASE
    * ATTACK
    * STUNNED
    * DEAD

* Game:
    * MAIN_MENU
    * PLAYING
    * PAUSED
    * GAME_OVER