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

[Website](https://www.trailsvr.pro) - [Releases](https://github.com/petonexus/tocs-vr-releases/releases) - [Gameplay showcase](https://youtu.be/E8FdEB3rqRY) - [Support on Ko-fi](https://ko-fi.com/petonexus)

## What works today

- **Real stereo VR.** Stereo views with head tracking: look around and lean into the scene.
- **First-person exploration.** Explore from Rean's viewpoint with free movement and smooth turning. Y switches the field leader.
- **Tracked hands and sword.** Tracked hands, the game's katana while holding A, and the native slash effect.
- **Battles in VR.** The original battle camera with head tracking, a floating HUD and linked portraits. Link, Swap and Link Attack open on a flat panel with the battle around it.
- **Menus, dialogue and scenes.** Read dialogue, shops and menus on a panel. Story scenes use a 16:9 screen; battle results use the full game screen.
- **Field map and HUD.** Left trigger opens the field map. Hold X to show the field HUD.

## Downloads

Download **tocs-vr-0.1.0-alpha.2-d17d2c8e.zip** from the [latest release](https://github.com/petonexus/tocs-vr-releases/releases).

SHA-256: `9d7c9e46d6e3ff546ab1e0b9e250bfaf8c42cd40eddaef4e0bbc580dae58ee54`

**New in 0.1.0-alpha.2**

- Smoother turning with the right stick: much less drag while you turn.
- 16:9 resolutions such as 1920x1080: story scenes and the battle HUD keep their proportions.

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
| **A** | Confirm, talk, interact, attack. The katana is in your hand only while you hold A. |
| **B** | Cancel / back (also closes the map). |
| **Left menu button** | Camp menu. |
| **Left trigger** | Field map. |
| **X (hold, left)** | Show the field HUD while held. |
| **Y (click, left)** | Switch the field leader. |

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
- **Tested at 3440x1440 and 1920x1080.** The mod has been tested with the game at 3440x1440 (21:9) and 1920x1080 (16:9). At 1920x1080 characters look less sharp unless they are close.
- **Tremor while walking, shaky hands while turning.** Walking can look less smooth than head movement, with some tremor or flicker. Turning with the right stick has much less drag now, but your hands may shake while you turn. Smoothing is the first thing planned for V1.1.
- **Enemy HP and damage numbers are on the battle HUD.** They float on the HUD panel, not above each enemy, and some may look out of place.
- **Some battle visual glitches.** A stray CP/EP gauge can appear after some turn bonuses. S-Craft camera cuts may feel abrupt, and some light halos look clipped after pausing.
- **The game may close by itself.** After some long sessions the game has closed on its own. Save often.
- **Hands and sword use Rean's setup.** Y can switch the field leader, but character-specific hands and weapons are not adapted yet. Rean is the reference setup.
- **No settings menu yet.** No in-VR settings, snap turn, seated mode or hand swap.
- **Story scenes are on a flat panel.** Cutscenes play on a flat 16:9 panel, mini-games and fishing are not adapted, and there is no positional audio.

## If something goes wrong

- **The game does not start, or Windows says `MSVCP140.dll` or `VCRUNTIME140.dll` is missing.** Install the latest Microsoft Visual C++ Redistributable 2015-2022 (x86), then start the game again.
- **The game stays on the flat window and never enters VR.** Make sure Virtual Desktop is connected and is your active OpenXR runtime before you start the game, then load a save: VR starts at the first field or battle. If it still does not, close the game and try again.
- **The view is off-axis.** Hold the Meta button on the right controller to recenter where you are looking.

## Roadmap

*A direction, not a deadline. These are plans, not promises, with no dates, and the order can change with what testers report.*

| Stage | Theme | What it brings |
|---|---|---|
| **V1 - this alpha** (Now) | Explore, talk, fight | Stereo exploration, tracked hands and sword; Battles, linked portraits, Link/Swap panels and Touch controls; Dialogue, menus, scenes and results on panels |
| **V1.1 - fixes after launch** (Next) | Smoother and clearer | Less tremor and drag while moving; S-Craft selection on a flat panel with the battle around it; Fixes from early feedback and a controls reference in VR |
| **V2 wave 1 - comfort and settings** (Planned) | Make it yours | In-VR settings menu that remembers your choices; Snap turn, seated mode, hand swap; Optional third-person exploration camera; Play with a regular gamepad in VR; Other party members as field leader |
| **V2 wave 2 - battle and controls** (Planned) | Better fights | Choose the battle camera: locked or following; HP and status attached to each enemy; Item done properly; S-Craft polish and results in 3D |
| **V2 wave 3 - presence and world** (Later) | Be there | Full body, and hands and weapon for each character; Sword trail and attack by gesture; Mini-games, fishing and cards; Positional audio |
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
