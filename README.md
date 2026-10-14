# Trails of Cold Steel VR

**Same world. A new perspective.** A fan-made VR mod for Trails of Cold Steel on Steam. Explore in first person, use tracked Touch controllers and fight with views made for VR: a tabletop miniature, a battle panel you place yourself and your arts list on your hand.

> **ALPHA - read this first.** Early alpha. Exploration, dialogue and battles work, with visual glitches and rough movement. Save often.
> Tested on: Meta Quest 3 with Virtual Desktop; Windows 11, RTX 4080 SUPER.

**Quick start**

- ALPHA: first-person exploration and battles made for VR (a tabletop miniature, a battle panel you place yourself), with bugs and rough edges.
- Requires the Steam game (PC v1.6, English), Virtual Desktop and the x86 Visual C++ runtime.
- Install: extract the ZIP beside `ed8.exe`. SenPatcher is included.
- Play: connect Virtual Desktop, launch from Steam and load a save. VR starts in the field or battle.
- Controls: left stick to move; A/B to confirm/back. Hold the right Meta button to recenter.

[Website](https://www.trailsvr.pro) - [Releases](https://github.com/petonexus/tocs-vr-releases/releases) - [Nexus Mods](https://www.nexusmods.com/thelegendofheroestrailsofcoldsteel/mods/6) - [Gameplay showcase](https://youtu.be/E8FdEB3rqRY) - [Support on Ko-fi](https://ko-fi.com/petonexus)

## What works today

- **Tabletop battles.** Watch the fight as a miniature board in front of you. Tilt it, turn it, and the attack, magic and enemy-charge effects turn to face you. Pick it in the VR settings, under Battle view.
- **A battle panel that is yours.** Grab the battle panel with the trigger and drag it where you want, change its distance and size, and make it follow your head or park it in space. Your choices are saved.
- **Arts and crafts on your hand.** Choose Wrist only in VR settings for the command wheel, target selection and Arts/Crafts list on your left palm in first-person, third-person or miniature battle. Point at a list row with your dominant hand and pull the trigger. Item placement still has a known problem.
- **First-person exploration.** Stereo VR with head tracking, free movement and smooth or step turning. Look down to see your body.
- **Hands and weapons.** Rean and the other school leaders up to chapter 3 have their own body, tracked hands and weapon. Swing your arm to attack.
- **Battles in VR.** The original battle camera with head tracking, enemy HP and status icons floating on the enemies, and controllers that vibrate with the game. First-person battle is there too, as an experiment (VR settings, Battle view).
- **Menus, dialogue and scenes.** Dialogue and shops show on a floating panel. The pause menu opens small on your left wrist when you look at it, or large in front of you, with the world moving behind it. Story scenes play on a 16:9 screen.
- **VR settings menu.** Click the right stick in the field to change turning, cameras, world size and panel positions. Choices are saved.
- **Field map and HUD.** Left trigger opens the field map. Hold the right trigger for Quick Navigation, or X for the field HUD.

## Downloads

Download **tocs-vr-0.1.0-alpha.7-b90e4acc.zip** from the [latest release](https://github.com/petonexus/tocs-vr-releases/releases).

SHA-256: `226309acd335d4e0229c2f705dfa3d63002a85059456665921e06d2929ce1e7f`

**New in 0.1.0-alpha.7**

- First-person battle: point at the target with your dominant hand and pull the trigger to confirm a normal Attack. Arts and Crafts keep their own selection controls.
- Arts and Crafts: the pointer shows a beam outside the list and a ring on the row you aim at. The stick takes over when you move it; B cancels while the trigger is held.
- First-person battle: the right stick turns your view with the existing menu and action controls preserved.
- Wrist-only commands move out of view during attacks and return when you raise your palm. Your saved panel and camera choices are kept.
- Rean's forearm keeps its shape and joins the elbow and wrist more consistently in the checked first-person poses.
- The body in the world stays normal in the checked Order and Orbment screens. The separate Equipment preview still needs work.

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
| **Left menu button** | Pause (camp) menu. It opens on your left wrist when you look at your hand and in front of you when you look ahead. |
| **Left trigger** | Field map. |
| **Right trigger (hold)** | Quick Navigation (fast travel) on a flat screen. |
| **X (hold, left)** | Show the field HUD. |
| **Y (click, left)** | Switch the field leader. |
| **Right stick (click)** | VR settings menu. Left stick changes values, A selects, B closes. |
| **Right hand (menu open)** | Point and pull the trigger. Battle Arts/Crafts use Wrist only in VR settings in all three battle views. *(experimental)* |

#### Battle

| Control | What it does |
|---|---|
| **Head** | Look around the battle and lean in. |
| **Left stick** | Pick commands, targets and arts. |
| **A / B** | Confirm / cancel. |
| **Left trigger (hold)** | S-Craft: hold, push the stick to the S-Craft, press A. |
| **Right trigger** | Skip the battle animation. |
| **Arm swing (target pick)** | First-person normal Attack, Rean/Jusis only: hold right grip, release left grip, then swing. *(experimental)* |
| **Left grip (hold)** | Link panel: pick a partner with the stick, confirm with A. In a Link Attack, A = Assist. |
| **Right grip (hold)** | Swap panel: pick with the stick, confirm with A. First-person Attack uses grip plus swing (above). |
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

- **Enemy Analysis and Item placement need fixes.** Enemy details can show only the background in the headset, without the model, HP or attributes. Item can stay on the right panel with Wrist only selected. The wrist checks cover wheel, targets and Arts/Crafts.
- **First-person and miniature battle views are new.** Rean's forearm passed three poses; other actors and outfits need checks. The Arts beam can start above the hand. Miniature bars and damage face the active character. Grip Attack: Rean/Jusis checked; weapons: Fie/Machias checked. Gaius can lack a weapon; Elliot/Laura weapons can stay still.
- **The pause menu is new.** Your character in the world stays normal in Order and Orbment. Equipment's separate preview still needs work. Choose wrist, gaze-following or fixed-front placement in VR settings.
- **Title screen and Load menu are flat.** VR starts at the first field or battle. Until then, use the keyboard or mouse.
- **Tested at 3440x1440 and 1920x1080.** At 1920x1080, characters look less sharp unless they are close. The latest battle changes were checked at 3440x1440; their 1920x1080 coverage remains partial.
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
| **V1 - this alpha** (Now) | Explore, talk, fight | Stereo exploration and battles; Bodies, tracked hands and weapons for the school leaders; Dialogue, menus and scenes on panels; In-VR settings menu |
| **V1.1 - fixes after launch** (Next) | Smoother and clearer | Less tremor while walking, steadier hands while turning; Fixes from feedback and a controls reference in VR |
| **V2 - comfort, battle and presence** (Planned) | Make it yours | Seated mode, hand swap and a regular gamepad; Fie and the later party members as field leader; Battle polish: Item, S-Craft and results in 3D; Sword trail, mini-games and positional audio |
| **V3 - installer** (Later) | One-click install | A proper installer with backups (the ZIP stays available) |

If support allows, Trails of Cold Steel II, III and IV come after this mod. *(Roadmap reviewed 2026-10-12.)*

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
