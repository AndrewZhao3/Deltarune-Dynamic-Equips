# Deltarune: Dynamic-Equips Mod (BETA)

**Dynamic Equips** is an open-source mod for *Deltarune* that dynamically renders weapons and armor overlays onto overworld character sprites.

Currently supports all obtainable armors and scarves in Chapters 1-5

## Features

Over 1k+ hand-drawn sprites for every armor equip and scarf in Deltarune for Kris, Susie, and Ralsei.
Armors are worn differently depending on who's wearing it, and what armor slot it occupies.

<img width="842" height="510" alt="image" src="https://github.com/user-attachments/assets/070b7557-2a72-4072-bd32-dabec0c4c8ae" />

Example of how Kris, Susie, and Ralsei wear the Red Ribbon item differently.

## Installation Guide

### Full Patch 
Includes all the scripts and all the sprites. Recommended for most players.

1. Download this modpack.
2. Download [DeltaPatcher](https://www.romhacking.net/utilities/704/).
3. Open Deltarune's Local Files using "Browse Local Files" in Steam.
4. Use Deltapatcher to patch each respective '.xdelta' file in [`patches/`](./patches) over each Chapter's 'data.win' file.

### Developers & Artists

Recommended if you wish to create your own sprites, or modify the source code.

1. Download UndertaleModLoader
2. Follow the steps in "Full Patch" to patch each respective '.xdelta' file in ['code_only/'](./code_only) over each Chapter's 'data.win' file.
3. You can now add your own sprites or edit the code.

## Known Issues & Limitations

Because *Deltarune* handles lighting systems, cutscene sprite overrides, and room rendering differently across chapters, please keep the following known behaviors in mind during the **BETA**:

* **Cutscene Visibility:** 
  * **Chapter 1:** Cutscenes do not currently support dynamic overlays. Equipment overlays will temporarily disappear during cutscene animations and reappear once control returns to the player.
  * **Chapters 2–5:** Overlays are functional in most cutscenes, but may temporarily disappear during certain scripted story poses or character-specific animations.
* **Sprite Layering & Depth (Ch. 4 & 5):** 
  * In some specific rooms in **Chapter 4** (and very rarely in **Chapter 5**), overlays may occasionally render underneath character sprites instead of on top.
* **Lighting Engine Interactions (Ch. 4 & 5):** 
  * **Chapter 4** is currently the most experimental due to how the game handles room lighting.
  * Overlays are set by default to draw *above* room lighting effects in Chapters 4 and 5. Because of this, equipment overlays may sometimes remain bright or ignore ambient dark/light shaders in specific lit areas.

**Found a new issue or crash?** Submit a bug report under the [Issues](../../issues) tab. Please include your Chapter, room, and current equipped items in both slots.

## License and Usage

**Code:** Licensed under [GNU General Public License v3.0 (GPL-3.0)](./LICENSE).
**Sprites:** Original artwork is created for this project. You can create and distribute your own custom replacement sprites using this system.

*Disclaimer: Deltarune: Dynamic Equips is an unofficial fan-made project and is not affiliated with Toby Fox or Materia Collective.*
