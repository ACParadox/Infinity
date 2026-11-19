# Repository Agent Guidance

## Source of truth

- Treat the latest committed `main` branch of this repository as authoritative for project material.
- Before changing project files, read the specific relevant files first and preserve existing decisions unless the requested change explicitly supersedes them.
- Do not rely on model memory for exact Infinity rules, profiles, points, SWC, AVA, or Fireteam legality when repository reference data exists.

## Markdown heading hierarchy

- Each Markdown file must have **exactly one top-level `#` heading**, placed at the very beginning of the file (apart from any required YAML front matter).
- Do not add any other `#` headings anywhere in the same file. Use `##` for main sections, `###` for subsections, and deeper levels only as needed.
- Preserve this heading hierarchy when creating, editing, or reorganizing Markdown files.

## Unit and profile list formatting

When writing or editing faction analysis, tactical notes, or other explanatory Markdown:

- **If a prose paragraph mentions multiple distinct units or alternative profiles, use a Markdown bullet list**, preferably one bullet per unit/profile with its role, relevant statistics and trade-offs. Keep a short introductory sentence and any conclusion outside the list.
- For comparisons, give each alternative its own bullet rather than packing several named units or profiles into a dense sentence.
- Treat a **Fireteam or explicitly synergistic multi-unit package as one named combination** when its members must be understood together; present alternative packages as separate bullets. Nested bullets can distinguish individual members when useful.
- Existing structured comparison tables or straightforward relationship statements (for example, who counts as whom in a Fireteam) do not need redundant lists. Do not sacrifice factual precision merely to force a list.
- Preserve profile identifiers, points/SWC, legality caveats, source links and the original tactical meaning when reformatting.

## Local-reference-first policy

For ordinary questions about a sectorial, its units, profiles, points/SWC, availability, or Fireteam access, **use the repository reference files first instead of searching the web or querying live APIs**.

Sectorial reference format:

- Design/schema: `sectorials/REFERENCE_DESIGN.md`
- Sectorial files: `sectorials/<parent-faction>/<sectorial-slug>.md`
- Index, when present: `sectorials/INDEX.md`

A sectorial reference file with `status: current` is the default factual authority for normal analysis and list building. Read the relevant sectorial file before using an external source. **`status: current` does not prove every common/base skill was transcribed**: before asserting a role-defining skill is absent (especially NCO, Forward Observer, Chain of Command or Tactical Awareness), inspect the exact pinned GitHub Army JSON.

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

### Pinned Infinity Army data on GitHub — roster audit authority

For any N5.3 reference **creation, refresh, correction, or skill audit**, start from [`massayoshi/infinity-army-backup`](https://github.com/massayoshi/infinity-army-backup). Fetch `n5/<army-slug>/<army_source_version>.json` **at the precise backup commit stated in that roster's provenance**. Do not assume all faction sources use one commit/version: Kosmoflot/Caledonia/Vanilla Ariadna pin `d4329bb596ffea5d568eb2435f74366c305a7630` and `7.26246.158`, while some other rosters pin `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b` and some use `7.26246.159`. Example: `https://raw.githubusercontent.com/massayoshi/infinity-army-backup/d4329bb596ffea5d568eb2435f74366c305a7630/n5/kosmoflot/7.26246.158.json`.

Use [`frankysan/InfinityDB`](https://github.com/frankysan/InfinityDB) **at the file's `infinitydb_commit`** as a secondary normalization and Fireteam/identity cross-check, not as a replacement for raw source data. Unpinned live InfinityDB or Army API data may have moved on; identify version/date differences before importing them. Corvus Belli's official Army updates, Wiki and FAQ provide independent evidence of changed rules/skills.

**Mandatory base-versus-loadout merge:** `units[].profileGroups[].profiles[]` records the underlying statline, **shared/base skills** and equipment. `units[].profileGroups[].options[]` (and any applicable `units[].options[]`) provides **loadout-specific additions/overrides**. Empty `options[].skills` does **not** imply a trooper has no skills. Check which profile group a selected option uses; combine that group's base skills/equipment with applicable loadout additions/overrides. Do not extrapolate skills across distinct base profiles, weapon options or FTO statuses without source evidence. Keep source parameters, IDs, unit membership, AVA, required members, Wildcards, compound bodies, Reinforcements and Fireteam rules intact.

**Checklist before publishing a `current` roster, auditing it, or rejecting a historical claim:**

1. Match the source GitHub commit, version, faction slug, unit ID, profile group and option ID in the roster provenance.
2. Compare **all applicable base-profile skills and equipment** as well as all loadout skills/equipment to the Markdown. Explicitly inspect NCO, Forward Observer, Chain of Command, Tactical Awareness, Lieutenant, Engineer/Doctor/Paramedic, Hacker/KHD, vision/marker/deployment and other mission-critical skills.
3. Confirm whether a capability is unit-wide or option-/group-specific and whether it can join the stated Fireteam. A skill can apply to a non-FTO troop even when that troop cannot link.
4. Independently investigate conflicting screenshots, official change logs and recordings. Mark unresolved discrepancies `partial`/`stale`, and propagate verified corrections to tactical/list-building and purchasing notes rather than leaving contradictory claims.
5. **Never conclude "skill removed" merely because a Markdown roster or `options[].skills` omitted it.** Validate negative claims against the pinned source.

**Regression example (19 Nov 2026):** Scots Guards' NCO and Forward Observer were present in `profileGroups[].profiles[].skills`, but a local transcription used only empty `options[].skills` and erroneously rejected the NCO/FO combination. Corrected Kosmoflot and Caledonian rosters document both shared skills, while only Scots Guard **FTO** options can join the relevant Fireteams. Corvus Belli's October 2025 Army update separately confirms these additions.

### Corvus Belli Infinity Army API

The official Army API is available under:

- `https://api.corvusbelli.com/army/infinity/en/metadata`
- Unit/army documents are exposed through the same `https://api.corvusbelli.com/army` API family.

Direct requests may return `403` unless made with browser-like request headers. InfinityDB's downloader is a useful reference implementation; it sends headers such as `Origin: https://infinityuniverse.com`, an Infinity Universe `Referer`, and a normal browser `User-Agent`.

For live/current Army verification or update detection, use the official Army API when accessible. To reproduce or audit a **pinned roster**, fetch the pinned GitHub raw snapshot above instead of silently substituting live data.

### InfinityDB

Primary references:

- Site: `https://infinitydb.tsudao.com/`
- Source: `https://github.com/frankysan/InfinityDB`

InfinityDB ingests Infinity Army data and normalizes units, profiles, loadouts, army membership, and Fireteam relationships. It is a **secondary structured normalization/Fireteam reference** for generating and updating sectorial files; the exact pinned raw Army GitHub snapshot is primary for verifying common/base skills and profile loadouts.

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

## Miniature proxy quality policy

For recommendations involving a model of **one unit representing a different unit**, follow the [miniature proxy guidelines](notes/miniature-proxy-guidelines.md): same **silhouette including base and height**, prefer similar **troop class / armour / physical archetype**, and **avoid a donor that is itself selectable in the target sectorial**. If no good owned proxy exists, say so rather than using a misleading alien TAG, dog model as armoured infantry or an incorrect silhouette. This is a collection-clarity preference, not an official legality claim. Do not modify the underlying inventory ownership totals when re-ranking a proxy.

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
4. **The exact pinned** `massayoshi/infinity-army-backup` JSON at its recorded commit/version for roster corrections and negative-skill audits.
5. **Pinned** `frankysan/InfinityDB` commit for semantic normalization and Fireteam reconciliation.
6. Current official Corvus Belli Army/API, Wiki, changelog and FAQ to verify later/live changes, clearly distinguishing them from the pinned baseline.
7. Other historical snapshots for before/after comparisons.
8. Reliable community analysis for discovery, interpretation, or undocumented-hotfix detection; verify against structured data whenever possible.

For Fireteams specifically, use the sectorial file's canonical `## Fireteams` section first. Use InfinityDB's current structured Fireteam chart only when the local-reference-first policy calls for external verification or when generating/updating that sectorial file.