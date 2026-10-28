# Layout structure

This repository contains game configuration, with no executable code or build step.

`UI_AEROLAMAH_LO1.ini` owns window placement, appearance, visibility, and chat routing. All `HotButtonWnd` sections come from Aerocell's backup; the remaining sections come from Lamah's template, except ChatManager, which adds the Pet tab and routes pet-specific filters to it.

`AEROLAMAH_LO1.ini` owns character-level settings. Its `HotButtons` sections, `Socials`, and `SpellLoadouts` come from Aerocell's backup. Socials accompany the buttons because buttons reference those macros. The remaining sections come from Lamah's template.

Installation copies both files into the game directory. The game's Copy Layout operation then imports the selected settings into the active character. The templates remain separate from the active character files.

When updating this repository, validate unique INI section names and compare copied files byte-for-byte with the intended source. Keep character backups outside the repository.
