# Trails of Cold Steel VR

**Same world. A new perspective.** Free VR mod for Trails of Cold Steel: tracked hands, battles and palm menus.

> **1.2 - official release.** 1.2 adds Alisa's bow, smoother edges and new menus. DLSS, first-person combat and features awaiting broader checks are experimental. Save often.
> Tested on: Meta Quest 3 with Virtual Desktop; Windows 11, RTX 4080 SUPER.

**Quick start**

- 1.2 adds Alisa's bow, smoother edges and new menus. DLSS and first-person combat are experimental.
- Requires the Steam game (PC v1.6, English), Virtual Desktop and Visual C++ x86.
- Extract the ZIP beside `ed8.exe`. Keep Steam open; start `tocs-vr\TocsVrPlayer.exe.`
- Touch controls: left stick, A to confirm, B to go back. Hold the right Meta button to recenter.

[Website](https://www.trailsvr.pro) - [Releases](https://github.com/petonexus/tocs-vr-releases/releases) - [Nexus Mods](https://www.nexusmods.com/thelegendofheroestrailsofcoldsteel/mods/6) - [Launch video](https://youtu.be/BCXjr3M0slI) - [Support on Ko-fi](https://ko-fi.com/petonexus)

## What works today

- **First-person exploration.** Explore Thors, Trista and the field in stereo VR with head tracking, leaning, a visible body, tracked hands and fingers, and smooth or step turning.
- **Hands and weapons.** Hold the right grip to draw your leader's weapon. School leaders through chapter 3 have their own hands and weapons, including Fie's two weapons. A swing can trigger an attack; this is not collision-based combat.
- **Alisa's exploration bow.** Hold the left grip for the bow. Close the right grip near it, pull back until the second haptic cue and release the right grip to shoot. Release the left grip to cancel. The native arrow follows horizontal aim; the first bow draw can trigger one preparation attack. Gaius can attack with a forward lance thrust.
- **Three ways to battle.** Use the original third-person camera, a tabletop miniature, or experimental first-person battle. The game keeps its turn-based rules; switch the view in VR settings or in the Touch launcher options.
- **Tabletop battles.** Turn and tilt the miniature with the right stick, or turn and scale the table with both hands. Enemy HP in miniature shows the selected enemy's HP below its feet in place of the game's own enemy gauges and markers; it starts on and can be turned off in VR settings.
- **ARCUS and Arts on your palm.** Put the command wheel, targets and Arts/Crafts lists on your left palm with Wrist only. Choose with the stick and A. A character pose can confirm a selected Art, with a visual guide and haptic feedback; A remains available. Battle results show on your palm too.
- **Experimental first-person combat.** See your whole body and walk with the game's own steps while choosing an Attack target; select with the stick or point your open hand at an enemy, and confirm with A. Rean and Jusis can also confirm with a grip-held swing, and Emma, Fie and Gaius with a strike of their own weapon type. The target HP bar follows the enemy you look at or attack.
- **Adjustable battle panels.** Move the gold-framed panel, change its distance and size, and park it or let it follow your head. Brightness and opacity are available in settings.ini. Choices survive updates.
- **Menus, dialogue and story.** Read dialogue and shops on a floating panel. Put the camp menu on your wrist, in front or following your gaze. Equipment, Orbment, Item, Link and Swap remain usable; in first-person play, story scenes play through the game's camera in 3D (the default), Rean's eyes (ultra-immersive, experimental) or an in-headset screen (VR menu, Scenes); third person and the gamepad mode use the screen.
- **Map, interaction and comfort.** Raise your left wrist to see the minimap, use the field map and Quick Navigation, and find talkable NPCs through a small gold marker. Saved immersion profiles, turning, scale and camera options live in the VR menu.
- **Player launcher and gamepad.** Choose Touch or a native gamepad, the x64 presenter (on by default), the PC eye mirror and an FPS preset before playing. Touch also offers immersion, battle view and a VR settings page with explanations and Save without starting the game. Gamepad uses third-person views and has no Touch gestures or VR menu. VR settings now use four themed tabs with large cards and icons; the new in-headset layout is experimental.
- **Recording and optional OFXR.** Show a smoothed left-eye view in the PC window for recording. OFXR Bridge is an optional external tool: the launcher reports its status, while you configure OFXR and Virtual Desktop separately. It is not bundled.
- **Experimental DLSS.** Choose Sharper picture in the launcher for optional NVIDIA DLSS, off by default. Requires the x64 presenter and a compatible NVIDIA GPU. The latest test improved clarity and removed the observed black flashes, but character trails and occasional world smearing remain. DLSS with OFXR has not passed final validation.

## Downloads

Download **tocs-vr-1.2.0.zip** from the [latest release](https://github.com/petonexus/tocs-vr-releases/releases).

SHA-256: `47fc4edf2623bd9114278c67a300105801fc31a662ec0f89e0022d13b9036a5a`

**New in 1.2.0**

- Includes the 1.1 advances: full-body first-person battle (experimental), native walking, open-hand target selection and weapon-specific strikes, including Gaius's thrust.
- Story scenes use the game's 3D camera by default; Scenes offers a flat comfort view or experimental Rean's eyes. Battle results stay in 3D with pages on the left palm.
- Miniature battles support two-hand turn/scale and smaller enemy HP bars, on by default. Smoother edges, steadier hand/panel layers, corrected water, turn percentage and fewer flashing lists/repeated frames.
- Alisa's bow: left-hand hold and horizontal aim, native arrow in the right hand, right-grip draw/release, and distinct nock/draw/cancel haptics.
- Redesigned launcher and four VR settings tabs with cards, icons, explanations and Save. The new in-headset layout and hand-ray interaction are experimental.
- Optional experimental DLSS, Off by default, includes the NVIDIA runtime and latest history/timing fixes. Trails and world smearing remain; DLSS + external OFXR can be unstable. No FPS gain is promised.

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

- Look ahead at startup. Hold right Meta to recenter; VR settings offers step turning.
- Game controller: third person, L3+R3 recenter; no Touch gestures or VR menu.
- DLSS: experimental, Off by default. Sharper picture needs x64 and a compatible NVIDIA GPU; failed initialization keeps the normal image. No DLAA.
- Optional external OFXR: https://github.com/tig3rmast3r/OFXR-Bridge. Start it first; use x64 and turn VD SSW off. DLSS + OFXR remains experimental, including normal 2x with Hybrid OFF.
- FPS targets: Recommended 60 / VD 120 Hz / optional OFXR 2x; Battery saver 45 / 90 Hz / 2x; Less powerful PC 30 / 90 Hz / 3x (ghosting). Set VD/OFXR yourself. The launcher backs up settings.xml.
- Panel appearance: copy vr\settings.ini.default to vr\settings.ini only if absent. Under [Video], panel_brightness is 50-150 and panel_opacity 40-100; both default to 100.

## Controls

Right hand leads; Alisa's bow uses the left. Experimental = needs more checks.

#### Exploration

| Control | What it does |
|---|---|
| **Head** | Look around and lean in. |
| **Left stick** | Walk; push further to run. |
| **Right stick (left / right)** | Turn. |
| **A** | Confirm, talk, interact, attack. Hold to show the weapon. |
| **Right grip (hold)** | Hold the weapon; swing your arm to attack. |
| **Alisa: left grip / right grip** | Hold left grip. Right grip near bow: nock, pull, release to fire. Left release cancels. Horizontal aim. |
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

- **DLSS and DLSS with OFXR are experimental.** Camera turns/sideways steps can leave trails and world smearing. The last DLSS-only test removed black flashes; DLSS+OFXR remains unvalidated after unstable earlier tests. Disable DLSS if uncomfortable.
- **Experimental coverage.** New VR menu/ray, F2 capture, gamepad target/orbit and other Analysis routes await broader checks, as do enemy icons, later characters and scenes.
- **Uneven motion.** Walking/turning judder, hand shake and FPS drops remain, especially with frame generation. Performance work continues.
- **Enemy Analysis and light halos.** Analysis was checked only in first person via View Specifics; other routes and miniature view may omit details. Some light halos can be clipped after pausing.
- **First-person battle is experimental.** Swing confirms Attack, not physical damage. Strikes lack full character coverage; Fie's Art has one calibration. With miniature HP off, game labels can face the actor.
- **Keep the default outfits.** Use default outfits. Other costumes may show incorrectly; report the outfit and scene if affected.
- **Gamepad uses third person.** No Touch gestures or VR menu. Panel settings apply at startup; target/orbit awaits a physical-controller check. Launcher VR settings needs Touch.
- **Flat screens and tested setup.** Title/loading are flat; results use 3D and wrist pages. Scenes options apply with first-person Touch; other modes use a screen. Tested: Quest 3 / VD, 3440x1440; no fresh 1920x1080 check.
- **Future features.** No seated mode, hand swap, positional audio or native 90 FPS. Later leaders and minigames need more work. Some camera and world-size settings need a restart.

## If something goes wrong

- **The game does not start, or `MSVCP140.dll` or `VCRUNTIME140.dll` is missing.** Install the latest Microsoft Visual C++ Redistributable 2015-2022 (x86).
- **The game never enters VR.** Set Virtual Desktop as the active OpenXR runtime, then load a save. VR begins in the field/battle. Restart if needed.
- **The view is off-axis.** Hold the Meta button on the right controller to recenter.

## Roadmap

*Planned priorities, not delivery dates. Fixes can ship separately as 1.2.x updates.*

| Stage | Theme | What it brings |
|---|---|---|
| **1.2 - first-person battle and scenes** (Now) | Fight and watch the story from your own eyes | Experimental first-person battle, 3D scenes/results, Alisa bow, smoother edges, new menus and optional DLSS |
| **1.2.x - maintenance** (Next) | Fix release regressions | Startup, compatibility and gameplay fixes from reproducible reports |
| **Next - performance and image** (Planned) | Polish what 1.2 left open | Reduce DLSS trails/OFXR instability; broader headset checks; investigate pacing, foveated DLSS and rendering cost |
| **Later - comfort and coverage** (Later) | Broader ways to play | Seated/left-handed play, more leaders/minigames, panel themes, positional audio and an installer |

Cold Steel II, III and IV are longer-term possibilities, depending on support. *(Roadmap reviewed 2026-11-03.)*

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

[Watch the 1.0 launch video](https://youtu.be/BCXjr3M0slI).

## Support Development

Made independently in spare time. Ko-fi donations are optional and are not a pre-order or a promise of a release date.

[![Support me on Ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/petonexus)

## Disclaimer

Unofficial fan mod. No Falcom/NVIDIA endorsement. Trails IP belongs to its owners. Requires your own game; no game files. NVIDIA components have separate licenses.

## Licenses

Each release has a versioned mod ZIP, a SHA-256 checksum, installation instructions, release notes and known issues. The ZIP contains the combined SenPatcher/VR loader, the Khronos OpenXR loader, the mod's configuration, a hash manifest, and the applicable third-party license texts. A separate SenPatcher download is not required.

The original VR mod portions are Copyright © 2026 petonexus; third-party components retain their own licenses. See [LICENSE.txt](tocs-vr/LICENSE.txt) and [THIRD_PARTY_NOTICES.txt](tocs-vr/THIRD_PARTY_NOTICES.txt). Release ZIPs include these files and the license texts under `tocs-vr/licenses/`.
