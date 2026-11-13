# Trails of Cold Steel VR

**Same world. A new perspective.** Free VR mod for Trails of Cold Steel: tracked hands, battles and palm menus.

> **1.4.0 - official release.** Stable stick locomotion (DLSS), ally hand targeting, seated mode. Save often.
> Tested on: Meta Quest 3 with Virtual Desktop; Windows 11, RTX 4080 SUPER.

**[Download](https://github.com/petonexus/tocs-vr-releases/releases/latest/download/tocs-vr-1.4.0.zip)** · [Website](https://www.trailsvr.pro) · [Nexus Mods](https://www.nexusmods.com/thelegendofheroestrailsofcoldsteel/mods/6) · [Video](https://youtu.be/BCXjr3M0slI) · [Ko-fi](https://ko-fi.com/petonexus)

**Quick start**

- 1.4.0: depth-reprojected stick locomotion (DLSS), ally hand targeting, seated mode, roomscale. DLSS and first-person combat are experimental.
- Requires the Steam game (PC v1.6, English), Virtual Desktop and Visual C++ x86.
- Extract the ZIP beside `ed8.exe`. Keep Steam open; start `tocs-vr\TocsVrPlayer.exe`.
- Touch controls: left stick, A to confirm, B to go back. Hold the right Meta button to recenter.

## Features

- **First-person exploration.** Stereo first person with a visible body, tracked hands and fingers, leaning, and smooth or snap turning (15 to 90 degrees). Play seated or standing; real steps move the character.
- **Hands and weapons.** Hold the right grip to draw your leader's weapon and swing to attack (it triggers the attack; no collision combat). School leaders through chapter 3 have their own weapons; Rean has an optional hip holster. Alisa shoots her bow with both grips and Gaius thrusts his lance.
- **Three ways to battle.** The original third-person camera, a tabletop miniature you turn, tilt and scale (enemy HP under their feet), or experimental first person. Battles stay turn-based; switch the view in VR settings or the Touch launcher options.
- **ARCUS on your palm.** With Wrist only, the command wheel, targets and Arts/Crafts lists sit on your left palm. Pick with the stick and A, or confirm an Art with a character pose (glowing rings, haptics). In first-person and tabletop battles, point an open hand at an ally for a single-target item or Tear Art. Results open in a window or in 3D on your wrist.
- **Experimental first-person combat.** Walk and see your whole body while choosing a target (stick or open hand, then A). Rean and Jusis swing a wide stroke, Laura and Fie cut, Elliot thrusts or swings, Emma cuts or thrusts, Gaius thrusts and Alisa draws her bow. The target HP bar follows the enemy.
- **Menus, dialogue and story.** Dialogue and shops on a floating panel; the camp menu on your wrist, in front or following your gaze. Move, resize or park the gold battle panel. In first person, story scenes play in 3D through the game camera (default), through Rean's eyes (ultra-immersive, experimental) or on a screen.
- **Map and comfort.** Minimap on your left wrist, field map, Quick Navigation and a gold marker on talkable NPCs. The VR menu holds immersion profiles, turning, scale, seated mode, eye height, arm reach and settings save/restore.
- **Launcher and gamepad.** Pick Touch or gamepad, the x64 presenter (default), the PC eye mirror and a frame mode (60 or 30, with DLSS or OFXR), and (with Touch) edit VR settings without starting the game. Gamepad plays in third person, without gestures or the VR menu. The redesigned in-headset VR menu is experimental.
- **Image, DLSS and recording.** DLSS Quality (default, 100%), Performance (77%) or Ultra performance (67%); DLSS needs the x64 presenter and a compatible NVIDIA GPU, the last two need RTX. In first person it adds depth reprojection for stick movement and foveated reconstruction; it can be turned off for battles. DLSS is experimental (trails may appear) and never combined with OFXR, an optional external tool that is not bundled. The PC window can show both eyes stitched for recording.

## Download

**[Download tocs-vr-1.4.0.zip](https://github.com/petonexus/tocs-vr-releases/releases/latest/download/tocs-vr-1.4.0.zip)** from the [latest release](https://github.com/petonexus/tocs-vr-releases/releases/latest).

<sub>SHA-256: `26b2603bacda9360afe71e2939c15c398262f2415e72380cc2da4647106acf5b`</sub>

<details>
<summary><b>New in 1.4.0</b></summary>

- Depth reprojection for stick locomotion: the presenter reprojects each frame by scene depth for strafe and smooth-turn yaw, so near-field characters and geometry stop juddering between 60 fps frames. Needs DLSS.
- DLSS no longer drops out mid-session: fixed the hand layer failing, which sent the image to the non-DLSS path and left the hands jittering until a restart. Fixed foveated DLSS: lower cost toward the lens periphery.
- Hand-pointed ally targeting: point at a party member to choose who receives a single-target item or Tear healing Art.
- Seated mode, eye-height offset, roomscale steps, arm-reach calibration.
- Save/restore VR settings, battle quick settings, snap turn 15-90 degrees.
- Per-eye ambient occlusion and bloom. Optional hip holster for Rean.

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
- Frame modes: 60 + DLSS (recommended) or 60 + OFXR 2x with VD at 120 Hz; 30 + DLSS or 30 + OFXR 3x (ghosting) with VD at 90 Hz. Set VD and OFXR yourself; the launcher refuses a mode that does not match OFXR and backs up settings.xml.
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
<summary><b>Show all 10</b></summary>

- **DLSS is experimental.** Fast motion can leave trails. DLSS with OFXR frame generation does not hold 120 Hz in heavy scenes, so the launcher keeps them mutually exclusive; choose an OFXR row if DLSS is uncomfortable.
- **Experimental coverage.** Hand ray, F2 capture, gamepad target/orbit, other Analysis routes, enemy icons and later characters/scenes need broader checks.
- **Reprojection limits.** Needs DLSS, first person. UI-layer markers and effects can shimmer in a strafe; the VR menu sways in smooth turns; after many turns the camera can sit 10-45 cm off the character until a recenter.
- **Not yet checked in a headset.** The marker, seated-camera and hand-targeting hitch fixes, the hip holster option and battle steps under reprojection.
- **Enemy Analysis.** Analysis was checked only in first person via View Specifics; other routes and miniature view may omit details.
- **First-person battle is experimental.** Swing confirms Attack, not physical damage. Strikes lack full character coverage. With miniature HP off, game labels can face the actor.
- **Keep the default outfits.** Use default outfits. Other costumes may show incorrectly; report the outfit and scene if affected.
- **Gamepad uses third person.** No Touch gestures or VR menu. Panel settings apply at startup; target/orbit awaits a physical-controller check. Launcher VR settings needs Touch.
- **Flat screens and tested setup.** Title/loading are flat; battle results open in a window by default, and 3D on the wrist is optional. Scenes options apply with first-person Touch; other modes use a screen. Tested: Quest 3 / VD, 3440x1440; no fresh 1920x1080 check.
- **Future features.** No hand swap, positional audio or native 90 FPS. Later leaders and minigames need more work. Some camera and world-size settings need a restart.

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

*Priorities, not delivery dates. Fixes can ship separately as 1.4.x updates.*

| Stage | Theme | What it brings |
|---|---|---|
| **1.4 - locomotion and comfort** (Now) | Stick locomotion without judder and more ways to play | Reprojection, ally targeting, seated mode |
| **1.4.1 - maintenance** (Next) | Check and finish what 1.4 shipped | Headset checks of the 1.4 fixes, camera drift after smooth turns, OFXR with DLSS at 120 Hz, DLSS startup |
| **Next - performance and image** (Planned) | Polish what 1.4 left open | Reduce DLSS trails and OFXR instability; broader headset checks; pacing and rendering cost |
| **Later - comfort and coverage** (Later) | Broader ways to play | Left-handed play, more leaders/minigames, panel themes, positional audio and an installer |

Cold Steel II, III and IV are longer-term possibilities, depending on support. *(Roadmap reviewed 2026-11-12.)*

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
