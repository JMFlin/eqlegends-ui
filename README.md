# AEROLAMAH for EverQuest Legends

A personal layout combining LamahHerder's window layout and chat filters with Aerocell's hotbars, macros, and saved spell sets.

## Install

1. Exit EverQuest Legends and back up your character's UI and character INI files.
2. Copy `UI_AEROLAMAH_LO1.ini` and `AEROLAMAH_LO1.ini` into the game directory beside `eqgame.exe`.
3. Start the game and select **Options > Copy Layout > AEROLAMAH**. Enable hotbutton and social copying if those options are offered.
4. Check window positions and hotbuttons for your character and screen size.
5. For client options, chat colors, filter toggles, and key bindings, exit the game and copy `eqclient.ini` over the one in the game directory. Copy Layout does not import these account-wide settings.

The local installation used `C:\Users\Public\Daybreak Game Company\Installed Games\EverQuest Legends`.

## Contents

- `UI_AEROLAMAH_LO1.ini`: Aerocell's saved window positions, sizes, visibility, and three chat containers, including the Pet tab. Saved by the running game on November 1, 2026 at 14:56.
- `AEROLAMAH_LO1.ini`: Lamah's character-settings baseline with Aerocell's five populated hotbars, socials, and saved spell sets.
- `eqclient.ini`: account-wide client settings, including video, options, chat colors, chat filters, and key bindings. Saved when the game exited on November 1, 2026 at 21:17.
- [CONTEXT.md](CONTEXT.md): file boundaries and how the layout was assembled.

Hotbuttons include character-specific item references, abilities, and macros. The UI template includes the in-game window adjustments saved on November 1, 2026. The character-settings file retains the earlier hotbar, macro, and spell-set snapshot.

The currency-scrolling change has not been implemented. Custom inventory XML and map packs are not bundled. The game command `/taskoverlay` toggles the task overlay.

## Pet chat tab

The combat chat container includes a Pet tab for pet melee messages, rampage/flurry, critical hits, spells, and responses. It uses ChannelMap entries 43, 44, 45, 51, and 52. Some pet spell damage shares the player's direct-damage critical filter; that shared filter stays in its existing tab. Mappings follow the [EverQuest Legends chat filter editor](https://eqlegends.tools/chat-filters/).

## Critical hits

Your melee criticals (ChannelMap 30) and spell criticals (ChannelMap 38) both go to the Hits tab. The client prints a critical as a normal damage line ending in `(Critical)`. The color list calls them **Your Hits (Critical)** and **Direct Damage (Your Critical Hits)**, stored as `User_46` and `User_47` in `[TextColors]`.

## Source and verification

Based on [LamahHerder/EQLegends](https://github.com/LamahHerder/EQLegends), commit `9fb89e7b71b277c6492e049fb5ec16d76a0f7677`. The upstream MIT license is retained in [LICENSE](LICENSE).

Aerocell's settings came from the local backup made on October 28, 2026 at 09:02:07. The original merge was checked against that backup and the Lamah template. The UI file was subsequently replaced with Aerocell's saved UI after the user finished arranging windows. Its hash matches that saved file, and the Pet tab and its five filter routes were checked. In-game appearance was approved by the user; it has not been independently inspected.
