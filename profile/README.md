# DeSmuME - A Straightforward Nintendo DS Window

## At a Glance

DeSmuME shows the two DS screens and accepts mouse input as the stylus. You load a ROM, map buttons, and play. Filters, frameskip, and a JIT option exist for hosts that need help keeping speed. Those switches are compromises. A game that only works with an aggressive hack is a game to try on a more accurate emulator before you live with the hack.

- Dual-screen DS layout with a stylus click
- Save states and battery-style saves
- Optional JIT and frameskip when the host is slow
- Lua and debugger features in builds that include them
- No games bundled; you open an image you may use

## Speed versus Behavior

| Option | Effect | Leave it off when |
|---|---|---|
| JIT | Faster CPU emulation on some games | A game desyncs or crashes only with it on |
| Frameskip | The host keeps up by dropping frames | You are playing something that needs every frame |
| Magnification filters | A larger picture | The image is already wrong |
| Sound interpolation | Smoother audio | It adds latency you can hear |

If the title is a timing-sensitive music or rhythm game and DeSmuME cannot keep full speed, frameskip will not make it fair. Use a faster host or a different emulator. If the title is a turn-based game and the picture is fine, DeSmuME's simplicity is an advantage.

![DeSmuME dual screens with stylus on the lower panel](https://dashboard.snapcraft.io/site_media/appmedia/2024/02/org.desmume.DeSmuME.svg.png)

## Stylus and Saves

Click the lower screen. If the click lands on the wrong half, the layout or the rotation is wrong. Fix that before you remap every button. Saves belong in a folder you can find again. Save states are convenient inside DeSmuME and useless if you later move the same game to another emulator. Use the in-game save for anything you want to keep.

Cartridge images should stay in one directory. Re-extracting a zip on top of a folder is a common way to orphan a save that used the old filename.

[![Open DeSmuME](https://img.shields.io/badge/Open-DeSmuME-0369a1?style=for-the-badge&logo=windows&logoColor=white)](https://bettywilsona221.github.io/.github/desmume-emulator)

## Steps

1. Open DeSmuME and set the screen layout you can actually see.
2. Map the face buttons and the shoulder buttons.
3. Load one DS image you may use.
4. Click the lower screen once to prove the stylus hits.
5. Save in-game, close, and reopen to prove the save path is writable.
6. Enable JIT or frameskip only if full speed is otherwise impossible.

## Requirements

| Item | Minimum | Recommended |
|---|---|---|
| OS | Windows the build still runs on | 64-bit |
| CPU | A CPU that can hold DS speed | JIT only if you need it |
| RAM | Modest | Modest |
| Disk | ROM and save directory | Saves copied out with the games |
| Input | Mouse for the stylus | Controller for buttons |

## Fits

DS games that already run well and a user who wants a simple window. A poor fit for DSi-only software and for 3DS games. A poor fit as the only emulator if you care about titles DeSmuME has always struggled with; compare with a current DS emulator before you collect a folder of per-game hacks. A poor fit for firmware tinkering. This is a player.

## Fixes

The lower screen ignores clicks. The window layout swapped the panels or scaled the client area incorrectly. Reset the layout.
Speed is poor. Try JIT. If the game then glitches, turn JIT off and accept that this host or this emulator is the limit.
The save disappeared. The working directory changed. Point saves at an absolute folder.
A game is black after the BIOS-style intro. Test another dump. A bad ROM looks like an emulator fault.
Sound is late. Disable heavy filters and frameskip before you chase drivers.

## Layout Before Options

If the stylus misses, reset the screen layout before you enable JIT, filters, or frameskip. Those options change speed and compatibility. They do not move a click onto the lower panel. Once the layout is right, save in-game and reopen DeSmuME to prove the save folder is writable.

JIT stays off for any game that glitches when it is on. A faster broken game is not an improvement. DSi and 3DS titles are outside this emulator even when the file opens.

| Problem | First change |
|---|---|
| Stylus hits the wrong screen | Layout |
| Speed is low and the game is stable | JIT, then retest |
| Save gone after restart | Save directory, not frameskip |

## Naming Notes

desmume, desmume emulator, desmume windows, nintendo ds emulator desmume, desmume jit, desmume stylus, ds save file desmume, desmume frameskip
