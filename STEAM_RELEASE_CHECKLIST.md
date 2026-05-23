# Steam Release Checklist

Use this as the command checklist before building a Steam upload candidate. Local source of truth remains `D:\SteamLibrary\steamapps\common\Call to Arms - Gates of Hell\mods\template`.

## Preflight

- [ ] Confirm `mod.info` name, description, tags, and game version support are correct.
- [ ] Confirm the mod folder boots from the local GoH `mods/template` directory.
- [ ] Confirm no full `resource/` or binary asset tree is being uploaded to this GitHub repo.
- [ ] Confirm `test/old/` remains quarantine/reference content and does not contain live required assets.

## Crash And Boot Checks

- [ ] Boot editor with the mod enabled.
- [ ] Check latest game/editor logs after boot.
- [ ] Spawn-test representative Moonic MDF and MHF units.
- [ ] Record any new crash signature in `KNOWN_ISSUES.md` and as a GitHub issue.

## Gameplay Data Validation

- [ ] Run brace checks on edited `.set`, `.inc`, `.ammo`, `.weapon`, `.def`, and `.mdl` text files.
- [ ] Validate breed inventories: filled weapon, matching ammo, valid special/ID items.
- [ ] Validate weapon/ammo references against `tools/MOONIC_AMMO_FAMILY_MATRIX.md`.
- [ ] Validate forcefields/shields: basic, elite, luck, holy, and Juggernaut dark-red shield.
- [ ] Validate localization coverage for new item, ammo, weapon, and breed IDs.

## Release Content Checks

- [ ] Review `tools/MOONIC_STEAM_UPLOAD_TRIM_AUDIT.md` before moving or deleting anything.
- [ ] Confirm confirmed-keep assets still resolve in game.
- [ ] Confirm candidate-trim assets have zero-reference proof before quarantine.
- [ ] Confirm conquest remains intentionally blank/safe unless a later conquest pass updates it.

## Final Candidate

- [ ] Editor boot succeeds after all release changes.
- [ ] Smoke tests pass for one baseline, specialist, leader, elite/signature role per major regiment group.
- [ ] Update `CHANGELOG.md` with final release notes.
- [ ] Record final known issues and workarounds.
