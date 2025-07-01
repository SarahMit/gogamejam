---
title: Character Controller
layout: home
nav_order: 4
parent: Code
---

# Character Controller
This is one of the most important scripts in a game as it denies how user input is translated into character behavior, essentially determining how playing your game feels.
Just getting to make the character to move based on input is easy, game engines usually have a lot of pre-built features for it. However, making character movement feel good and satisfying might be tricky.

## Check Stuff
* jumping / is on floor
* is sliding


## Input Handling
Many game engines offer premade solutions, e.g., 🤖 [Godot's Input Map](https://docs.godotengine.org/en/latest/tutorials/inputs/input_examples.html#inputmap). 
In code, you can then check if a button is pressed and what should happen if that is true.

E.g., adjust the coordinates of your character, to update their position when they are supposed to move:

```
if Input.is_pressed("move_left"):
    character.position.x -= movement_speed * delta_time
```

{: .note }
> Actions, such as movement, should always be scaled with the delta time (sometimes it's just called 'delta'), otherwise your character's movement speed depends on the performance of the PC!The delta time represents the time elapsed in seconds since the last frame was rendered. This value is important to ensure consistent game speed regardless of the frame rate.

For some input, you might want to check the current state of the character. E.g., to prevent endless jumping, check if your player is currently touching the floor before allowing them to jump again. Some game engines might offer more elegant pre-made solutions for this.

```
bool can_jump = false

if collision_with_ground():
    can_jump = true
else:
    can_jump = false

if can_jump and Input.pressed("jump"):
    jump()
```

## Signals and Events
Often, game engines offer to emit *signals* or trigger *events*. These concepts come in handy, e.g., when your characters dies and you want to communicate this to your Game Manager or UI. It is worth an online search to figure out what you tool of choice offers before making scripts too complex or global. E.g., see [how Signals work in 🤖 Godot](https://docs.godotengine.org/en/4.4/getting_started/step_by_step/signals.html)
