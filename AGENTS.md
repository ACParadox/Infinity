# Repository Agent Guidance

## Source of truth

- Treat the latest committed `main` branch of this repository as authoritative for project material.
- Before changing project files, read the specific relevant files first and preserve existing decisions unless the requested change explicitly supersedes them.
- For current Infinity rules, Army profiles, Fireteams, availability, points, SWC, or recent balance changes, verify against current external data rather than relying on model memory.

## Infinity Army and InfinityDB data

Use structured data whenever possible instead of reconstructing Army information manually from prose or screenshots.

### Corvus Belli Infinity Army API

The official Army API is available under:

- `https://api.corvusbelli.com/army/infinity/en/metadata`
- Unit/army documents are exposed through the same `https://api.corvusbelli.com/army` API family.

Direct requests may return `403` unless made with browser-like request headers. InfinityDB's downloader is a useful reference implementation; it sends headers such as `Origin: https://infinityuniverse.com`, an Infinity Universe `Referer`, and a normal browser `User-Agent`.

Prefer the official Army API when direct current-source verification is useful, but do not spend time reverse-engineering access if InfinityDB already exposes the same source data in a normalized form.

### InfinityDB

Primary references:

- Site: `https://infinitydb.tsudao.com/`
- Source: `https://github.com/frankysan/InfinityDB`

InfinityDB ingests Infinity Army data and normalizes units, profiles, loadouts, army membership, and Fireteam relationships. It is the preferred structured interface for analysis when available.

For Fireteams, InfinityDB exposes application API endpoints equivalent to:

- `GET /api/fireteams` — list armies/sectorials with Fireteam data.
- `GET /api/fireteams?army_id=<army>` — retrieve the selected army's Fireteam chart.

Fireteam data can include:

- Fireteam type(s), e.g. Core, Haris, Duo, or named formations.
- Legal members.
- Required members and minimum/maximum counts.
- Wildcard status and Wildcard members.
- `Counts as` / equivalence labels.
- FTO markers and profile/loadout restrictions.
- Army-specific notes, observations, and chart limits.

When doing list-building or modular-block analysis, use the current Fireteam data rather than assuming legality from general knowledge.

## Historical changes

For before/after unit or Army comparisons, use historical Army snapshots rather than attempting to infer an old profile from the current database.

Useful historical source:

- `https://github.com/massayoshi/infinity-army-backup`

Use pinned dated/committed snapshots to calculate semantic profile diffs. Distinguish actual gameplay changes from source churn such as IDs, ordering, metadata, or mirrored faction copies.

For change documentation, separate evidence types clearly:

1. Official Corvus Belli changelog/prose.
2. Official current Army/API data.
3. Historical Army snapshot diff.
4. InfinityDB normalization/reconciliation.
5. Community or video analysis.

Do not present a reconstructed snapshot delta as though Corvus Belli explicitly documented the exact change in prose.

## Preferred authority order

For current Army/list-building work, use approximately:

1. Current Corvus Belli rules, FAQ, Army data, and official update notices.
2. Current InfinityDB normalized Army/Fireteam data, reconciled to the official source when needed.
3. Historical Army snapshots for before/after comparisons.
4. Reliable community analysis for discovery, interpretation, or undocumented hotfix detection; verify against structured data whenever possible.

For Fireteams specifically, use InfinityDB's current structured Fireteam chart first, then verify unusual or ambiguous cases against current Corvus Belli material.
