# Infinity Army unit-change references

This directory tracks Army/profile changes that materially affect unit selection, profiles, availability, or Fireteams.

## Current scope

- [`N5.2_Army_Changes.md`](N5.2_Army_Changes.md) — the October 15, 2025 Army update released alongside rules v5.2.
- [`N5.2_Era_May_2026_Army_Changes.md`](N5.2_Era_May_2026_Army_Changes.md) — the May 27, 2026 Mazebreaker Army update. This happened while v5.2 was still the active rules baseline, but it is **not** part of the October 2025 N5.2 release.
- [`N5.3_Army_Changes.md`](N5.3_Army_Changes.md) — the September 1, 2026 Army update released with N5.3 / ITS Season 18.

## Sources and evidence policy

Primary/current unit reference:

- [InfinityDB](https://infinitydb.tsudao.com/units?s=v1.u.EwExFAExFQExFgEx)

Official changelogs:

- [Army Update October 2025 - Part 2](https://infinityuniverse.com/en/news/army-update-october-2025-part2)
- [Army Update - May 2026](https://infinityuniverse.com/en/news/army-update-mazebreaker)
- [ITS Season 18 + N5.3 Rules Update](https://infinityuniverse.com/en/news/infinity-rules-update-5-3)

Historical Army-data corroboration:

- [massayoshi/infinity-army-backup](https://github.com/massayoshi/infinity-army-backup) — unofficial historical backup of public Army API data, also identified by InfinityDB's own source-history documentation as useful corroborating evidence.
- [InfinityDB N5 source/update history](https://github.com/frankysan/InfinityDB/blob/main/docs/n5-source-history.md)
- [InfinityDB N5.3 reconciliation](https://github.com/frankysan/InfinityDB/blob/main/docs/rules-explanation-audit-1.0-n5.3-reconciliation.md)

### Historical snapshot anchors used

- N5.2 archive commit: `646187ca89995e7091138c694498a684cb5c4ca3` (`army: N5.2`, 2025-10-15).
- N5.2.1 archive commit: `05384cfce5eac9afc384c88c96a9a8a0431a3050` (`army: N5.2.1`, 2025-10-16). The inspected diff is primarily source/peripheral-ID repair, so it is not treated here as a separate gameplay balance pass without a semantic profile delta.
- May 2026 archive commit: `9b9c6014c9a80f1f4163e166a44e941443297f95` (`army: N5 Mazebreaker`, 2026-05-27).
- N5.3 archive commit: `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b` (`army: N5.3 + ITS18`, archived 2026-09-03).

The archive is **corroborating evidence, not official authority**. When an official changelog and a historical snapshot differ, preserve the discrepancy rather than silently choosing one.
