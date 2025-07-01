---
title: Project Structure
layout: home
nav_order: 1
parent: Code
---

# Project Structure
Try to keep your project clean and modular. Structure your files so that it's easy to find and reuse scenes, scripts, and assets. 

{: .note }
> When you work in a team with multiple programmers, and you use Git for version controlling, your *in-progress structure* might not always be the final or optimal structure. To avoid merge conflicts and losing progress, it often makes sense that only one person works within one scene. Therefore, you might split up things that would otherwise go into the same scene. Whenever a component - even if it is not large - is finalized, try to merge it before starting on the next part of the project. This way, you avoid large merge conflicts later on and can clean up your project structure on the run.

## Potential Folder Layout

```
 📁 game project
  ├─ 📁 assets
  │   ├─ 📁 sprites
      ├─ 📁 audio
      ├─ 📁 fonts
      ├─ 📁 dialogue-scripts
      └─ 📁 particles
  ├─ 📁 globals
      ├─ 📁 audio-manager
      └─ 📁 game-manager
  ├─ 📁 UI
      └─ 📁 menus
  ├─ 📁 scenes
      ├─ 📁 player
      ├─ 📁 enemy
      ├─ 📁 levels
      └─ 📁 
  ├─ 📁 scripts
  └─ README.md
```

* assets: all files you want to import, e.g., art, audio, texts
* UI: everything that is part of the user interface, e.g., 
* scenes: all kinds of elements in your game, e.g., player, enemies, level (scene-specific scripts can go in these subfolders, too)
* scripts: other scripts

### Group by Purpose vs. File Type
How to structure a project depends also on personal preferences. Some people might prefer to strictly separate scripts and scenes, whole others like to group files by purpose rather than by type (e.g., putting the player scene in the same folder with the player script).

{: .note-title }
> 💡 Tipp
>
>Name related scripts and scenes the same, e.g., *player.scene* and *player.script*.