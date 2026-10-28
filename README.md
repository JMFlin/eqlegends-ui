# AEROLAMAH for EverQuest Legends

A personal layout combining LamahHerder's window layout and chat filters with Aerocell's hotbars, macros, and saved spell sets.

## Install

1. Exit EverQuest Legends and back up your character's UI and character INI files.
2. Copy `UI_AEROLAMAH_LO1.ini` and `AEROLAMAH_LO1.ini` into the game directory beside `eqgame.exe`.
3. Start the game and select **Options > Copy Layout > AEROLAMAH**. Enable hotbutton and social copying if those options are offered.
4. Check window positions and hotbuttons for your character and screen size.

The local installation used `C:\Users\Public\Daybreak Game Company\Installed Games\EverQuest Legends`.

## Contents

- `UI_AEROLAMAH_LO1.ini`: Lamah's windows and three chat containers, with Aerocell's hotbar positions, sizes, and visibility.
- `AEROLAMAH_LO1.ini`: Lamah's character-settings baseline with Aerocell's five populated hotbars, socials, and saved spell sets.
- [CONTEXT.md](CONTEXT.md): file boundaries and how the layout was assembled.

Hotbuttons include character-specific item references, abilities, and macros. Keyboard bindings are not included. This is the saved AEROLAMAH template, not a snapshot of later in-game adjustments.

The currency-scrolling change has not been implemented. Custom inventory XML and map packs are not bundled. The game command `/taskoverlay` toggles the task overlay; its hidden state has not been baked into this template.

## Pet chat tab

The combat chat container includes a Pet tab for pet melee messages, rampage/flurry, critical hits, spells, and responses. It uses ChannelMap entries 43, 44, 45, 51, and 52. Some pet spell damage shares the player's direct-damage critical filter; that shared filter stays in its existing tab. Mappings follow the [EverQuest Legends chat filter editor](https://eqlegends.tools/chat-filters/).

## Source and verification

Based on [LamahHerder/EQLegends](https://github.com/LamahHerder/EQLegends), commit `9fb89e7b71b277c6492e049fb5ec16d76a0f7677`. The upstream MIT license is retained in [LICENSE](LICENSE).

Aerocell's settings came from the local backup made on October 28, 2026 at 09:02:07. The merged sections were checked against that backup and all other sections against the Lamah template. In-game appearance has not been independently verified.
