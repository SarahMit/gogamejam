---
title: Getting Started
layout: home
nav_order: 2
---


# Getting Started

You can join a game jam either solo or as part of a team. If you're attending an on-site jam, you can usually find teammates there, so there's no need to form a group in advance. When working as a team, tasks are typically divided — for example, who will write which scripts or create or source which assets.

{: .note }
> While creating your own assets can be a lot of fun, it also takes time. If you don’t plan to make art or sound yourself, you can explore plenty of [free online resources](assets/free-resources.md).

Before diving into development, make a plan for the game you're creating — see [Game Design](game-design.md) for guidance. Once you have a concept, coordinate with your team to divide responsibilities and set up a basic workflow.
One of the most common mistakes during game jams is splitting up the work, working independently, and only trying to merge everything at the end. This often leads to serious issues — not just time pressure but also technical problems like merge conflicts that can corrupt your game project.
While game jams are about creativity and fun, it's a good idea to set up a **basic working plan** with your team.

---

## Workflow
Schedule regular team check-ins, ideally two to three times a day or every few hours. In each meeting, cover:

* What each team member is working on, what’s finished, and any problems encountered
* Open questions or design discussions
* Whether the project is on track with the schedule — and if not, whether scope should be reduced
* Next steps: who will do what
* Which components should be merged, and **do the merging together** to avoid conflicts

Some people prefer focusing only on art or programming, while others like to mix. Create a rough task distribution at the beginning of the jam based on interests.
In your **initial meeting**, discuss what each person wants to do and assign clear first tasks. During your regular meetings, adjust and plan upcoming tasks. If someone finishes early and doesn't know what to do, discuss their next task together as a team — **don’t just start working independently without letting others know!**

---

## General Game Components to Start With
Here are some typical game components that individuals can work on:

1. **🎨 Art:** Start with essential assets, like the player sprite. Art takes time, so programmers will often begin with placeholders. Agree on sprite resolutions early so placeholders and final art match in size (this avoids rework later).
Check out [Art](assets/art.md) if you're creating your own sprites, or [Free Resources](assets/free-resources.md) for ready-made assets.
Avoid over-polishing your art early on — aim for a clean, usable style you can refine later if time allows.

2. **🧠 Game Manager:** The game manager handles things like transitions between menus, levels, and game states. Since it's a core part of the game logic, this is best handled by a more experienced game developer.

3. **📋 Menu:** Menus are often separate from the main game logic. This makes them great starter tasks, especially for team members who want to explore the engine but have limited experience. Just keep in mind that menu transitions may need coordination with the game manager.

4. **🕹️ Player movement:** In some games (e.g. platformers), smooth player movement is critical. While basic movement is easy to implement, getting it to "feel right" takes time and iteration — so it’s smart to tackle early.

5. **🛠️ UI Elements / HUD:** Health bars, score counters, inventory screens, and timers are important for user feedback and game feel. They are often implemented in parallel with core gameplay.

6. **🧱 Level Design / Environment:** Building the actual playable levels or scenes by creating the layout, platforms, obstacles, or backgrounds. Use placeholder art at first, then swap in final assets.

---

## Choosing Your Tools
Below are battle-tested tools that are beginner-friendly, free or cheap, and great for rapid game development.

### 🎮 Game Engine
* 🔷 Godot (Recommended)
    * Open source, lightweight, and perfect for 2D games
    * GDScript is easy to learn, especially for beginners
    * Export to HTML5, Windows, Linux, macOS with minimal hassle
    * Ideal for small-scope games with clean scene/node architecture
* Alternatives: Unity (heavier, steeper learning), Construct (drag & drop), PICO-8 (fantasy console with limits)

### 🎨 Art & Animation
* 🟠 Aseprite (pixel art, animations)
    * Pixel-perfect editor with animation support (onion skin, frame control)
    * Affordable, fast, and widely used in the gamedev community
    * [www.aseprite.org](https://www.aseprite.org)

* 🟢 Piskel (free, web-based)
    * Great free alternative for pixel art & animations
    * https://www.piskelapp.com

* 🔵 LibreSprite (open-source Aseprite fork)
    * Almost identical to Aseprite, but free
    * https://libresprite.github.io

### 🔊 Sound & Music
* 🔊 BFXR / SFXR (SFX generators)
    * Generate jump, shoot, hit, pickup sounds instantly
    * https://www.bfxr.net

* 🎵 BeepBox (music generator)
    * Web-based music composer, great for chiptunes
    * https://www.beepbox.co

* 🎶 Bosca Ceoil Blue (looping music tool)
    * Simple music-making software made for devs
    * https://yurisizov.itch.io/boscaceoil-blue

### 🛠️ Other Handy Tools
* Tiled – 2D tilemap editor (can import into Godot)
    * https://www.mapeditor.org

* TinyPNG – Compresses PNG files without quality loss
    * https://tinypng.com

[Game Design →](game-design.md){: .btn }
