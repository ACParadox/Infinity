# Infinity Army unit-change references

This directory tracks Army/profile changes that materially affect unit selection, profiles, availability, or Fireteams.

## Current scope

Summary changelogs:

- [`N5.2_Army_Changes.md`](N5.2_Army_Changes.md) — October 15, 2025 Army update released alongside rules v5.2.
- [`N5.2_Era_May_2026_Army_Changes.md`](N5.2_Era_May_2026_Army_Changes.md) — May 27, 2026 Mazebreaker Army update, while v5.2 was still the active rules baseline.
- [`N5.3_Army_Changes.md`](N5.3_Army_Changes.md) — September 1, 2026 Army update released with N5.3 / ITS Season 18.

Profile-level appendices:

- [`N5.2_Profile_Diff.md`](N5.2_Profile_Diff.md) — profile/loadout/stat deltas for N5.2 plus the October/November 2025 Army hotfixes.
- [`N5.2_Era_May_2026_Profile_Diff.md`](N5.2_Era_May_2026_Profile_Diff.md) — profile/loadout/stat deltas for Mazebreaker plus the quiet post-Mazebreaker corrections found on the live Army data.
- [`N5.3_Profile_Diff.md`](N5.3_Profile_Diff.md) — N5.3 new-unit/profile matrix, Sāchā consolidation, and small profile/data corrections.

## What “profile-level exhaustive” means here

Within the scoped Army releases, every unit explicitly named by the official changelog, historical snapshot diff, or corroborated post-release hotfix is accounted for. Gameplay-relevant changes are separated from:

- faction/AVA/Fireteam-only changes;
- internal ID/peripheral renumbering;
- duplicated faction copies of the same canonical profile;
- source/editorial fixes with no gameplay effect.

Exact old → new values are recorded where the official notice or pinned historical Army JSON makes them reconstructable. If a publication says only “Options and Costs Review” and an exact semantic delta cannot be isolated safely, the row is retained and marked **UNRESOLVED** rather than guessed.

## Evidence labels

- **OFFICIAL+SNAPSHOT** — official Corvus Belli change and matching historical Army-data delta.
- **SNAPSHOT** — gameplay delta directly observed between pinned historical Army JSON states.
- **OFFICIAL** — explicit Corvus Belli changelog/hotfix, but no independently pinned before/after snapshot for that exact field.
- **CURRENT-DATA** — observed in current/live Army-derived data after an unannounced patch; exact introduction date may be uncertain.
- **COMMUNITY-CROSSCHECK** — community diff/video used only to discover or corroborate; never overrides official/pinned data.
- **UNRESOLVED** — affected profile is known, but the exact old/new semantic field is not safely reconstructable from the retained evidence.

## Sources

Primary/current unit reference:

- [InfinityDB](https://infinitydb.tsudao.com/units?s=v1.u.EwExFAExFQExFgEx)

Official changelogs:

- [Army Update October 2025 - Part 2](https://infinityuniverse.com/en/news/army-update-october-2025-part2)
- [Army Update - May 2026](https://infinityuniverse.com/en/news/army-update-mazebreaker)
- [ITS Season 18 + N5.3 Rules Update](https://infinityuniverse.com/en/news/infinity-rules-update-5-3)

Historical Army data:

- [massayoshi/infinity-army-backup](https://github.com/massayoshi/infinity-army-backup)
- [InfinityDB N5 source/update history](https://github.com/frankysan/InfinityDB/blob/main/docs/n5-source-history.md)
- [InfinityDB N5.3 reconciliation](https://github.com/frankysan/InfinityDB/blob/main/docs/rules-explanation-audit-1.0-n5.3-reconciliation.md)

Community/current-data cross-checks:

- [Infinity: The Classifieds — changelog](https://www.infinitytheclassifieds.com/changelog)
- [Infinity: The Classifieds — Sitrep](https://www.infinitytheclassifieds.com/sitrep)
- [May 2026 community profile changelog PDF](https://www.brueckenkopf-online.com/wp-content/uploads/2026/05/Infinity-Changelog-260526.pdf)
- [Robert Shepherd — Operation Mazebreaker profile analysis](https://www.youtube.com/watch?v=NRRP4Fects8)
- [The Dice Gods War Gaming — May 2026 Army update discussion](https://www.youtube.com/watch?v=L7aAA8_TL2Y)

Community material is discovery/corroboration only.

## Historical snapshot anchors

- pre-N5.2: `cad673d3d9a3538d0c9ad3475336d4dfe5939bc7`
- N5.2: `646187ca89995e7091138c694498a684cb5c4ca3`
- N5.2.1 archive repair: `05384cfce5eac9afc384c88c96a9a8a0431a3050`
- pre-Mazebreaker: `0da30f6692d94b4ed097b2fe60445e6d7249c032`
- Mazebreaker: `9b9c6014c9a80f1f4163e166a44e941443297f95`
- N5.3 post-release snapshot: `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b`

The historical archive is corroborating evidence, not official authority. Preserve conflicts rather than silently choosing a winner.
