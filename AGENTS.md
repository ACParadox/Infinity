# Repository Agent Guidance

## Source of truth

- Treat the latest committed `main` branch of this repository as authoritative for project material.
- Before changing project files, read the specific relevant files first and preserve existing decisions unless the requested change explicitly supersedes them.
- Do not rely on model memory for exact Infinity rules, profiles, points, SWC, AVA, or Fireteam legality when repository reference data exists.

## Local-reference-first policy

For ordinary questions about a sectorial, its units, profiles, points/SWC, availability, or Fireteam access, **use the repository reference files first instead of searching the web or querying live APIs**.

Sectorial reference format:

- Design/schema: `sectorials/REFERENCE_DESIGN.md`
- Sectorial files: `sectorials/<parent-faction>/<sectorial-slug>.md`
- Index, when present: `sectorials/INDEX.md`

A sectorial reference file with `status: current` is the default factual authority for normal analysis and list building. Read the relevant sectorial file before using an external source.

Do **not** perform external verification merely because the question asks about exact unit data or Fireteam legality if the required fact is already present in a `current` repository reference.

Use external/current sources only when one of these applies:

1. No reference file exists for the requested sectorial.
2. The relevant file is marked `partial` or `stale`.
3. The requested fact is absent from the reference.
4. The file contains an internal contradiction or unresolved ambiguity relevant to the question.
5. Another repository file establishes that newer Army/rules data supersedes the reference.
6. The user explicitly asks for live/current-source verification, a web/API check, or an update of the reference data.
7. The task is specifically about a newly announced change that postdates the repository reference.

If a local `current` reference and external data are found to disagree, do not silently substitute the external value. Identify the conflict and update/mark the repository reference appropriately when the task permits.

## Sectorial reference semantics

`sectorials/REFERENCE_DESIGN.md` defines the required structure and precedence rules.

Important points:

- Each sectorial file is intended to be self-contained for roster, unit-profile, and Fireteam questions.
- The `## Fireteams` section is the canonical Fireteam definition.
- The Unit → Fireteam access index is derivative and exists for fast lookup. If it conflicts with the canonical Fireteam section, the canonical Fireteam section wins and the reverse index should be corrected.
- Preserve profile/loadout IDs, FTO restrictions, Wildcards, required/min/max members, and `Counts as` relationships.
- Keep Main and Reinforcement Fireteam charts distinct.
- Derived tactical tags, if present, are analysis rather than official Army characteristics.
- A file marked `current` must carry source/provenance fields describing the Army revision and InfinityDB commit used to create or verify it.

For modular army-block analysis, answer from these reference files whenever possible rather than reconstructing Fireteam legality from memory or repeatedly looking it up online.

## Infinity Army and InfinityDB data

Use these sources primarily to **create, refresh, or verify repository reference files**, or when the local-reference-first exceptions above apply.

### Corvus Belli Infinity Army API

The official Army API is available under:

- `https://api.corvusbelli.com/army/infinity/en/metadata`
- Unit/army documents are exposed through the same `https://api.corvusbelli.com/army` API family.

Direct requests may return `403` unless made with browser-like request headers. InfinityDB's downloader is a useful reference implementation; it sends headers such as `Origin: https://infinityuniverse.com`, an Infinity Universe `Referer`, and a normal browser `User-Agent`.

Prefer the official Army API for direct source verification when necessary, but do not spend time reverse-engineering access if InfinityDB already exposes the same source data in a normalized form.

### InfinityDB

Primary references:

- Site: `https://infinitydb.tsudao.com/`
- Source: `https://github.com/frankysan/InfinityDB`

InfinityDB ingests Infinity Army data and normalizes units, profiles, loadouts, army membership, and Fireteam relationships. It is the preferred structured interface for generating and updating sectorial reference files.

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

When refreshing a reference file, preserve these structured relationships rather than simplifying them into prose.

## Rules references

For rules questions, prefer the repository's `rules/` reference material first. `rules/README.md` states the current local rules baseline and the precedence of versioned correction files.

Use live official rules/wiki sources when:

- the local rules reference does not answer the question;
- the local material is explicitly known to be superseded;
- a contradiction needs resolution; or
- the user asks for current/live verification.

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

## Authority order

For ordinary sectorial/unit/list-building work:

1. Relevant `sectorials/...` file with `status: current`.
2. Repository `rules/` files for rules semantics.
3. Repository `units/` change references when historical/update context matters.
4. Current Corvus Belli Army/rules data when local data is insufficient or requires verification.
5. Current InfinityDB normalized data for structured reconciliation or refresh.
6. Historical Army snapshots for before/after comparisons.
7. Reliable community analysis for discovery, interpretation, or undocumented-hotfix detection; verify against structured data whenever possible.

For Fireteams specifically, use the sectorial file's canonical `## Fireteams` section first. Use InfinityDB's current structured Fireteam chart only when the local-reference-first policy calls for external verification or when generating/updating that sectorial file.