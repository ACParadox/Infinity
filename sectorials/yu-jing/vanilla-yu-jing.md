---
schema_version: 1
reference_type: sectorial
status: partial
sectorial_id: 201
sectorial_slug: yu-jing
sectorial_name: Vanilla Yu Jing
parent_faction: Yu Jing
rules_baseline: N5.3
army_source_version: "7.26246.158"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-15
coverage: "Complete standard vanilla Yu Jing roster membership/AVA, canonical vanilla Fireteam chart and reverse index, optional-mode hooks, and linked Daebak Force Reinforcement roster/Fireteam chart. Vanilla-specific Hulang, Krit Kokram, RacerBot and Hac Tao profile distinctions are recorded; the remaining loadout tables are deliberately source-linked rather than copied from sectorial projections until their vanilla profile projection is completed."
---

# Vanilla Yu Jing

## Overview and provenance

Repository-native reference for **vanilla Yu Jing** (`army_id: 201`). This file uses the repository's sectorial-reference schema even though Yu Jing is the parent vanilla faction rather than a sectorial.

Sources used:

- Army-derived Yu Jing source revision `7.26246.158` from `massayoshi/infinity-army-backup` commit `d4329bb596ffea5d568eb2435f74366c305a7630`, especially `n5/yu-jing/7.26246.158.json` and its `n5/yu-jing/units/` parent-unit records.
- Existing repository Yu Jing references (`invincible-army.md`, `white-banner.md`, `imperial-service.md`) as cross-checks only. Their faction-specific profile projections are **not** assumed to be identical to vanilla.
- InfinityDB Fireteam normalization/semantics at commit `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: N5.3 + the current N5 FAQ material tracked by this repository.

Coverage notes:

- The ordinary matched-play roster contains **55 standard units** in Army roster order.
- `Guǐ Fēng Spec-Ops` and `Yu Jing Team-Ops` are optional-mode hooks, not ordinary matched-play roster entries.
- Soldier-of-Fortune-only catalog entries are not part of the base Yu Jing roster.
- Vanilla Yu Jing has a real, limited Fireteam chart in the pinned Army source: **no Core, maximum 1 Haris, maximum 2 Duos**.
- Fireteam legality comes from the canonical chart below, not from an `FTO` loadout name alone.
- The chart-level `FTO` restrictions on Húláng and Krit Kokram use their exact vanilla `FTO` profiles, not their `FTO-2` profiles.
- Linked Reinforcement army: **Daebak Force** (`army_id: 299`). Its roster and Fireteams are kept separate from the main Yu Jing chart.
- This file is marked `partial` only because the complete per-loadout vanilla projection has not yet been copied inline for every shared unit. The roster, AVA, Fireteam data and Reinforcement chart are complete against the pinned source.

## Sectorial summary

| Field | Value |
|---|---|
| Faction | Vanilla Yu Jing |
| Parent faction | Yu Jing |
| Army ID | 201 |
| Rules baseline | N5.3 |
| Standard roster units | 55 |
| Optional-mode units | Guǐ Fēng Spec-Ops; Yu Jing Team-Ops |
| Linked Reinforcement roster | Daebak Force (Army ID 299) |
| Main Fireteam chart | yes |
| Reinforcement Fireteam chart | yes |

## Fireteam chart limits and faction-level restrictions

| Constraint | Value / wording |
|---|---|
| Core | `0`: none |
| Haris | `1`: maximum 1 |
| Duo | `2`: maximum 2 |
| Main/Reinforcement mixing | no source exception recorded; charts are kept separate |
| FTO labels | only chart-level FTO restrictions create profile restrictions; an FTO label by itself does not grant access |

## Roster index

| Unit | ID | AVA | Type | Order | Vanilla Fireteam access |
|---|---:|---:|---|---|---|
| Chaīyì Yáokòng | 142 | 1 | REM | Regular | — |
| Hǎidào Special Support Group | 1246 | 1 | HI | Regular | Yu Jing Fireteams Duo max 1 |
| Libertos Freedom Fighters | 1275 | 1 | LI | Irregular | — |
| Dāoyīng Operative Control Unit | 1244 | 1 | MI | Regular | — |
| Gūijiă Squadrons | 133 | 2 | TAG | Regular | Yu Jing Fireteams Duo max 1 |
| Léi Gōng | 1497 | 1 | HI | Regular | — |
| Shàng Jí Invincibles | 150 | 2 | HI | Regular | Yu Jing Fireteams Duo max 2 |
| Dàofěi Tactical Section | 130 | 1 | HI | Regular | — |
| Mówáng Troops | 1254 | 1 | HI | Regular | Yu Jing Fireteams Duo max 1 |
| Hwarang Corps | 1752 | 2 | HI | Regular | Yu Jing Fireteams II max 1 |
| Dokkaebi Cyberteam | 1756 | 1 | HI | Regular | Yu Jing Fireteams II max 1 |
| Bìxié, the Jade Champion | 1599 | 1 | HI | Regular | Yu Jing Fireteams II max 1 |
| Haetae Unit | 1754 | 1 | HI | Regular | — |
| Hùsòng Yáokòng | 140 | 2 | REM | Regular | — |
| Naval Operations Group Sulyong | 1755 | 2 | MI | Regular | Yu Jing Fireteams II max 2 |
| Zhēnchá | 1259 | 2 | HI | Regular | — |
| Yáoxiè Lù Duān | 160 | 2 | REM | Regular | — |
| Sun Tze | 143 | 1 | HI | Regular | — |
| Blue Wolf Mongol Cavalry | 1495 | 1 | TAG | Regular | Yu Jing Fireteams Duo max 1 |
| Zhànyīng Imperial Agents | 125 | 1 | LI | Regular | Yu Jing Fireteams Duo max 1 |
| Major Lunah | 947 | 1 | LI | Regular | — |
| Johnny Kao | 1892 | 1 | MI | Regular | Wildcard max 1 |
| RacerBots | 1905 | 2 | REM | Regular | — |
| Yáofáng Lóng Yá | 1537 | 2 | REM | Regular | — |
| Tiger Soldiers | 126 | 2 | MI | Regular | — |
| Qíshì, StateEmpire TAG Support Pilots | 1838 | 1 | LI | Regular | — |
| Yáoxiè Rui Shi | 159 | 2 | REM | Regular | — |
| Gŭiláng Skirmishers | 134 | 2 | SK | Regular | — |
| Yān Huǒ Invincibles | 128 | 2 | HI | Regular | — |
| Beasthunters Free Guild | 1570 | 1 | SK | Irregular | — |
| Hac Tao Special Unit | 131 | 1 | HI | Regular | — |
| Hsien Warriors | 132 | 1 | HI | Regular | — |
| Krit Kokram | 1445 | 1 | HI | Regular | Both Yu Jing team pools, FTO profiles only |
| Hùndùn Ambush Unit | 1492 | 1 | MI | Regular | — |
| Shaolin Warrior Monks | 136 | 4 | WB | Irregular + Impetuous | Yu Jing Fireteams Duo max 2 |
| Wèibīng Yáokòng | 139 | 2 | REM | Regular | — |
| Zhanshi Yīshēng | 137 | 1 | LI | Regular | — |
| Sulsa Warriors | 1753 | 1 | SK | Regular | — |
| Yáopú Pangguling | 162 | 2 | REM | Regular | — |
| Imperial Agent, Pheasant Rank | 148 | 1 | MI | Regular | Yu Jing Fireteams Duo max 1 |
| Húláng Shocktroopers | 1257 | 1 | HI | Regular | Yu Jing Fireteams Duo max 1, FTO profiles only |
| Yáozăo | 161 | 3 | REM | Peripheral | — |
| Kuang Shi | 146 | 4 | LI | Regular + Impetuous | — |
| Zhanshi | 124 | 255 | LI | Regular | — |
| Silver Snakes, Yín-Shé Unit | 1840 | 2 | MI | Regular | — |
| Ninjas | 135 | 2 | SK | Regular | — |
| Fēiquán Imperial Tactical Wing | 1842 | 1 | VH | Regular | — |
| Warcors | 50 | 1 | LI | Irregular | — |
| Lóngwáng, Imperial TAG Police | 1839 | 1 | TAG | Regular | — |
| Son-Bae Yáokòng | 141 | 2 | REM | Regular | — |
| Liú Xīng Jump Infantry | 1248 | 1 | HI | Regular | — |
| Gūdǎn Troops | 1841 | 2 | LI | Regular | — |
| Mech-Engineer (Zhanshi Gōngchéng) | 138 | 1 | LI | Regular | — |
| Sù-Jiàn Immediate Action Unit | 155 | 1 | HI | Regular | Yu Jing Fireteams Duo max 1 |
| Zúyŏng Invincibles | 127 | 3 | HI | Regular | Both Yu Jing team pools |

### Optional-mode units

| Unit | ID | Mode | Ordinary roster? | Main-chart relevance |
|---|---:|---|---|---|
| Guǐ Fēng Spec-Ops | 1914 | Spec-Ops | No | no ordinary vanilla Fireteam row in the pinned chart |
| Yu Jing Team-Ops | 1928 | Team-Ops | No | no ordinary vanilla Fireteam row |

## Unit details and vanilla profile provenance

The pinned **vanilla** Army source is authoritative for profile/loadout values. Do not substitute the same unit's Invincible Army, White Banner or Imperial Service values without checking: some shared units have faction-specific profile projections.

Until every loadout table is copied inline, use the roster ID above with the pinned Yu Jing source `n5/yu-jing/7.26246.158.json` and the matching parent-unit record under `n5/yu-jing/units/`. The following vanilla-specific cases are recorded explicitly because they affect list construction or Fireteam legality.

### RacerBots

**Unit ID:** 1905  
**AVA:** 2  
**Troop type:** REM  
**Regularity:** Regular

Two profile groups share `MOV 20-15 | CC 8 | BS 11 | PH 12 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 4`.

#### RacerBot Brute

Base: Remote Presence, Courage, Berserk (Hyper-Dynamics), Tactical Awareness.

| Profile ID | Points | SWC | Distinguishing facts |
|---:|---:|---:|---|
| 1 | 16 | 0 | RacerBot Brute; BS Attack (+1B) |
| 2 | 14 | 0 | RacerBot Brute; BS Attack (+1B) |

#### RacerBot Gearhead

Base: Engineer; Deactivator, GizmoKit.

| Profile ID | Points | SWC | Distinguishing facts |
|---:|---:|---:|---|
| 1 | 16 | 0 | RacerBot Gearhead (Engineer) |
| 2 | 13 | 0 | RacerBot Gearhead (Engineer) |

### Húláng Shocktroopers — vanilla projection

**Unit ID:** 1257  
**AVA:** 1  
**Troop type:** HI  
**Regularity:** Regular

Vanilla parent profile: `MOV 15-5 | CC 22 | BS 13 | PH 13 | WIP 13 | ARM 3 | BTS 3 | W 2 | S 2`.

| Profile ID | Label | Points | SWC | Vanilla Fireteam eligibility |
|---:|---|---:|---:|---|
| 1 | HÚLÁNG FTO-2 | 36 | 0 | no — chart says `FTO`, not `FTO-2` |
| 2 | HÚLÁNG FTO-2 | 37 | 0 | no — chart says `FTO`, not `FTO-2` |
| 3 | HÚLÁNG FTO | 36 | 0 | yes — Yu Jing Fireteams Duo max 1 |
| 4 | HÚLÁNG FTO | 37 | 0 | yes — Yu Jing Fireteams Duo max 1 |

Profile 2/4 adds a Cybermine in the parent vanilla projection.

### Krit Kokram — vanilla projection

**Unit ID:** 1445  
**AVA:** 1  
**Troop type:** HI  
**Regularity:** Regular

Vanilla parent profile: `MOV 15-5 | CC 17 | BS 13 | PH 12 | WIP 13 | ARM 3 | BTS 6 | W 2 | S 2`. Engineer; Deactivator and GizmoKit.

| Profile ID | Label | Points | SWC | Vanilla Fireteam eligibility |
|---:|---|---:|---:|---|
| 1 | KRIT KOKRAM FTO-2 | 37 | 0 | no — chart says `FTO`, not `FTO-2` |
| 2 | KRIT KOKRAM FTO | 35 | 0 | yes — either vanilla Yu Jing team pool |
| 3 | KRIT KOKRAM FTO | 40 | 0 | yes — either vanilla Yu Jing team pool |

### Hac Tao Special Unit — vanilla projection

**Unit ID:** 131  
**AVA:** 1  
**Troop type:** HI  
**Regularity:** Regular

The vanilla source exposes the following standard loadout IDs in the pinned projection; do not substitute the White Banner/Invincible Army point/SWC projection without checking the vanilla source.

| Profile ID | Points | SWC | Loadout / role |
|---:|---:|---:|---|
| 4 | 54 | 1.5 | Missile Launcher, Nanopulser, Boarding Shotgun, Pistol, AP CCW |
| 5 | 58 | 0 | AP HMG, Nanopulser, Pistol, AP CCW; Hacking Device |
| 7 | 56 | +1 | AP HMG, Nanopulser, Pistol, AP CCW; NCO |

## Canonical Fireteams

This section is authoritative for main-force Fireteam legality in this file. The reverse index below is derivative.

### FT-01 — Yu Jing Fireteams

**Type:** Duo  
**Chart context:** Main vanilla Yu Jing

| Member | Unit ID | Required | Min | Max | Counts as | FTO restriction | Allowed loadout IDs | Notes |
|---|---:|---|---:|---:|---|---|---|---|
| Hǎidào | 1246 | no | 0 | 1 | — | — | all vanilla profiles | — |
| Zhànyīng | 125 | no | 0 | 1 | — | — | all vanilla profiles | — |
| Imperial Agent, Pheasant Rank | 148 | no | 0 | 1 | — | — | all vanilla profiles | — |
| Zúyŏng | 127 | no | 0 | 2 | — | — | all vanilla profiles | — |
| Shàng Jí | 150 | no | 0 | 2 | — | — | all vanilla profiles | — |
| Húláng | 1257 | no | 0 | 1 | — | FTO | 3, 4 | `FTO-2` profiles do not satisfy this row |
| Sù-Jiàn | 155 | no | 0 | 1 | — | — | all vanilla profiles | — |
| Mówáng | 1254 | no | 0 | 1 | — | — | all vanilla profiles | — |
| Gūijiă | 133 | no | 0 | 1 | — | — | all vanilla profiles | — |
| Blue Wolf | 1495 | no | 0 | 1 | — | — | all vanilla profiles | — |
| Shaolin Warrior Monk | 136 | no | 0 | 2 | — | — | all vanilla profiles | — |
| Krit Kokram | 1445 | no | 0 | 1 | — | FTO | 2, 3 | `FTO-2` profile does not satisfy this row |

### FT-02 — Yu Jing Fireteams II

**Types:** Duo, Haris  
**Chart context:** Main vanilla Yu Jing

| Member | Unit ID | Required | Min | Max | Counts as | FTO restriction | Allowed loadout IDs | Notes |
|---|---:|---|---:|---:|---|---|---|---|
| Zúyŏng | 127 | no | 0 | 3 | — | — | all vanilla profiles | — |
| Sulyong | 1755 | no | 0 | 2 | — | — | all vanilla profiles | — |
| Hwarang | 1752 | no | 0 | 1 | — | — | all vanilla profiles | — |
| Dokkaebi | 1756 | no | 0 | 1 | — | — | all vanilla profiles | — |
| Bìxié | 1599 | no | 0 | 1 | — | — | all vanilla profiles | — |
| Krit Kokram | 1445 | no | 0 | 1 | — | FTO | 2, 3 | `FTO-2` profile does not satisfy this row |

### Main-force Wildcards

| Wildcard | Unit ID | Max | Counts as | FTO/profile restriction | Notes |
|---|---:|---:|---|---|---|
| Johnny Kao | 1892 | 1 | — | all vanilla profiles | May join an otherwise legal main-force Yu Jing Fireteam; does not remove team-size or chart-limit requirements |

## Unit → Fireteam access index

| Unit | Fireteam | Type | Access | Profile restriction | Min/Max | Notes |
|---|---|---|---|---|---|---|
| Hǎidào | FT-01 Yu Jing Fireteams | Duo | native | all | 0–1 | — |
| Zhànyīng | FT-01 Yu Jing Fireteams | Duo | native | all | 0–1 | — |
| Pheasant Agent | FT-01 Yu Jing Fireteams | Duo | native | all | 0–1 | — |
| Zúyŏng | FT-01 Yu Jing Fireteams | Duo | native | all | 0–2 | also FT-02 |
| Shàng Jí | FT-01 Yu Jing Fireteams | Duo | native | all | 0–2 | — |
| Húláng | FT-01 Yu Jing Fireteams | Duo | native | profile 3/4 `FTO` only | 0–1 | `FTO-2` excluded by chart row |
| Sù-Jiàn | FT-01 Yu Jing Fireteams | Duo | native | all | 0–1 | — |
| Mówáng | FT-01 Yu Jing Fireteams | Duo | native | all | 0–1 | — |
| Gūijiă | FT-01 Yu Jing Fireteams | Duo | native | all | 0–1 | — |
| Blue Wolf | FT-01 Yu Jing Fireteams | Duo | native | all | 0–1 | — |
| Shaolin | FT-01 Yu Jing Fireteams | Duo | native | all | 0–2 | — |
| Krit Kokram | FT-01 Yu Jing Fireteams | Duo | native | profile 2/3 `FTO` only | 0–1 | also FT-02 |
| Zúyŏng | FT-02 Yu Jing Fireteams II | Duo/Haris | native | all | 0–3 | also FT-01 |
| Sulyong | FT-02 Yu Jing Fireteams II | Duo/Haris | native | all | 0–2 | — |
| Hwarang | FT-02 Yu Jing Fireteams II | Duo/Haris | native | all | 0–1 | — |
| Dokkaebi | FT-02 Yu Jing Fireteams II | Duo/Haris | native | all | 0–1 | — |
| Bìxié | FT-02 Yu Jing Fireteams II | Duo/Haris | native | all | 0–1 | — |
| Krit Kokram | FT-02 Yu Jing Fireteams II | Duo/Haris | native | profile 2/3 `FTO` only | 0–1 | also FT-01 |
| Johnny Kao | all eligible main Yu Jing teams | varies | wildcard | all | max 1 | does not bypass main Fireteam limits |

All other standard vanilla Yu Jing units have no main-chart Fireteam row in the pinned source.

## Reinforcements — Daebak Force

Linked Army ID: **299**. The pinned Daebak document has a distinct Reinforcement roster and Fireteam chart. It is not merged into the main vanilla Yu Jing chart.

### Reinforcement roster membership

| Unit | ID | AVA | Type |
|---|---:|---:|---|
| Reinf. Yáozăo | 1709 | 2 | REM |
| Reinf. Hwarang Corps | 1711 | 4 | HI |
| Reinf. Sulsa Warriors | 1712 | 2 | SK |
| Reinf. Yáoxiè Rui Shi | 1718 | 1 | REM |
| Reinf. Chief Mech-Engineer Chung-Hee Jeong | 1708 | 1 | LI |
| Reinf. Dokkaebi Cyberteam | 1715 | 2 | HI |
| Reinf. Son-Bae Yáokòng | 1717 | 1 | REM |
| Reinf. Naval Operations Group Sulyong | 1714 | 2 | MI |
| Reinf. Bìxié, the Jade Champion | 1719 | 1 | HI |
| Reinf. Jujak Regiment | 1707 | 3 | HI |
| Reinf. Wèibīng Yáokòng | 1716 | 2 | REM |
| Reinf. Sergeant So-ra Kwon | 1710 | 1 | HI |
| Reinf. Haetae Unit | 1713 | 1 | HI |

### Reinforcement Fireteam chart limits

The Daebak source `spec` block records `CORE: 0`, `HARIS: 0`, `DUO: 0`; the named Reinforcement Fireteam rows below still explicitly define the available formations. Do not reinterpret those zero values as deleting the named rows.

### RF-01 — Jujaks Reinforcement Fireteams

**Types:** Duo, Haris, Core

| Member | Unit ID | Min | Max | Counts as | Restriction |
|---|---:|---:|---:|---|---|
| Jujak REF. | 1707 | 1 | 3 | — | native minimum 1 |
| Hwarang REF. | 1711 | 0 | 1 | — | — |

### RF-02 — Hwarang Reinforcement Fireteams

**Types:** Duo, Haris, Core

| Member | Unit ID | Min | Max | Counts as | Restriction |
|---|---:|---:|---:|---|---|
| Hwarang REF. | 1711 | 1 | 4 | — | native minimum 1 |
| Sulsa Warrior REF. | 1712 | 0 | 2 | Hwarang | — |
| Haetae REF. | 1713 | 0 | 1 | — | — |
| Bìxié REF. | 1719 | 0 | 1 | — | — |

### Reinforcement Wildcards

| Wildcard | Unit ID | Max | Counts as | FTO restriction |
|---|---:|---:|---|---|
| Sulyong REF. | 1714 | 2 | — | — |
| Wèibīng Yáokòng REF. | 1716 | 2 | — | — |
| Son-Bae Yáokòng REF. | 1717 | 1 | — | FTO; option 3 |
| Dokkaebi REF. | 1715 | 1 | — | — |
| Chief Jeong REF. | 1708 | 1 | — | — |
| So-ra Kwon REF. | 1710 | 1 | Jujaks | — |

### Reinforcement units without chart access

- Reinf. Yáozăo — servant peripheral; no Fireteam row.
- Reinf. Yáoxiè Rui Shi — no Fireteam row.

## Tactical tags

Derived analysis aids, not official characteristics. These tags are intentionally broad until the complete vanilla loadout projection is inlined.

| Unit | Tags |
|---|---|
| Gūijiă | TAG, TacAware, heavy gunfighter, CC mobility |
| Blue Wolf | TAG, mobile attack, close-range pressure |
| Lóngwáng | TAG, TacAware/NCO profile family, control weapons |
| Hac Tao | hidden deployment, Mimetism (-6), heavy gunfighter/hacker/NCO |
| Dàofěi | camouflaged/infiltrating HI, midfield attacker/specialist |
| Húláng | midfield/assault HI, strong CC, vanilla Duo option through FTO profiles |
| Mówáng | durable attack HI, vanilla Duo option |
| Shàng Jí | TacAware HI, vanilla Duo option |
| Zúyŏng | efficient HI, vanilla Duo/Haris anchor |
| Sulyong | mobile MI, vanilla Duo/Haris option |
| Hwarang | aggressive HI, vanilla Duo/Haris option |
| Dokkaebi | cyber/support HI, vanilla Duo/Haris option |
| Bìxié | mobile NCO/FO character, vanilla Duo/Haris option |
| Krit Kokram | Engineer, vanilla Duo/Haris option through exact FTO profiles |
| Sù-Jiàn | very fast durable attack piece, vanilla Duo option |
| Shaolin | smoke/CC warband, vanilla Duo option |
| Johnny Kao | main-force Wildcard |
| Gŭiláng | camouflaged infiltrating specialist |
| Zhēnchá | camouflaged infiltrating HI specialist |
| Tiger Soldier | airborne attack/specialist |
| Liú Xīng | airborne HI attack/specialist |
| RacerBot | very fast TacAware attack/support REM profiles |
| Wèibīng | Sensor/FO Repeater |
| Pangguling | Baggage/EVO/support REM |
| Son-Bae | missile/guided support REM |
| Rui Shi | attack REM |
| Lù Duān | Holoprojector attack REM |

## Validation and maintenance

- Standard vanilla Yu Jing roster represented: **55 units**.
- Optional-mode hooks represented: **Guǐ Fēng Spec-Ops** and **Yu Jing Team-Ops**.
- Main Fireteam limits preserved: **Core 0, Haris 1, Duo 2**.
- Canonical main Fireteam rows represented: **Yu Jing Fireteams, Yu Jing Fireteams II, Wildcards**.
- Húláng chart access is restricted to vanilla profile IDs **3/4** (`FTO`), not `FTO-2` IDs 1/2.
- Krit Kokram chart access is restricted to vanilla profile IDs **2/3** (`FTO`), not `FTO-2` ID 1.
- Johnny Kao is represented as a main-force Wildcard, maximum 1.
- Linked Reinforcement force **Daebak Force** is represented separately with its distinct roster and Fireteam chart.
- Reinforcement chart rows represented: **Jujaks Reinforcement, Hwarang Reinforcement, Reinforcement Wildcards**.
- Main and Reinforcement Fireteams are deliberately not merged.
- Shared-unit sectorial profiles are not silently substituted for vanilla profiles. Where a full vanilla loadout table is not yet inlined, the pinned vanilla Army source remains authoritative.

### Remaining work before `status: current`

Inline and verify the complete vanilla loadout table for every standard unit against `n5/yu-jing/7.26246.158.json` / `n5/yu-jing/units/`, preserving vanilla-specific stats, points, SWC, profile IDs and equipment. Do **not** bulk-copy sibling sectorial projections without checking the vanilla source first.

### Refresh rule

When a newer Army source revision or InfinityDB normalization supersedes the provenance above, set `status: stale` until roster/profile/Fireteam changes are reconciled. Do not silently mix newer live values into this file without updating the provenance block.
