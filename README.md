# Trails of Cold Steel VR

**Same world. A new perspective.** A fan-made VR mod for Trails of Cold Steel on Steam. Explore in first person, fight in stereo and use tracked Touch controllers.

> **ALPHA - read this first.** Early alpha. Exploration, dialogue and battles work, with visual glitches and rough movement. Save often.
> Tested on: Meta Quest 3 with Virtual Desktop; Windows 11, RTX 4080 SUPER.

**Quick start**

- ALPHA: stereo exploration and battles, with bugs and rough edges.
- Requires the Steam game (PC v1.6, English), Virtual Desktop and the x86 Visual C++ runtime.
- Install: extract the ZIP beside `ed8.exe`. SenPatcher is included.
- Play: connect Virtual Desktop, launch from Steam and load a save. VR starts in the field or battle.
- Controls: left stick to move; A/B to confirm/back. Hold the right Meta button to recenter.

[Website](https://www.trailsvr.pro) - [Releases](https://github.com/petonexus/tocs-vr-releases/releases) - [Nexus Mods](https://www.nexusmods.com/thelegendofheroestrailsofcoldsteel/mods/6) - [Gameplay showcase](https://youtu.be/E8FdEB3rqRY) - [Support on Ko-fi](https://ko-fi.com/petonexus)

## What works today

- **First-person exploration.** Stereo VR with head tracking, free movement and smooth or step turning. Look down to see your body.
- **Hands and weapons.** Rean and the other school leaders up to chapter 3 have their own body, tracked hands and weapon. Swing your arm to attack.
- **Battles in VR.** The original battle camera with head tracking. Enemy HP and status icons float on the enemies, and the controllers vibrate.
- **Menus, dialogue and scenes.** Dialogue, shops and menus show on a floating panel. Story scenes play on a 16:9 screen.
- **VR settings menu.** Click the right stick in the field to change turning, cameras, world size and panel positions. Choices are saved.
- **Field map and HUD.** Left trigger opens the field map. Hold the right trigger for Quick Navigation, or X for the field HUD.

## Downloads

Download **tocs-vr-0.1.0-alpha.4-cb85adac.zip** from the [latest release](https://github.com/petonexus/tocs-vr-releases/releases).

SHA-256: `3161baf9ea55ee59c74e068d2323b10670c2869a0abd76adf39e40904d60be27`

**New in 0.1.0-alpha.4**

- Look down to see your body: Rean and the other school leaders have shoulders and arms joined to your hands, and the body turns with you.
- Weapons: hold the right grip (or A) to hold your leader's weapon and swing your arm to attack. Every school leader up to chapter 3 has their own weapon and attack effects.
- Your fingers follow the controller (trigger, grip and thumb), Machias' hands show and each leader sees from their own eye height.
- Battles: the HUD panel follows when you turn away, the floor stays level, status icons sit on each enemy, the controllers vibrate with the game, and an arm swing can confirm your Attack.
- Menus: point at the VR settings menu with your hand, hold the right trigger for Quick Navigation on a flat screen, and turning VR off or pausing keeps the game's proportions.
- New VR settings: step turning, a third-person camera and the world size. Doors and loads fade in from black, and the image is less washed-out.

## Requirements

- **The game.** Trails of Cold Steel on Steam, PC version 1.6, English (`ed8.exe`).
- **VR.** A headset with Virtual Desktop as the active OpenXR runtime. Tested with a Meta Quest 3 and Touch controllers.
- **Visual C++.** Microsoft Visual C++ Redistributable 2015-2022 (x86). Without it the game does not start.

## Install

1. Close the game and open the folder that contains `ed8.exe` (Steam: right-click the game > Manage > Browse local files).
2. Extract everything from the ZIP into that folder, keeping its folders. Say yes to replacing `DINPUT8.dll` (SenPatcher is included; back up yours if you may want it back).

To update, extract the new ZIP over the old files. Your saves are never touched.

**Verify a download.** Compare the SHA-256 of the ZIP (Get-FileHash <zip> in PowerShell) with the one on the release page.

## First launch and how to play

1. Connect Virtual Desktop and start the game from Steam. Load a save with the keyboard or mouse: the title screen is flat, and a gamepad does not work with the mod yet.
2. VR starts by itself at the first field or battle. From then on, use the Touch controllers.

- Look straight ahead when VR starts. Hold the Meta button on the right controller to recenter at any time.
- Take breaks. If smooth turning bothers you, pick step turning in the VR settings menu.

## Controls

Right hand is the dominant hand. Controls marked experimental are not confirmed in play yet.

#### Exploration

| Control | What it does |
|---|---|
| **Head** | Look around and lean in. |
| **Left stick** | Walk; push further to run. |
| **Right stick (left / right)** | Turn. |
| **A** | Confirm, talk, interact, attack. Hold to show the weapon. |
| **Right grip (hold)** | Hold the weapon; swing your arm to attack. |
| **B** | Cancel / back. Also closes the map. |
| **Left menu button** | Camp menu. |
| **Left trigger** | Field map. |
| **Right trigger (hold)** | Quick Navigation (fast travel) on a flat screen. |
| **X (hold, left)** | Show the field HUD. |
| **Y (click, left)** | Switch the field leader. |
| **Right stick (click)** | VR settings menu. Left stick changes values, A selects, B closes. |
| **Right hand (menu open)** | Point at a row, pull the trigger. *(experimental)* |

#### Battle

| Control | What it does |
|---|---|
| **Head** | Look around the battle and lean in. |
| **Left stick** | Pick commands, targets and arts. |
| **A / B** | Confirm / cancel. |
| **Left trigger (hold)** | S-Craft: hold, push the stick to the S-Craft, press A. |
| **Right trigger** | Skip the battle animation. |
| **Arm swing (target pick)** | Confirms the Attack target. *(experimental)* |
| **Left grip (hold)** | Link panel: pick a partner with the stick, confirm with A. In a Link Attack, A = Assist. |
| **Right grip (hold)** | Swap panel: pick a party member with the stick, confirm with A. |
| **Y (click, left)** | Burst during a Link Attack. *(experimental)* |

#### Menus, dialogue and results

| Control | What it does |
|---|---|
| **Left stick, A, B** | Move, confirm and go back in menus, shops and dialogue. |

#### Anywhere

| Control | What it does |
|---|---|
| **Meta button (right controller, hold)** | Recenter where you are looking. VR also recenters at the start and after a battle. |

Other buttons do nothing in this alpha.

## Known issues in this alpha

- **Title screen and Load menu are flat.** VR starts at the first field or battle. Until then, use the keyboard or mouse.
- **Tested at 3440x1440 and 1920x1080.** At 1920x1080, characters look less sharp unless they are close.
- **Tremor while walking and turning.** Walking can show tremor or flicker, and your hands can shake while you turn. Smoothing comes first in V1.1.
- **Battle visual glitches.** A stray CP/EP gauge after some turn bonuses, abrupt S-Craft camera cuts and clipped light halos after pausing.
- **The game may close by itself.** This has happened after long sessions. Save often.
- **Not done yet.** Some outfits hide the hands or body. No seated mode, hand swap, sword trail or positional audio. Mini-games and fishing are not adapted, and cutscenes play on a flat 16:9 panel.
- **Some settings need a restart.** The third-person camera and world size change at the next game start.

## If something goes wrong

- **The game does not start, or `MSVCP140.dll` or `VCRUNTIME140.dll` is missing.** Install the latest Microsoft Visual C++ Redistributable 2015-2022 (x86).
- **The game never enters VR.** Connect Virtual Desktop and make it the active OpenXR runtime before you start the game, then load a save. VR starts at the first field or battle. If not, restart the game.
- **The view is off-axis.** Hold the Meta button on the right controller to recenter.

## Roadmap

*Plans, not promises. No dates, and the order can change with feedback.*

| Stage | Theme | What it brings |
|---|---|---|
| **V1 - this alpha (0.1.0-alpha.4)** (Now) | Explore, talk, fight | Stereo exploration and battles; Bodies, tracked hands and weapons for the school leaders; Dialogue, menus and scenes on panels; In-VR settings menu |
| **V1.1 - fixes after launch** (Next) | Smoother and clearer | Less tremor while walking, steadier hands while turning; Fixes from feedback and a controls reference in VR |
| **V2 - comfort, battle and presence** (Planned) | Make it yours | Seated mode, hand swap and a regular gamepad; Fie and the later party members as field leader; Battle polish: Item, S-Craft and results in 3D; Sword trail, mini-games and positional audio |
| **V3 - installer** (Later) | One-click install | A proper installer with backups (the ZIP stays available) |

If support allows, Trails of Cold Steel II, III and IV come after this mod. *(Roadmap reviewed 2026-10-09.)*

## Uninstall

1. Close the game.
2. Delete `DINPUT8.dll`, the `vr\` folder (it also holds `vr\in_vr_settings.json`) and the `tocs-vr\` folder from the game folder.
3. Delete `config\defaults.json` and `config\production_profile.selector` (and `config\` if it is empty).
4. Put back your own `DINPUT8.dll` if you kept one.

Your saves are never touched. Log files such as `vr-mod-diagnostic.log` can be deleted too.

## Report a problem

Include the mod version (the ZIP name), your headset and what you were doing.

To attach a log, close the game, open `config\defaults.json` and change "debug_log": false to true. Play until the problem happens, then send `vr-mod-diagnostic.log` from the game folder and set it back to false (the log grows fast). If the game never enters VR, set "debug_log_lifecycle" to true instead (a much smaller log).

## Videos

[Watch the pre-alpha gameplay showcase](https://youtu.be/E8FdEB3rqRY): exploration, battles, Blade and the opening of the game.

## Support Development

Made independently in spare time. Ko-fi donations are optional and are not a pre-order or a promise of a release date.

[![Support me on Ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/petonexus)

## Disclaimer

Unofficial fan-made project, not affiliated with or endorsed by Nihon Falcom. The Legend of Heroes, Trails and all related intellectual property belong to their respective owners. You need your own copy of the game; no game files are included.

## Licenses

Each release has a versioned mod ZIP, a SHA-256 checksum, installation instructions, release notes and known issues. The ZIP contains the combined SenPatcher/VR loader, the Khronos OpenXR loader, the mod's configuration, a hash manifest, and the applicable third-party license texts. A separate SenPatcher download is not required.

The original VR mod portions are Copyright © 2026 petonexus; third-party components retain their own licenses. See [LICENSE.txt](tocs-vr/LICENSE.txt) and [THIRD_PARTY_NOTICES.txt](tocs-vr/THIRD_PARTY_NOTICES.txt). Release ZIPs include these files and the license texts under `tocs-vr/licenses/`.
