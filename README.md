# Trails of Cold Steel VR

**Same world. A new perspective.** A fan-made VR mod for Trails of Cold Steel on Steam. Explore with tracked hands and weapons, fight from three viewpoints, cast Arts with character poses, and bring the ARCUS and battle menus onto your palm.

> **1.0 - official release.** The official 1.0 feature set. First-person battle remains experimental; known visual and performance issues are listed below. Save often.
> Tested on: Meta Quest 3 with Virtual Desktop; Windows 11, RTX 4080 SUPER.

**Quick start**

- 1.0: stereo exploration, tracked hands and weapons, tabletop battles and experimental first-person combat.
- Requires the Steam game (PC v1.6, English), Virtual Desktop and Visual C++ x86.
- Extract the ZIP beside `ed8.exe`. Keep Steam open; start `tocs-vr\TocsVrPlayer.exe.`
- Touch controls: left stick, A to confirm, B to go back. Hold the right Meta button to recenter.

[Website](https://www.trailsvr.pro) - [Releases](https://github.com/petonexus/tocs-vr-releases/releases) - [Nexus Mods](https://www.nexusmods.com/thelegendofheroestrailsofcoldsteel/mods/6) - [Gameplay showcase](https://youtu.be/E8FdEB3rqRY) - [Support on Ko-fi](https://ko-fi.com/petonexus)

## What works today

- **First-person exploration.** Explore Thors, Trista and the field in stereo VR with head tracking, leaning, a visible body, tracked hands and fingers, and smooth or step turning.
- **Hands and weapons.** Hold the right grip to draw your leader's weapon. School leaders through chapter 3 have their own hands and weapons, including Fie's two weapons. A swing can trigger an attack; this is not collision-based combat.
- **Three ways to battle.** Use the original third-person camera, a tabletop miniature, or experimental first-person battle. The game keeps its turn-based rules; switch the view in VR settings or in the Touch launcher options.
- **Tabletop battles.** Turn and tilt the miniature with the right stick. Optional Enemy HP in miniature shows the selected enemy's HP below its feet; it starts off and can be toggled in VR settings.
- **ARCUS and Arts on your palm.** Put the command wheel, targets and Arts/Crafts lists on your left palm with Wrist only. Choose with the stick and A. A character pose can confirm a selected Art, with a visual guide and haptic feedback; A remains available.
- **Experimental first-person combat.** Walk while choosing an Attack target, select with the stick and confirm with A. Rean and Jusis can also confirm with a grip-held swing. The target HP bar follows the enemy you look at or attack.
- **Adjustable battle panels.** Move the gold-framed panel, change its distance and size, and park it or let it follow your head. Brightness and opacity are available in settings.ini. Choices survive updates.
- **Menus, dialogue and story.** Read dialogue and shops on a floating panel. Put the camp menu on your wrist, in front or following your gaze. Equipment, Orbment, Item, Link and Swap remain usable; story scenes and results use an in-headset screen.
- **Map, interaction and comfort.** Raise your left wrist to see the minimap, use the field map and Quick Navigation, and find talkable NPCs through a small gold marker. Saved immersion profiles, turning, scale and camera options live in the VR menu.
- **Player launcher and gamepad.** Choose Touch or a native gamepad, the x64 presenter (on by default), the PC eye mirror and an FPS preset before playing. Touch also offers immersion, battle view and a VR settings page with explanations and Save without starting the game. Gamepad uses third-person views and has no Touch gestures or VR menu.
- **Recording and optional OFXR.** Show a smoothed left-eye view in the PC window for recording. OFXR Bridge is an optional external tool: the launcher reports its status, while you configure OFXR and Virtual Desktop separately. It is not bundled.

## Downloads

Download **tocs-vr-1.0.0-d68b4512-player-db88cc7e.zip** from the [latest release](https://github.com/petonexus/tocs-vr-releases/releases).

SHA-256: `7cc8e7d607b24de0d0b68f7452c74daaaacce06bab5edba8c460f6997571b7b6`

**New in 1.0.0**

- Official 1.0: stereo exploration, tracked hands and weapons, and third-person, miniature and experimental first-person battles.
- Palm ARCUS, Arts by character pose, wrist lists, adjustable gold panels, wrist minimap and talk markers.
- Battle fixes for Item, cancelled Arts/Crafts, target crystals and the command wheel; animated walking while choosing an Attack. Added late and lightly tested, so please report what you see: the enemy Analysis window on a flat screen, enemy status icons beside the HP bar, and game controller choice and orbit in the miniature battle.
- Optional enemy HP in the miniature, off by default. Saved comfort, camera and panel settings, with a launcher VR settings page, explanations and Save without starting.
- Cold Steel launcher with Touch/gamepad, x64 by default, FPS presets and a smoothed PC eye mirror. Updated stereo rendering; game 60 FPS, VD 120 Hz and optional OFXR 2x were tested together. OFXR is a separate download.
- One ZIP with the launcher and x64 components; updates preserve player settings. Known issues and the 1.1 roadmap are listed below.

## Requirements

- **The game.** Trails of Cold Steel on Steam, PC version 1.6, English (`ed8.exe`).
- **VR.** A headset with Virtual Desktop as the active OpenXR runtime. Tested with a Meta Quest 3 and Touch controllers.
- **Visual C++.** Microsoft Visual C++ Redistributable 2015-2022 (x86). Without it the game does not start.

## Install

1. Close the game and open the folder that contains `ed8.exe` (Steam: right-click the game > Manage > Browse local files).
2. Extract everything from the ZIP into that folder, keeping its folders. Say yes to replacing `DINPUT8.dll` (SenPatcher is included; back up yours if you may want it back).

Updates replace `vr\settings.ini.default`, not settings.ini or saves.

**Verify a download.** Compare the SHA-256 of the ZIP (Get-FileHash <zip> in PowerShell) with the one on the release page.

## First launch and how to play

1. Connect Virtual Desktop and keep Steam open. Start `tocs-vr\TocsVrPlayer.exe`; x64 is selected by default. Use keyboard or mouse to load a save from the flat title screen.
2. VR starts in the field or battle. Steam direct uses the classic presenter.

- Look ahead at startup; hold the right Meta button to recenter. For step turning, open VR settings.
- Gamepad: choose Game controller in the launcher; L3+R3 recenters. Third person only, no Touch gestures or VR menu. Choose Touch controllers to return.
- Touch: after the first VR run, use VR settings for camera, comfort and panel adjustments with help. Save keeps the launcher open.
- OFXR is optional and not bundled: https://github.com/tig3rmast3r/OFXR-Bridge. Start it first, keep x64 selected and turn Virtual Desktop SSW off.
- FPS presets: Recommended = game 60, VD 120 Hz, optional OFXR 2x; Battery saver = 45, VD 90 Hz, OFXR 2x; Less powerful PC = 30, VD 90 Hz, OFXR 3x (ghosting). Set VD and OFXR yourself. The launcher backs up settings.xml; these are targets, not guaranteed FPS.
- Panel appearance: copy vr\settings.ini.default to vr\settings.ini only if absent. Under [Video], panel_brightness is 50-150 and panel_opacity 40-100; both default to 100.

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
| **Right hand (menu open)** | Point and pull the trigger. *(experimental)* |

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

Use the VR menu for camera and panel options. Gamepad uses the game's native controls.

## Known issues

- **Brief panel flashes.** New battle panels or lists can flash in both eyes for about two frames. A fix is planned.
- **Uneven motion.** Some scenes show walking or turning judder, hand shake or FPS drops, especially with frame generation. 1.1 targets measured performance and pacing improvements.
- **Enemy Analysis and light halos.** Enemy Analysis now shows on a flat screen, but it was checked on one route only (first person, View Specifics); other ways to open it and the miniature view may still omit details. Some light halos can be clipped after pausing. The halos are on the backlog.
- **First-person battle is experimental.** Swing confirms a selected Attack, not physical damage. Weapon-specific gestures are unfinished. Miniature native damage labels can face the actor. Fie's Art pose has one calibration sample.
- **Keep the default outfits.** We recommend keeping the characters' default outfits. Some other outfits and costumes may not show correctly in VR, and not every scene and outfit could be tested. If one looks wrong, please report the outfit and the scene.
- **Gamepad uses third person.** No Touch gestures or VR menu. Visual panel settings are read at startup. Choosing a target and orbiting the miniature battle with the game controller is new and has not been tried with a physical controller. The launcher VR settings page currently requires Touch.
- **Flat screens and tested setup.** Title, loading menus, story scenes and results use a screen. Tested on Quest 3 / Virtual Desktop at 3440x1440; the newest changes have no fresh 1920x1080 check.
- **Future features.** No seated mode, hand swap, positional audio or native 90 FPS. Later leaders and minigames need more work. Some camera and world-size settings need a restart.

## If something goes wrong

- **The game does not start, or `MSVCP140.dll` or `VCRUNTIME140.dll` is missing.** Install the latest Microsoft Visual C++ Redistributable 2015-2022 (x86).
- **The game never enters VR.** Connect Virtual Desktop and make it the active OpenXR runtime before you start the game, then load a save. VR starts at the first field or battle. If not, restart the game.
- **The view is off-axis.** Hold the Meta button on the right controller to recenter.

## Roadmap

*Planned priorities, not delivery dates. Fixes can ship separately as 1.0.x updates.*

| Stage | Theme | What it brings |
|---|---|---|
| **1.0 - official launch** (Now) | Explore, talk and fight in VR | Stereo exploration; three battle views; tracked hands and weapons; Palm ARCUS, Arts poses, menus and player launcher |
| **1.0.x - maintenance** (Next) | Fix release regressions | Startup, compatibility and gameplay fixes from reproducible reports |
| **1.1 - first-person battle and scenes** (Planned) | Fight and watch the story from your own eyes | Natural walking and your own body in first-person battle; Weapon attack gestures; First-person story scenes; Better performance and visuals |
| **Later - comfort and coverage** (Later) | Broader ways to play | Seated and left-handed play, more leaders, minigames, panel themes; Positional audio and an installer with backups |

Cold Steel II, III and IV are longer-term possibilities, depending on support. *(Roadmap reviewed 2026-10-29.)*

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
