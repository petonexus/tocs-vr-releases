# Trails of Cold Steel VR

**Same world. A new perspective.** Explore Erebonia in first person, fight in stereo VR and play with tracked Touch controllers. A fan-made VR mod for the Steam version of Trails of Cold Steel.

> **ALPHA - read this first.** Early alpha. Exploration, dialogue and battles are playable; visual glitches and rough movement remain. Save often and expect changes between releases.
> Tested on: Meta Quest 3 with Virtual Desktop; Windows 11, RTX 4080 SUPER.

**Quick start**

- ALPHA: stereo exploration and battles, with bugs and rough edges.
- Requires the Steam game (PC v1.6, English), Virtual Desktop and the x86 Visual C++ runtime.
- Install: extract the ZIP beside `ed8.exe`. SenPatcher is included.
- Play: connect Virtual Desktop, launch from Steam and load a save. VR starts in the field or battle.
- Controls: left stick to move; A/B to confirm/back. Hold the right Meta button to recenter.

[Website](https://www.trailsvr.pro) - [Releases](https://github.com/petonexus/tocs-vr-releases/releases) - [Nexus Mods](https://www.nexusmods.com/thelegendofheroestrailsofcoldsteel/mods/6) - [Gameplay showcase](https://youtu.be/E8FdEB3rqRY) - [Support on Ko-fi](https://ko-fi.com/petonexus)

## What works today

- **Real stereo VR.** Stereo views with head tracking: look around and lean into the scene.
- **First-person exploration.** Explore in first person with free movement and smooth or step turning. Look down to see your body: Rean and every school leader up to chapter 3 have their own body and hands. Y switches the field leader.
- **Tracked hands and weapons.** Tracked hands for every school leader with fingers that follow the controller, their own weapon in your hand while you hold A or the right grip, an arm swing to attack, and their attack effects.
- **Battles in VR.** The original battle camera with head tracking and a level floor, a floating HUD that follows when you turn away, and linked portraits. Enemy HP, damage and status icons float on the enemies. Link, Swap, Link Attack and the S-Break wheel open on a flat panel with the battle around it. The controllers vibrate with the game.
- **Menus, dialogue and scenes.** Read dialogue, shops and menus on a panel. Story scenes use a 16:9 screen; pause and battle results use a level game screen a little farther away.
- **VR settings menu.** Click the right stick in the field: turn speed and step turning, battle camera (following or locked), a third-person exploration camera and the world size (from the next start), S-Craft animation on a flat screen and the panel positions. Your choices are saved.
- **Field map and HUD.** Left trigger opens the field map; hold the right trigger for Quick Navigation. Hold X to show the field HUD.

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

- **The game.** The Legend of Heroes: Trails of Cold Steel on Steam, PC version 1.6, English executable (`ed8.exe`).
- **VR.** A VR headset connected with Virtual Desktop, which must be your active OpenXR runtime. Tested with a Meta Quest 3 and its Touch controllers.
- **Visual C++.** Microsoft Visual C++ Redistributable 2015-2022 (x86), latest version. Without it the game does not start (Windows reports a missing `MSVCP140.dll` or `VCRUNTIME140.dll`).

## Install

1. Close the game and open the folder that contains `ed8.exe` (Steam: right-click the game > Manage > Browse local files).
2. Extract everything from the ZIP into that folder, keeping its folders. If Windows asks to replace `DINPUT8.dll`, say yes: SenPatcher is included (keep a copy of yours if you may want to go back).

Then connect Virtual Desktop, start the game from Steam and load a save (see First launch). To update later, extract the new ZIP over the old files; your saves are never touched.

**Verify a download.** Compare the SHA-256 of the ZIP (Get-FileHash <zip> in PowerShell) with the one on the release page.

## First launch and how to play

1. Connect Virtual Desktop, then start the game from Steam. The title screen and the Load menu are on the flat PC window: pick your save with the keyboard or mouse (a gamepad does not work with the mod yet).
2. VR starts by itself at your first field or battle. From then on, use your Touch controllers (see Controls).

- Look straight ahead when VR starts, and hold the Meta button on the right controller to recenter at any time.
- Take breaks. If smooth turning bothers you, pick step turning in the VR settings menu.

## Controls

Right hand is the dominant hand. Everything below has been used by the author in the headset unless it is marked experimental.

#### Exploration

| Control | What it does |
|---|---|
| **Head** | Look around and lean in. |
| **Left stick** | Walk and run (push further to go faster). |
| **Right stick (left / right)** | Turn. |
| **A** | Confirm, talk, interact, attack. The weapon shows while you hold A or the right grip. |
| **Right grip (hold)** | Hold the weapon; swing the arm to attack. |
| **B** | Cancel / back (also closes the map). |
| **Left menu button** | Camp menu. |
| **Left trigger** | Field map. |
| **Right trigger (hold)** | Quick Navigation (fast travel) on a flat screen. |
| **X (hold, left)** | Show the field HUD while held. |
| **Y (click, left)** | Switch the field leader. |
| **Right stick (click)** | VR settings menu: left stick moves and changes values, A selects, B closes. Saved. |
| **Right hand (menu open)** | Point at a row, pull the trigger. *(experimental)* |

#### Battle

| Control | What it does |
|---|---|
| **Head** | Look around the battle camera and lean in. |
| **Left stick** | Pick commands, targets and arts. |
| **A / B** | Confirm / cancel. |
| **Left trigger (hold)** | S-Craft: hold it, push the stick toward the S-Craft, confirm with A. |
| **Right trigger** | Skip the battle animation. |
| **Arm swing (target pick)** | Confirms the Attack target. *(experimental)* |
| **Left grip (hold)** | Link: hold to open the flat panel. Pick a partner with the stick, confirm with A. Link Attack also uses a flat panel (A = Assist). |
| **Right grip (hold)** | Swap: hold to open the flat party panel. Pick a member with the stick, confirm with A. |
| **Y (click, left)** | Burst during a Link Attack (Tab). Not seen working in play yet. *(experimental)* |

#### Menus, dialogue and results

| Control | What it does |
|---|---|
| **Left stick, A, B** | The same buttons work in menus, shops and dialogue. They show on a floating panel; battle results are full screen. |

#### Anywhere

| Control | What it does |
|---|---|
| **Meta button (right controller, hold)** | Recenter the view where you are looking. VR also centres itself at the start and after a battle. |

Nothing else is mapped: the other buttons do nothing in this alpha.

## Known issues in this alpha

- **Title screen and Load menu are flat.** VR starts at your first field or battle after loading a save. Until then use the keyboard or mouse on the PC (a gamepad does not work with the mod yet).
- **Tested at 3440x1440 and 1920x1080.** At 1920x1080 (16:9) characters look less sharp than at 3440x1440 (21:9) unless they are close.
- **Tremor while walking, shaky hands while turning.** Walking can show some tremor or flicker, and your hands may shake while you turn with the right stick. Smoothing is the first thing planned for V1.1.
- **Some battle visual glitches.** A stray CP/EP gauge can appear after some turn bonuses. S-Craft camera cuts may feel abrupt, and some light halos look clipped after pausing.
- **The game may close by itself.** After some long sessions the game has closed on its own. Save often.
- **Some outfits hide hands.** Some alternate outfits still hide the hands or the body; no sword trail yet.
- **The settings menu is basic.** No seated mode or hand swap yet; the camera and world size apply at the next start.
- **Story scenes are on a flat panel.** Cutscenes play on a flat 16:9 panel, mini-games and fishing are not adapted, and there is no positional audio.

## If something goes wrong

- **The game does not start, or Windows says `MSVCP140.dll` or `VCRUNTIME140.dll` is missing.** Install the latest Microsoft Visual C++ Redistributable 2015-2022 (x86), then start the game again.
- **The game stays on the flat window and never enters VR.** Make sure Virtual Desktop is connected and is your active OpenXR runtime before you start the game, then load a save: VR starts at the first field or battle. If it still does not, close the game and try again.
- **The view is off-axis.** Hold the Meta button on the right controller to recenter where you are looking.

## Roadmap

*A direction, not a deadline. These are plans, not promises, with no dates, and the order can change with what testers report.*

| Stage | Theme | What it brings |
|---|---|---|
| **V1 - this alpha (0.1.0-alpha.4)** (Now) | Explore, talk, fight | Stereo exploration, tracked hands and sword; Battles, linked portraits, Link/Swap panels and Touch controls; Dialogue, menus, scenes and results on panels; In-VR settings menu that remembers your choices; Leaders' bodies, hands and weapons; arm-swing attack; Enemy HP, damage and status icons on each enemy; S-Break wheel on a flat panel |
| **V1.1 - fixes after launch** (Next) | Smoother and clearer | Less tremor while walking and steadier hands while turning; Fixes from early feedback and a controls reference in VR |
| **V2 wave 1 - comfort and settings** (Planned) | Make it yours | Seated mode and hand swap in the VR settings menu; Play with a regular gamepad in VR; Fie and the later party members as field leader |
| **V2 wave 2 - battle and controls** (Planned) | Better fights | Item done properly; S-Craft polish and results in 3D |
| **V2 wave 3 - presence and world** (Later) | Be there | Full body for each character; Sword trail that follows your swing; Mini-games, fishing and cards; Positional audio |
| **V3 - installer** (Later) | One-click install | A proper installer with backups (the ZIP stays available) |

If support allows, Trails of Cold Steel II, III and IV come after this mod. *(Roadmap reviewed 2026-10-09.)*

## Uninstall

1. Close the game.
2. Delete `DINPUT8.dll`, the `vr\` folder (it also holds `vr\in_vr_settings.json`) and the `tocs-vr\` folder from the game folder.
3. Delete `config\defaults.json` and `config\production_profile.selector` (and `config\` if it is empty).
4. Put back your own `DINPUT8.dll` if you kept one.

Your saves are never touched. Log files such as `vr-mod-diagnostic.log` can be deleted too.

## Report a problem

Tell us the mod version (the ZIP name), your headset and what you were doing.

To attach a log: close the game, open `config\defaults.json` in a text editor, change "debug_log": false to true, play until the problem happens and send `vr-mod-diagnostic.log` from the game folder. Set it back to false afterwards, because the log grows quickly. If the game never enters VR, change "debug_log_lifecycle": false to true instead (a much smaller log).

## Videos

[Watch the pre-alpha gameplay showcase](https://youtu.be/E8FdEB3rqRY): exploration, battles, Blade and the opening of the game.

## Support Development

This mod is developed independently in spare time. If you would like to support continued development, you can donate on Ko-fi. Support is optional and is not a pre-order or a promise of a release date.

[![Support me on Ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/petonexus)

## Disclaimer

Unofficial fan-made project, not affiliated with or endorsed by Nihon Falcom. The Legend of Heroes, Trails and all related intellectual property belong to their respective owners. You need your own copy of the game; no game files are included.

## Licenses

Each release has a versioned mod ZIP, a SHA-256 checksum, installation instructions, release notes and known issues. The ZIP contains the combined SenPatcher/VR loader, the Khronos OpenXR loader, the mod's configuration, a hash manifest, and the applicable third-party license texts. A separate SenPatcher download is not required.

The original VR mod portions are Copyright © 2026 petonexus; third-party components retain their own licenses. See [LICENSE.txt](tocs-vr/LICENSE.txt) and [THIRD_PARTY_NOTICES.txt](tocs-vr/THIRD_PARTY_NOTICES.txt). Release ZIPs include these files and the license texts under `tocs-vr/licenses/`.
