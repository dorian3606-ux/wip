# Known Issues

This file tracks release blockers and risky systems. Use GitHub issues for actionable work; keep deeper implementation notes in the local mod `tools/` folder.

## Active Risk Areas

- **Ammo migration:** Broad all-at-once ammo unification caused instability before rollback. Future ammo work should happen one weapon family at a time and use `tools/MOONIC_AMMO_FAMILY_MATRIX.md` as the rule sheet.
- **Mental/psyker ammo:** Keep `mental_staff.ammo` reserved for actual psyker staff weapons. If a transferable mental trait is added later, test one family first, e.g. `mhf_raider.mental.ammo`, before expanding.
- **Forcefields and shields:** Basic, elite, luck, War Pilgrim holy, and Juggernaut dark-red energy shields need spawn, damage, break, and recharge smoke tests.
- **Localization gaps:** New or renamed weapons, ammo, shields, helmets, and breed IDs need `desc/stuff`, `desc/weapon`, or `desc/ammo` coverage before upload.
- **Conquest visibility:** Conquest purchase files are intentionally not rebuilt yet; verify no parser-unsafe or half-populated conquest entries block visible units.
- **Trim safety:** Do not delete or move live assets until zero-reference proof is recorded in `tools/MOONIC_STEAM_UPLOAD_TRIM_AUDIT.md`.

## Recently Stabilized Notes

- The generated MDF/MHF `mental_staff` ammo overlay was rolled back and the game was reported working again.
- Local docs record a complete Moonic breed rebalance and exact baseline re-ladder across 302 breed files.
- `test/old/` is quarantine/reference content, not active gameplay content.
