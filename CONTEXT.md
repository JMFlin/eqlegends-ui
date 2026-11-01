# Layout structure

This repository contains game configuration, with no executable code or build step.

`UI_AEROLAMAH_LO1.ini` owns window placement, appearance, visibility, and chat routing. It mirrors Aerocell's live `UI_Aerocell_freeport_LO1.ini`. It retains the Lamah-derived chat setup and the added Pet tab with its five pet-specific filter routes, and it sends your melee and spell criticals to the Hits tab.

`AEROLAMAH_LO1.ini` owns character-level settings: hotbars, socials, spell sets, and sound and gameplay options. It mirrors Aerocell's live `Aerocell_freeport_LO1.ini`, which began as Lamah's template with Aerocell's hotbars, socials, and spell sets merged in.

`eqclient.ini` owns account-wide client settings: video, options, chat colors (`[TextColors]`), filter toggles (`[ChatFilters]`), and key bindings. It mirrors the live `eqclient.ini`. Copy Layout does not touch it, so it is copied over the game's copy by hand.

Installation copies both template files into the game directory. The game's Copy Layout operation then imports the selected settings into the active character. The templates remain separate from the active character files.

The repository is a mirror of the live game files. Whenever settings are saved, copy all three live files over their repository counterparts after the game has exited, so the game has written its final state. Do not save only some of them.

When updating this repository, validate unique INI section names and compare copied files byte-for-byte with the intended source. Keep character backups outside the repository.
