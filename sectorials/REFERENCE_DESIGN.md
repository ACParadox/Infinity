# Sectorial Reference File Design

## Purpose

Sectorial reference files are the repository-native source for answering questions about a sectorial's roster, unit profiles, availability, points/SWC, and Fireteam access without repeatedly querying external sites.

The files should be sufficiently complete for an LLM to answer questions such as:

- What profiles does this unit have in this sectorial?
- What are their points/SWC, stats, skills, equipment, and weapons?
- What Fireteams can this unit join?
- Is the unit a native member, Wildcard, required member, or a `Counts as` member?
- Is Fireteam access restricted to an FTO marker or a specific loadout?
- Which units can join a particular Core/Haris/Duo/named Fireteam?
- What Fireteam limits apply to the sectorial?

The design intentionally stores both the canonical Fireteam chart and a generated per-unit Fireteam index. The Fireteam chart is authoritative; the per-unit index exists for fast lookup and must be mechanically consistent with it.

## Directory layout

Use one Markdown file per sectorial:

```text
sectorials/
  REFERENCE_DESIGN.md
  INDEX.md
  panoceania/
    kestrel-colonial-force.md
    military-orders.md
    varuna-immediate-reaction-division.md
    neoterran-capitaline-army.md
  ariadna/
    tartary-army-corps.md
    caledonian-highlander-army.md
    kosmoflot.md
  aleph/
    operations-subsection.md
    steel-phalanx.md
  ...
```

Use stable public slugs where possible. Do not create separate unit files unless a later design change explicitly calls for that; the sectorial file should be self-contained so an LLM can read one file and answer most sectorial questions.

## File contract

Every sectorial file should follow the sections below in the same order.

### 1. Machine-readable metadata

Start with YAML front matter.

```yaml
---
schema_version: 1
reference_type: sectorial
status: current            # current | partial | stale
sectorial_id: 107
sectorial_slug: kestrel-colonial-force
sectorial_name: Kestrel Colonial Force
parent_faction: PanOceania
rules_baseline: N5.3
army_source_version: "7.26246.158"
army_data_changed_on: 2026-09-03
infinitydb_commit: "<commit sha used to generate/verify this file>"
verified_on: 2026-10-15
---
```

Field meanings:

- `schema_version`: version of this repository format.
- `status`:
  - `current` — complete reference generated/verified against the stated source versions.
  - `partial` — usable but one or more required sections are incomplete.
  - `stale` — known to have been superseded by newer Army/Fireteam data.
- `sectorial_id`: Corvus Belli/InfinityDB Army identifier where available.
- `army_source_version`: source revision from the Army document/snapshot.
- `army_data_changed_on`: date encoded/derived from the Army source revision when known.
- `infinitydb_commit`: pinned InfinityDB commit used for normalized data or Fireteam semantics.
- `verified_on`: date the repository file was last checked.

Do not label a file `current` if required data is knowingly missing.

## 2. Sectorial summary

Include a small factual summary table:

| Field | Value |
|---|---|
| Sectorial | Kestrel Colonial Force |
| Parent faction | PanOceania |
| Army ID | 107 |
| Rules baseline | N5.3 |
| Main roster units | N |
| Reinforcement roster | yes/no |
| Fireteam chart | yes |

This section is factual metadata, not tactical analysis.

## 3. Fireteam chart limits and sectorial-level restrictions

Record chart-wide constraints before individual teams.

Example:

| Constraint | Value / wording |
|---|---|
| Core | up to X |
| Haris | up to X |
| Duo | up to X |
| Special/named teams | exact source wording or normalized requirement |
| Main/Reinforcement mixing | prohibited/allowed as applicable |

Preserve explicit source wording when a restriction is unusual. Do not infer a restriction merely from common Fireteam rules.

## 4. Unit roster index

Provide one compact row per logical unit available to the sectorial.

| Unit ID | Unit | AVA | Troop type | Classification | Regularity | Notes |
|---:|---|---:|---|---|---|---|

The index is for navigation. Detailed profile data belongs in the unit sections below.

Distinguish:

- main roster;
- Reinforcement-only roster;
- optional/mercenary inclusions when the source exposes them separately;
- units sharing a canonical profile but having sectorial-specific AVA or Fireteam access.

## 5. Unit details

Create one section per logical unit, ordered as the Army roster presents them unless there is a strong reason to use another stable order.

Use this shape:

```markdown
### Fennec Fusiliers

**Unit ID:** 1234  
**Slug:** `fennec-fusiliers`  
**AVA:** 4  
**Troop type:** LI  
**Classification:** Garrison Troops

#### Base profile

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| ... |

**Skills:** ...  
**Equipment:** ...  
**Characteristics/notes:** ...

#### Loadouts

| Profile ID | FTO | SWC | Points | Weapons | Skills / equipment differences | LT / Specialist / other flags |
|---|---|---:|---:|---|---|---|
| ... |
```

Rules for unit sections:

1. Preserve exact profile distinctions from the structured source.
2. Keep stable profile/loadout IDs where available so Fireteam restrictions can point to an exact row.
3. Put common stats/skills/equipment in `Base profile`; put only loadout-specific differences in the loadout table.
4. If profiles have different statlines, split them into explicit profile groups rather than hiding the difference in prose.
5. Represent Lieutenant, Hacker, KHD, Doctor, Engineer, Forward Observer, Chain of Command, NCO, Tactical Awareness, etc. as source facts, not inferred tactical roles.
6. Do not collapse two profiles merely because their points are the same.
7. Preserve FTO/FTO-X markers exactly.

## 6. Canonical Fireteam definitions

This is the authoritative Fireteam section of the file.

Assign a stable local ID to each Fireteam row, preferably using the source Fireteam ID when stable:

```markdown
## Fireteams

### FT-01 — Fennec Fusiliers

**Types:** Core, Haris  
**Source Fireteam ID:** 17  
**Wildcard team:** no  
**Observation:** exact normalized/source note if present

| Member | Unit ID | Required | Min | Max | Counts as | FTO restriction | Allowed loadout IDs | Notes |
|---|---:|---|---:|---:|---|---|---|---|
| Fennec Fusiliers | 1234 | no | 0 | 3 | Fennec Fusilier | — | all | — |
| Example character | 5678 | no | 0 | 1 | Fennec Fusilier | FTO | 5678-03 | ... |
```

Record all source semantics that affect legality:

- Fireteam type(s): Core, Haris, Duo, named/special formations.
- Member unit.
- required member flag;
- minimum and maximum count;
- Wildcard status;
- `Counts as` / equivalence labels;
- FTO marker restriction;
- exact allowed loadout/profile IDs when restricted;
- observations and source notes;
- Main vs Reinforcement chart context.

### Wildcards

If the chart exposes Wildcards separately, preserve a dedicated subsection:

| Unit | Unit ID | Counts as | FTO/profile restriction | Notes |
|---|---:|---|---|---|

Do not silently inject Wildcards into every Fireteam member table. The canonical representation should match how the source models the chart, while the generated per-unit index may resolve the effective access.

## 7. Unit → Fireteam access index

After the canonical chart, generate a reverse index for fast LLM lookup.

| Unit | Fireteam | Type | Access | Counts as | Profile restriction | Min/Max | Notes |
|---|---|---|---|---|---|---|---|
| Fennec Fusiliers | FT-01 Fennec Fusiliers | Core/Haris | native | Fennec Fusilier | all | 0–3 | — |
| Example character | FT-01 Fennec Fusiliers | Core/Haris | native | Fennec Fusilier | FTO loadout 03 | 0–1 | — |
| Example wildcard | all eligible teams | varies | Wildcard | — | profile 02 only | — | — |

Allowed `Access` values:

- `native`
- `wildcard`
- `required`
- `counts-as`
- `special`

This index is derivative. If it conflicts with `## Fireteams`, the canonical Fireteam definition wins and the index must be corrected.

## 8. Reinforcement Fireteams

If the sectorial has a distinct Reinforcement chart, keep it in a separate section rather than merging it into the main chart.

Use the same schema as the main Fireteam section and explicitly mark:

- Reinforcement roster membership;
- Reinforcement Fireteam chart limits;
- source Fireteam IDs;
- whether any source-defined exceptions exist.

Never imply Main and Reinforcement troopers can mix unless the current rules/source explicitly permit it.

## 9. Derived tactical tags (optional)

A future generator may add a clearly separated, non-authoritative section for fast list-building queries:

```markdown
## Derived tactical index

| Unit/profile | Tags |
|---|---|
| ... | long-range attack, ARO, specialist, network projection, vision control, etc. |
```

These tags are analysis, not source data. They must never overwrite or be confused with actual Army characteristics.

If included, use a controlled vocabulary aligned with this project's modular blocks, such as:

- long-range attack
- mid-range attack
- long-range ARO
- mid-range ARO
- close assault
- specialist
- cheerleader
- TAG support
- REM support
- DZ defense
- midfield defense
- midfield specialist
- warband
- airborne
- enemy-DZ attacker
- network projection
- vision control
- hacker
- KHD
- tech-counter

## 10. Provenance and validation

End each file with provenance.

```markdown
## Provenance

- Corvus Belli Army source revision: `...`
- Army data changed on: YYYY-MM-DD
- InfinityDB commit: `...`
- Fireteam source: InfinityDB normalized Army chart / official Army source
- Generated or verified: YYYY-MM-DD
```

Before marking a file `current`, validate at least:

1. Every roster unit has a detailed unit section.
2. Every source loadout/profile appears exactly once in the unit details unless the source itself duplicates it intentionally.
3. Points and SWC match the pinned structured source.
4. Every Fireteam member references an existing logical unit or an explicitly documented external/alias identity.
5. Every Fireteam loadout restriction references an existing profile/loadout ID.
6. Required/min/max membership values are preserved.
7. `Counts as` labels are preserved exactly enough to reconstruct legal compositions.
8. Wildcards are represented explicitly.
9. The reverse Unit → Fireteam index is consistent with the canonical Fireteam chart.
10. Main and Reinforcement charts are not accidentally merged.
11. Any unresolved source ambiguity is written explicitly and causes `status: partial` unless it is irrelevant to the file's stated coverage.

## Source and precedence rules

For generation or refresh of these files:

1. Use current Corvus Belli Army data when directly available.
2. Use InfinityDB's normalized Army/profile/Fireteam data as the preferred structured interface.
3. Reconcile unusual or ambiguous Fireteam semantics against the official source/rules when necessary.
4. Use historical snapshots only for historical comparisons, not to override a current file.
5. Community material may discover a possible issue but must not silently override structured current data.

Once a sectorial file is committed with `status: current`, it becomes the repository's default factual reference for ordinary sectorial/unit/Fireteam questions. External lookup is not required unless the file is missing, partial, stale, internally contradictory, the requested fact is absent, or the user explicitly asks for live/current-source verification.

## Update policy

When new Army data is known to supersede a sectorial reference:

1. Change `status` to `stale` as soon as the mismatch is established, or update the file in the same change.
2. Regenerate/reconcile unit profiles and the canonical Fireteam chart from the new structured source.
3. Regenerate the reverse Unit → Fireteam index from the canonical chart.
4. Update all provenance fields.
5. Return the file to `status: current` only after the validation checklist passes.

Do not silently retain old points, SWC, AVA, profile options, or Fireteam legality under a `current` status.