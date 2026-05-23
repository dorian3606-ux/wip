# Moonic Steam Release Prep

This repository is a lightweight release-control hub for **Moon's Heretics Unit Pack**, a WIP Gates of Hell / Indomitus submod.

The actual mod source stays local in:

```text
D:\SteamLibrary\steamapps\common\Call to Arms - Gates of Hell\mods\template
```

This repo intentionally stores docs, checklists, known issues, and release notes only. It does **not** mirror the full `resource/`, `localizations/`, model, texture, or binary asset tree.

## Current Release Posture

- Local mod footprint is about 2.5 GB and should not be pushed here without Git LFS planning.
- Breed rebalance and exact baseline re-ladder are documented locally in `tools/MOONIC_FULL_BREED_BALANCE_AUDIT.md`.
- Ammo family rules are documented locally in `tools/MOONIC_AMMO_FAMILY_MATRIX.md`.
- Steam trim/quarantine status is documented locally in `tools/MOONIC_STEAM_UPLOAD_TRIM_AUDIT.md`.
- Local files remain the source of truth until a Steam upload candidate is built.

## Docs In This Repo

- `STEAM_RELEASE_CHECKLIST.md`: release readiness checklist.
- `KNOWN_ISSUES.md`: active risk areas and test targets.
- `CHANGELOG.md`: high-level release notes.
- `TRIM_AUDIT_SUMMARY.md`: summary of current trim/quarantine posture.

## Working Rule

Use GitHub issues as the command board. Keep implementation in the local mod folder, then record test results and release decisions here.
