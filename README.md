# Trails of Cold Steel VR

**Same world. A new perspective.** Free VR mod for Trails of Cold Steel: tracked hands, battles and palm menus.

> **1.6.9 - official release.** VR starts sooner after a save loads, and on the Link attack prompt Y does Rush and X does Burst. Save often.
> Tested on: Meta Quest 3 with Virtual Desktop; Windows 11, RTX 4080 SUPER.

**[Download](https://github.com/petonexus/tocs-vr-releases/releases/latest/download/tocs-vr-1.6.9.zip)** · [Website](https://www.trailsvr.pro) · [Nexus Mods](https://www.nexusmods.com/thelegendofheroestrailsofcoldsteel/mods/6) · [Video](https://youtu.be/BCXjr3M0slI) · [Ko-fi](https://ko-fi.com/petonexus)

**Quick start**

- 1.6.9: VR starts sooner after a save loads, and on the Link attack prompt Y does Rush and X does Burst.
- Requires the Steam game (PC v1.6, English), Virtual Desktop and Visual C++ x86.
- Extract the ZIP beside `ed8.exe`. Keep Steam open; start `tocs-vr\TocsVrPlayer.exe`.
- Touch controls: left stick, A to confirm, B to go back. Hold the right Meta button to recenter.

## Features

- **First-person exploration.** Stereo first person with a visible body, tracked hands and fingers, leaning, and smooth or snap turning (15 to 90 degrees). Play seated or standing; real steps move the character. Starting in first person with Touch lets you switch views during exploration. If you start in third person, choose first person and restart once to enable live switching.
- **Hands and weapons.** Hold the right grip to draw your leader's weapon and swing to attack (it triggers the attack; no collision combat). School leaders through chapter 3 have their own weapons; Rean has an optional hip holster. Alisa shoots her bow with both grips and Gaius thrusts his lance.
- **Three ways to battle.** The original third-person camera, a tabletop miniature you turn, tilt and scale, or experimental first person. HP bars hang under allies and enemies; in third person and the miniature X shows or hides them, and hidden bars pop up on damage or healing. With Touch and first-person exploration, the right stick turns the third-person view. Battles stay turn-based; switch the view in VR settings or the Touch launcher options.
- **ARCUS on your palm.** With Wrist only, the command wheel, targets and Arts/Crafts lists sit on your left palm. Pick with the stick and A, or confirm an Art with a character pose (glowing rings, haptics). In first-person and tabletop battles, point an open hand at an ally for a single-target item or Tear Art. Battle results open in a window in front of you.
- **Experimental first-person combat.** Walk and see your whole body while choosing a target (stick or open hand, then A). Rean and Jusis swing a wide stroke, Laura and Fie cut, Elliot thrusts or swings, Emma cuts or thrusts, Gaius thrusts and Alisa draws her bow. The target HP bar follows the enemy.
- **Menus, dialogue and story.** Dialogue and shops on a floating panel; the camp menu on your wrist, in front or following your gaze. Move, resize or park the gold battle panel. In first person, story scenes play in 3D through the game camera (default), through Rean's eyes (ultra-immersive, experimental) or on a screen.
- **Map and comfort.** Minimap on your left wrist, field map, Quick Navigation and a gold marker on talkable NPCs. The VR menu holds immersion profiles, turning, scale, seated mode, eye height, arm reach and settings save/restore.
- **Launcher and gamepad.** Choose English, Brazilian Portuguese or Spanish. Pick Touch or gamepad, the x64 presenter (default), the PC eye mirror and a frame mode (60 or 30, with DLSS or OFXR), and (with Touch) edit VR settings without starting the game. Gamepad plays in third person, without gestures or the VR menu. The redesigned in-headset VR menu is experimental.
- **Image, DLSS and recording.** DLSS Quality (default, 100%), Performance (77%) or Ultra performance (67%); DLSS needs the x64 presenter and a compatible NVIDIA GPU, the last two need RTX. In first person it adds depth reprojection for stick movement and turns, character frame generation at 90 or 120 Hz and foveated reconstruction; it can be turned off for battles. DLSS is experimental (trails may appear) and never combined with OFXR, an optional external tool that is not bundled. The PC window can show both eyes stitched for recording.

## Optional add-ons

- **[Class VII HD](https://www.nexusmods.com/thelegendofheroestrailsofcoldsteel/mods/9).** Optional add-on on Nexus Mods: 2x textures and light proportion tweaks for the playable characters (regular and summer uniforms). One .p3a file for the game's mods folder; it works with or without VR.

## Download

**[Download tocs-vr-1.6.9.zip](https://github.com/petonexus/tocs-vr-releases/releases/latest/download/tocs-vr-1.6.9.zip)** from the [latest release](https://github.com/petonexus/tocs-vr-releases/releases/latest).

<sub>SHA-256: `70c22c6bae64e2c4f248866fcd840b502f1ef72431d6be0bcc14ee1571851e4e`</sub>

<details>
<summary><b>New in 1.6.9</b></summary>

- VR now starts sooner after you load a save: the mod asks Virtual Desktop for the headset details while you are still on the title screen.
- On the Link attack prompt in battle, the left controller's Y button now does Rush and X does Burst, matching the Xbox letters the game shows; elsewhere the buttons work as before.

</details>

## Install

**You need**

- **The game.** Trails of Cold Steel on Steam, PC version 1.6, English (`ed8.exe`).
- **VR.** A headset with Virtual Desktop as the active OpenXR runtime. Tested with a Meta Quest 3 and Touch controllers.
- **Visual C++.** Microsoft Visual C++ Redistributable 2015-2022 (x86). Without it the game does not start.

**Install**

1. Close the game and open the folder that contains `ed8.exe` (Steam: right-click the game > Manage > Browse local files).
2. Extract everything from the ZIP into that folder, keeping its folders. Say yes to replacing `DINPUT8.dll` (SenPatcher is included; back up yours if you may want it back).

<sub>Updates replace `vr\settings.ini.default`, not settings.ini or saves. **Verify a download:** Compare the SHA-256 of the ZIP (Get-FileHash <zip> in PowerShell) with the one on the release page.</sub>

**Play**

1. Connect Virtual Desktop and keep Steam open. Start `tocs-vr\TocsVrPlayer.exe`; x64 is selected by default. Use keyboard or mouse to load a save from the flat title screen.
2. VR starts in the field or battle. Steam direct uses the classic presenter.

<details>
<summary><b>Tips: recentering, gamepad, frame modes, OFXR, panels</b></summary>

- Look ahead at startup. Hold right Meta to recenter; VR settings offers step turning.
- Game controller: third person, L3+R3 recenter; no Touch gestures or VR menu.
- Frame modes: 60 + DLSS (recommended) with VD at 90 or 120 Hz (120 is a little smoother), or 60 + OFXR 2x with VD at 120 Hz; 30 + DLSS or 30 + OFXR 3x (ghosting) with VD at 90 Hz. Set VD and OFXR yourself; the launcher refuses a mode that does not match OFXR and backs up settings.xml.
- Optional OFXR (external): https://github.com/tig3rmast3r/OFXR-Bridge. Start it first, use x64 and turn VD SSW off.
- Panel brightness and opacity: copy `vr\settings.ini.default` to `vr\settings.ini` if it is absent, then under [Video] set panel_brightness (50-150) and panel_opacity (40-100); both default to 100.

</details>

## Controls

Right hand leads; Alisa's bow uses the left. 🧪 = *(experimental)*, needs more checks.

**Exploration**

| Control | What it does |
|:--|:--|
| **Head** | Look around and lean in. |
| <kbd>Left stick</kbd> | Walk; push further to run. |
| <kbd>Right stick</kbd> <sub>left / right</sub> | Turn. |
| <kbd>A</kbd> | Confirm, talk, interact, attack. Hold to show the weapon. |
| <kbd>Right grip</kbd> <sub>hold</sub> | Hold the weapon; swing your arm to attack. |
| **Alisa:** <kbd>Left grip</kbd> / <kbd>Right grip</kbd> | Left holds bow. Right grip near bow: nock, pull, release. Left release cancels. Horizontal aim. |
| <kbd>B</kbd> | Cancel / back. Also closes the map. |
| <kbd>Left menu button</kbd> | Pause (camp) menu on your wrist when looking at your hand, otherwise in front. |
| <kbd>Left trigger</kbd> | Field map. |
| <kbd>Right trigger</kbd> <sub>hold</sub> | Quick Navigation (fast travel) on a flat screen. |
| <kbd>Right trigger</kbd> <sub>hold, in a scene</sub> | Speed up the scene with the game's turbo (Scene turbo in the launcher). |
| <kbd>X</kbd> <sub>hold, left</sub> | Show the field HUD. |
| <kbd>Y</kbd> <sub>click, left</sub> | Switch the field leader. |
| <kbd>Right stick</kbd> <sub>click</sub> | VR settings menu. Left stick changes values, A selects, B closes. |
| **Right hand** <sub>menu open</sub> | Point; trigger changes a value on its left or right side. 🧪 |

**Battle**

| Control | What it does |
|:--|:--|
| **Head** | Look around the battle and lean in. |
| <kbd>Left stick</kbd> | Pick commands, targets and arts. |
| <kbd>Stick click</kbd> <sub>target pick</sub> | First person. Center and click swaps walking and choosing a target. A confirms. 🧪 |
| **Open hand** <sub>target pick</sub> | First person: aim at an enemy. Stick wins until the next selection. A confirms. 🧪 |
| <kbd>A</kbd> / <kbd>B</kbd> | Confirm / cancel. |
| <kbd>Left trigger</kbd> <sub>hold</sub> | S-Craft: hold, push the stick to the S-Craft, press A. |
| <kbd>Right trigger</kbd> | Skip the battle animation. |
| **Arm swing** <sub>target pick</sub> | First-person Attack: hold right grip, left free. Rean/Jusis: wide forward, side or down stroke. Laura/Fie: cut. Elliot: thrust or swing. Emma: cut/thrust. Gaius: thrust. 🧪 |
| **Alisa:** bow <sub>target pick</sub> | First-person Attack: hold left grip; grip near bow with right, pull, release right grip. Left release cancels; A also confirms. 🧪 |
| <kbd>Left grip</kbd> <sub>hold</sub> | Link: stick selects, A confirms; A = Assist in Link Attack. Alisa uses this grip for her bow. |
| <kbd>Right grip</kbd> <sub>hold</sub> | Swap: choose with stick, A confirms. First-person Attack: grip plus swing. |
| <kbd>X</kbd> <sub>click, left</sub> | 3rd person, miniature: show/hide HP bars. |
| <kbd>Y</kbd> <sub>click, left</sub> | Burst during a Link Attack. 🧪 |

**Menus, dialogue and results**

| Control | What it does |
|:--|:--|
| <kbd>Left stick</kbd>, <kbd>A</kbd>, <kbd>B</kbd> | Move, confirm and go back in menus, shops and dialogue. |

**Anywhere**

| Control | What it does |
|:--|:--|
| <kbd>Meta button</kbd> <sub>right controller, hold</sub> | Recenter where you are looking. VR also recenters at the start and after a battle. |

Use the VR menu for camera and panel options. Gamepad uses the game's native controls.

## Known issues

<details>
<summary><b>Show all 9</b></summary>

- **DLSS is experimental.** Fast movement can leave faint trails. DLSS never runs with OFXR, the optional external frame tool: together they miss 120 Hz in busy scenes. If DLSS bothers you, pick an OFXR frame mode.
- **Smooth walking and turning.** Stick smoothing needs DLSS and first person. Some markers can flicker when you walk sideways, the VR menu sways in smooth turns, and turns in game-camera story scenes are less smooth.
- **Less tested.** Little testing so far: the hand pointer, F2 problem capture, gamepad in the miniature, enemy status icons, the mod's character frame generation, real steps in battle, the full package and later chapters.
- **Enemy Analysis.** Checked only in first-person battle via View Specifics. Other ways to open it, and the miniature, may leave out details.
- **First-person battle is experimental.** A swing chooses Attack; the blade does not hit physically. In the miniature with the mod's HP bars off, the game's own enemy labels may tilt away from you.
- **Keep the default outfits.** Other outfits may show the body or hands wrongly; report the outfit and scene.
- **Gamepad uses third person.** No hand gestures, VR menu or mod HP bars; panel settings apply at game start. Launcher VR settings need Touch controllers.
- **Flat screens, restarts and tested setup.** Title and loading screens are flat; battle results open in a window. Scene options need first person with Touch. Some camera and world-size settings need a restart. Tested: Meta Quest 3, Virtual Desktop, 3440x1440 monitor; 1920x1080 not rechecked.
- **Not in the mod.** No left-handed mode, positional audio or native 90 FPS. Characters who join after chapter 3 have no VR weapon; minigames are not adapted for VR.

</details>

## More

<details>
<summary><b>If something goes wrong</b></summary>

- **The game does not start, or `MSVCP140.dll` or `VCRUNTIME140.dll` is missing.** Install the latest Microsoft Visual C++ Redistributable 2015-2022 (x86).
- **The game never enters VR.** Set Virtual Desktop as the active OpenXR runtime, then load a save. VR begins in the field/battle. Restart if needed.
- **The view is off-axis.** Hold the Meta button on the right controller to recenter.

</details>

<details>
<summary><b>Roadmap</b></summary>

*Priorities, not delivery dates.*

| Stage | Theme | What it brings |
|---|---|---|
| **1.6.9 - current version** (Now) | Faster VR start and Rush on the Link attack prompt | VR starts sooner after a save loads; On the Link attack prompt, Y does Rush and X does Burst on the left controller; Battle tips show in the headset, the park battle floor is no longer black, and the first-person view stays out of big enemies |
| **1.6.x - fixes and maintenance** (Next) | Keep what exists working well | Fixes for reported problems and small, targeted improvements to existing features |
| **Trails of Cold Steel II in VR** (Planned) | The next game | Bringing the VR mod to Trails of Cold Steel II |

Player requests can be added to the list. *(Roadmap reviewed 2026-11-23.)*

</details>

<details>
<summary><b>Uninstall</b></summary>

1. Close the game.
2. Delete `DINPUT8.dll`, the `vr\` folder (it also holds `vr\in_vr_settings.json`) and the `tocs-vr\` folder from the game folder.
3. Delete `config\defaults.json` and `config\production_profile.selector` (and `config\` if it is empty).
4. Put back your own `DINPUT8.dll` if you kept one.

Your saves are never touched. Log files such as `vr-mod-diagnostic.log` can be deleted too.

</details>

<details>
<summary><b>Report a problem</b></summary>

Include the mod version (the ZIP name), your headset and what you were doing.

To attach a log, close the game, open `config\defaults.json` and change "debug_log": false to true. Play until the problem happens, then send `vr-mod-diagnostic.log` from the game folder and set it back to false (the log grows fast). If the game never enters VR, set "debug_log_lifecycle" to true instead (a much smaller log).

</details>

## Support

Made independently in spare time. Ko-fi donations are optional and are not a pre-order or a promise of a release date.

[![Support me on Ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/petonexus)

---

<sub>Unofficial fan mod. No Falcom/NVIDIA endorsement. Trails IP belongs to its owners. Requires your own game; no game files. NVIDIA components have separate licenses. Original mod code Copyright © 2026 petonexus; third-party components (SenPatcher, the Khronos OpenXR loader and others, all included in the ZIP) keep their own licenses: [LICENSE.txt](tocs-vr/LICENSE.txt), [THIRD_PARTY_NOTICES.txt](tocs-vr/THIRD_PARTY_NOTICES.txt) and `tocs-vr/licenses/` in every ZIP.</sub>
