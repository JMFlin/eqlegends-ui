# Layout structure

This repository contains game configuration, with no executable code or build step.

`UI_AEROLAMAH_LO1.ini` owns window placement, appearance, visibility, and chat routing. It is a snapshot of Aerocell's UI as saved by the game on November 1, 2026. It retains the Lamah-derived chat setup and the added Pet tab with its five pet-specific filter routes, and it sends your melee and spell criticals to the Hits tab.

`AEROLAMAH_LO1.ini` owns character-level settings. Its `HotButtons` sections, `Socials`, and `SpellLoadouts` come from Aerocell's backup. Socials accompany the buttons because buttons reference those macros. The remaining sections come from Lamah's template.

`eqclient.ini` owns account-wide client settings: video, options, chat colors (`[TextColors]`), filter toggles (`[ChatFilters]`), and key bindings. Copy Layout does not touch it, so it is copied over the game's copy by hand.

Installation copies both template files into the game directory. The game's Copy Layout operation then imports the selected settings into the active character. The templates remain separate from the active character files.

When updating this repository, validate unique INI section names and compare copied files byte-for-byte with the intended source. Keep character backups outside the repository.
