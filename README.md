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
- **First-person exploration.** Explore in first person with free movement and smooth turning. Y switches the field leader, and the other school leaders get their own hands.
- **Tracked hands and weapons.** Tracked hands, the leader's own weapon while holding A (Rean, Jusis, Alisa and Emma), and Rean's native slash effect.
- **Battles in VR.** The original battle camera with head tracking, a floating HUD and linked portraits. Enemy HP and damage float on the enemies. Link, Swap, Link Attack and the S-Break wheel open on a flat panel with the battle around it.
- **Menus, dialogue and scenes.** Read dialogue, shops and menus on a panel. Story scenes use a 16:9 screen; pause and battle results use a level game screen a little farther away.
- **VR settings menu.** Click the right stick in the field: turn speed, battle camera (following or locked), S-Craft animation on a flat screen and the panel positions. Your choices are saved.
- **Field map and HUD.** Left trigger opens the field map. Hold X to show the field HUD.

## Downloads

Download **tocs-vr-0.1.0-alpha.3-d1795093.zip** from the [latest release](https://github.com/petonexus/tocs-vr-releases/releases).

SHA-256: `523571ea43a371d9cfd72ed73f536c555b22413466c43a70a1473eafc815c032`

**New in 0.1.0-alpha.3**

- VR settings menu: click the right stick in the field to change turn speed, the battle camera (following or locked), the S-Craft animation on a flat screen and the panel positions. Your choices are saved.
- The other school leaders get their own hands, and Jusis, Alisa and Emma hold their weapon while you hold A.
- Enemy HP, damage and the target arrow float on the enemies; your party's numbers stay on the HUD panel.
- The S-Break wheel opens on a flat panel; pause and battle results are level and a little farther away.
- Sideways walking sends depth to Virtual Desktop to reduce judder (a first step; the effect is subtle).
- Fixes: Alisa's hands, a texture strip on Jusis's and Emma's arm, the party HP bar on the HUD panel and Emma's glasses.

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

1. Connect Virtual Desktop, then start the game from Steam. The title screen and the Load menu are on the flat PC window: pick your save with the keyboard, mouse or a gamepad.
2. VR starts by itself at your first field or battle. From then on, use your Touch controllers (see Controls).

- Look straight ahead when VR starts, and hold the Meta button on the right controller to recenter at any time.
- Take breaks. Turning is smooth only, so go easy if you are sensitive to motion.

## Controls

Right hand is the dominant hand. Everything below has been used by the author in the headset unless it is marked experimental.

#### Exploration

| Control | What it does |
|---|---|
| **Head** | Look around and lean in. |
| **Left stick** | Walk and run (push further to go faster). |
| **Right stick (left / right)** | Turn. |
| **A** | Confirm, talk, interact, attack. The leader's weapon is in your hand only while you hold A. |
| **B** | Cancel / back (also closes the map). |
| **Left menu button** | Camp menu. |
| **Left trigger** | Field map. |
| **X (hold, left)** | Show the field HUD while held. |
| **Y (click, left)** | Switch the field leader. |
| **Right stick (click)** | VR settings menu: left stick moves and changes values, A selects, B closes. Saved. |

#### Battle

| Control | What it does |
|---|---|
| **Head** | Look around the battle camera and lean in. |
| **Left stick** | Pick commands, targets and arts. |
| **A / B** | Confirm / cancel. |
| **Left trigger (hold)** | S-Craft: hold it, push the stick toward the S-Craft, confirm with A. |
| **Right trigger** | Skip the battle animation. |
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

- **Title screen and Load menu are flat.** VR starts at your first field or battle after loading a save. Until then use the keyboard, mouse or a gamepad on the PC.
- **Tested at 3440x1440 and 1920x1080.** At 1920x1080 (16:9) characters look less sharp than at 3440x1440 (21:9) unless they are close.
- **Tremor while walking, shaky hands while turning.** Walking can show some tremor or flicker, and your hands may shake while you turn with the right stick. Smoothing is the first thing planned for V1.1.
- **Status icons are on the battle HUD.** Enemy HP, damage and the target arrow float on the enemies; status icons stay on the HUD panel.
- **Some battle visual glitches.** A stray CP/EP gauge can appear after some turn bonuses. S-Craft camera cuts may feel abrupt, and some light halos look clipped after pausing.
- **The game may close by itself.** After some long sessions the game has closed on its own. Save often.
- **Weapons are basic.** Only Rean, Jusis, Alisa and Emma show a weapon, some outfits hide hands, and there is no gesture attack or sword trail yet.
- **The settings menu is basic.** No snap turn, seated mode or hand swap yet. Turning VR off in the menu shows the game on a large flat screen.
- **Story scenes are on a flat panel.** Cutscenes play on a flat 16:9 panel, mini-games and fishing are not adapted, and there is no positional audio.

## If something goes wrong

- **The game does not start, or Windows says `MSVCP140.dll` or `VCRUNTIME140.dll` is missing.** Install the latest Microsoft Visual C++ Redistributable 2015-2022 (x86), then start the game again.
- **The game stays on the flat window and never enters VR.** Make sure Virtual Desktop is connected and is your active OpenXR runtime before you start the game, then load a save: VR starts at the first field or battle. If it still does not, close the game and try again.
- **The view is off-axis.** Hold the Meta button on the right controller to recenter where you are looking.

## Roadmap

*A direction, not a deadline. These are plans, not promises, with no dates, and the order can change with what testers report.*

| Stage | Theme | What it brings |
|---|---|---|
| **V1 - this alpha (0.1.0-alpha.3)** (Now) | Explore, talk, fight | Stereo exploration, tracked hands and sword; Battles, linked portraits, Link/Swap panels and Touch controls; Dialogue, menus, scenes and results on panels; In-VR settings menu that remembers your choices; Other school leaders' hands; their weapon while you hold A; Enemy HP and damage on each enemy; S-Break wheel on a flat panel |
| **V1.1 - fixes after launch** (Next) | Smoother and clearer | Less tremor while walking and steadier hands while turning; Fixes from early feedback and a controls reference in VR |
| **V2 wave 1 - comfort and settings** (Planned) | Make it yours | More options in the VR settings menu; Snap turn, seated mode, hand swap; Optional third-person exploration camera; Play with a regular gamepad in VR; Fie and the later party members as field leader |
| **V2 wave 2 - battle and controls** (Planned) | Better fights | Status icons attached to each enemy; Item done properly; S-Craft polish and results in 3D |
| **V2 wave 3 - presence and world** (Later) | Be there | Full body for each character; Sword trail that follows your swing, and attack by gesture; Mini-games, fishing and cards; Positional audio |
| **V3 - installer** (Later) | One-click install | A proper installer with backups (the ZIP stays available) |

If support allows, Trails of Cold Steel II, III and IV come after this mod. *(Roadmap reviewed 2026-10-07.)*

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
