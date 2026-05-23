# Trim Audit Summary

Summary of the local `tools/MOONIC_STEAM_UPLOAD_TRIM_AUDIT.md`. The full ledger stays local with exact path details.

## Confirmed Keep

- Moonic M43 helmet variants, especially `moonic_ger_stalhelm_m43_dirt_wire` as the Cronus basic helmet.
- `mdf_mgun_belt.ammo` and `mhf_mgun_belt.ammo` as active MDF/MHF heavy MG belt ammo.
- `mgun_rus_belt_ammo` compatibility entity for old belt references.
- Conquest blank shell files until the conquest tree is intentionally rebuilt.

## Candidate Trim Areas

- Old duplicate ammo clones after shared ammo migration stabilizes.
- Unused WIP helmets and skins after reference audits.
- Retired conquest aliases after conquest rebuild decisions.

## Already Quarantined

The local `test/old/` folder holds reversible cleanup/reference content, including disabled overrides, extraction scratch workspaces, old backup folders, root scratch files, and the `3510016454` armor-hitbox reference pack.

## Do Not Move Yet

- Anything referenced by breed inventory, weapon filling, entity extenders, localization, or saved editor compositions.
- Any entity used as a parent/template by another `.def` or `.mdl`.
- Any shared texture used by helmets, uniforms, weapons, or vehicles.
- Any special, forcefield, or ID item until it has been spawn-tested.

## Required Proof Before Deleting

Search `resource/set`, `resource/entity`, `localizations/default`, `map`, and `tools`; record the exact search term and result count in the local trim audit; move to quarantine before deletion; boot editor and run representative spawn tests.
