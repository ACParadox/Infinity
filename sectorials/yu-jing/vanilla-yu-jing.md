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
coverage: "Complete standard vanilla Yu Jing roster membership/AVA, canonical vanilla Fireteam chart and reverse index, optional-mode hooks, and linked Daebak Force Reinforcement roster/Fireteam chart. Vanilla-specific RacerBot, Hulang, Krit Kokram and Hac Tao profile distinctions are recorded; remaining full vanilla loadout tables are source-linked pending inline projection."
---

# Vanilla Yu Jing

## Overview and provenance

Repository-native reference for **vanilla Yu Jing** (`army_id: 201`). This file uses the repository sectorial-reference schema even though Yu Jing is the parent vanilla faction rather than a sectorial.

Sources used:

- Army-derived Yu Jing source revision `7.26246.158` from `massayoshi/infinity-army-backup` commit `d4329bb596ffea5d568eb2435f74366c305a7630`, especially `n5/yu-jing/7.26246.158.json` and matching parent-unit records under `n5/yu-jing/units/`.
- Existing repository Yu Jing references (`invincible-army.md`, `white-banner.md`, `imperial-service.md`) as cross-checks only. Their faction-specific profile projections are not assumed to be identical to vanilla.
- InfinityDB Fireteam normalization/semantics at commit `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: N5.3 + current N5 FAQ material tracked by this repository.

Coverage notes:

- The ordinary matched-play roster contains **55 standard units** in Army roster order.
- `Guǐ Fēng Spec-Ops` and `Yu Jing Team-Ops` are optional-mode hooks, not ordinary matched-play roster entries.
- Soldier-of-Fortune-only catalog entries are excluded from the base roster.
- Vanilla Yu Jing has a source-defined Fireteam chart: **no Core, maximum 1 Haris, maximum 2 Duos**.
- Fireteam legality comes from the canonical chart below, not from an `FTO` loadout name alone.
- The chart-level `FTO` restrictions on Húláng and Krit Kokram use their exact vanilla `FTO` profiles, not their `FTO-2` profiles.
- Linked Reinforcement army: **Daebak Force** (`army_id: 299`). Its roster and Fireteams are kept separate from the main Yu Jing chart.
- This file remains `partial` only because every vanilla loadout has not yet been copied inline. Roster membership, AVA, main Fireteam data and Reinforcement Fireteam data are complete against the pinned source.

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
| Hǎidào Special Support Group | 1246 | 1 | HI | Regular | FT-01 Duo max 1 |
| Libertos Freedom Fighters | 1275 | 1 | LI | Irregular | — |
| Dāoyīng Operative Control Unit | 1244 | 1 | MI | Regular | — |
| Gūijiă Squadrons | 133 | 2 | TAG | Regular | FT-01 Duo max 1 |
| Léi Gōng | 1497 | 1 | HI | Regular | — |
| Shàng Jí Invincibles | 150 | 2 | HI | Regular | FT-01 Duo max 2 |
| Dàofěi Tactical Section | 130 | 1 | HI | Regular | — |
| Mówáng Troops | 1254 | 1 | HI | Regular | FT-01 Duo max 1 |
| Hwarang Corps | 1752 | 2 | HI | Regular | FT-02 Duo/Haris max 1 |
| Dokkaebi Cyberteam | 1756 | 1 | HI | Regular | FT-02 Duo/Haris max 1 |
| Bìxié, the Jade Champion | 1599 | 1 | HI | Regular | FT-02 Duo/Haris max 1 |
| Haetae Unit | 1754 | 1 | HI | Regular | — |
| Hùsòng Yáokòng | 140 | 2 | REM | Regular | — |
| Naval Operations Group Sulyong | 1755 | 2 | MI | Regular | FT-02 Duo/Haris max 2 |
| Zhēnchá | 1259 | 2 | HI | Regular | — |
| Yáoxiè Lù Duān | 160 | 2 | REM | Regular | — |
| Sun Tze | 143 | 1 | HI | Regular | — |
| Blue Wolf Mongol Cavalry | 1495 | 1 | TAG | Regular | FT-01 Duo max 1 |
| Zhànyīng Imperial Agents | 125 | 1 | LI | Regular | FT-01 Duo max 1 |
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
| Krit Kokram | 1445 | 1 | HI | Regular | FT-01/FT-02, exact FTO profiles only |
| Hùndùn Ambush Unit | 1492 | 1 | MI | Regular | — |
| Shaolin Warrior Monks | 136 | 4 | WB | Irregular + Impetuous | FT-01 Duo max 2 |
| Wèibīng Yáokòng | 139 | 2 | REM | Regular | — |
| Zhanshi Yīshēng | 137 | 1 | LI | Regular | — |
| Sulsa Warriors | 1753 | 1 | SK | Regular | — |
| Yáopú Pangguling | 162 | 2 | REM | Regular | — |
| Imperial Agent, Pheasant Rank | 148 | 1 | MI | Regular | FT-01 Duo max 1 |
| Húláng Shocktroopers | 1257 | 1 | HI | Regular | FT-01 Duo max 1, exact FTO profiles only |
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
| Sù-Jiàn Immediate Action Unit | 155 | 1 | HI | Regular | FT-01 Duo max 1 |
| Zúyŏng Invincibles | 127 | 3 | HI | Regular | FT-01/FT-02 |

### Optional-mode units

| Unit | ID | Mode | Ordinary roster? | Main-chart relevance |
|---|---:|---|---|---|
| Guǐ Fēng Spec-Ops | 1914 | Spec-Ops | No | no ordinary vanilla Fireteam row in the pinned chart |
| Yu Jing Team-Ops | 1928 | Team-Ops | No | no ordinary vanilla Fireteam row |

## Unit details and vanilla profile provenance

The pinned **vanilla** Army source is authoritative for profile/loadout values. Do not substitute the same unit's Invincible Army, White Banner or Imperial Service values without checking: some shared units have faction-specific profile projections.

Until every loadout table is copied inline, use the roster ID above with the pinned Yu Jing source `n5/yu-jing/7.26246.158.json` and the matching parent-unit record under `n5/yu-jing/units/`. The following vanilla-specific/current cases are recorded explicitly because they affect list construction or Fireteam legality.

### RacerBots

**Unit ID:** 1905  
**AVA:** 2  
**Troop type:** REM  
**Structure:** yes  
**Regularity:** Regular characteristic in the parent profile

Base profile: `MOV 20-10 | CC 13 | BS 11 | PH 12 | WIP 11 | ARM 0 | BTS 3 | W 1 | S 2`.

The pinned parent-unit record exposes a single profile group with two 9-point variants. Numeric weapon/equipment IDs are retained here where the current repository lookup has not yet been normalized into display names; this is preferable to guessing from an older profile projection.

| Profile ID | Label | Points | SWC | Source distinctions |
|---:|---|---:|---:|---|
| 1 | RACERBOT Mk-I | 9 | 0 | weapon IDs `216`, `220`, `71`; base equipment IDs `246(+310)`, `241(-3)`, `113`; base skills include Remote Presence and Courage |
| 2 | RACERBOT Mk-II | 9 | 0 | weapon IDs `188`, `176`, `71`; `176` = Mine Dispenser; `71` = PARA CCW; same base profile/equipment |

### Húláng Shocktroopers — vanilla projection

**Unit ID:** 1257  
**AVA:** 1 in vanilla  
**Troop type:** HI  
**Regularity:** Regular

Base profile: `MOV 15-5 | CC 22 | BS 12 | PH 12 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`.

**Common equipment/skills:** Multispectral Visor L1, CrazyKoala; Martial Arts L3, Dodge (+5cm), Courage, Mimetism (-3), Forward Deployment (+20cm), Immunity (Shock), Stealth, No Wound Incapacitation.

| Profile ID | Label | Points | SWC | Loadout distinction | Vanilla Fireteam eligibility |
|---:|---|---:|---:|---|---|
| 1 | HÚLÁNG FTO-2 | 38 | 0.5 | SMG, E/M Grenade Launcher (+1B), Pistol, Monofilament CCW (PS=6); Minelayer | no — chart says `FTO`, not `FTO-2` |
| 2 | HÚLÁNG FTO-2 | 38 | 0 | SMG, Disco Baller, Deployable Repeater, Pistol, Monofilament CCW (PS=6) | no — chart says `FTO`, not `FTO-2` |
| 3 | HÚLÁNG FTO | 31 | 0 | Combi Rifle, E/M Grenade Launcher, Pistol, Monofilament CCW (PS=6) | yes — FT-01 Duo max 1 |
| 4 | HÚLÁNG FTO | 33 | 0 | Combi Rifle, Disco Baller, Deployable Repeater, Pistol, Monofilament CCW (PS=6) | yes — FT-01 Duo max 1 |

### Krit Kokram — vanilla projection

**Unit ID:** 1445  
**AVA:** 1  
**Troop type:** HI  
**Regularity:** Regular

Base profile: `MOV 15-5 | CC 19 | BS 13 | PH 12 | WIP 14 | ARM 3 | BTS 3 | W 2 | S 2`.

**Common equipment/skills:** Deactivator, GizmoKit; Courage, Dodge (+5cm), Engineer, NCO.

| Profile ID | Label | Points | SWC | Loadout distinction | Vanilla Fireteam eligibility |
|---:|---|---:|---:|---|---|
| 1 | KRIT KOKRAM FTO-2 | 37 | 0 | Heavy Shotgun, E/Mitter, Chain-colt, E/M Mine, Heavy Pistol (+1B), CCW; Deployable Repeater, Forward Deployment (+20cm), Minelayer | no — chart says `FTO`, not `FTO-2` |
| 2 | KRIT KOKRAM FTO | 35 | 0 | MULTI Rifle (PS=6), Chain-colt, D-Charges, Heavy Pistol (+1B), CCW | yes — FT-01 or FT-02 |
| 3 | KRIT KOKRAM FTO | 40 | 1.5 | Feuerbach, Chain-colt, D-Charges, Heavy Pistol (+1B), CCW | yes — FT-01 or FT-02 |

### Hac Tao Special Unit — vanilla projection

**Unit ID:** 131  
**AVA:** 1  
**Troop type:** HI  
**Regularity:** Regular

Base profile: `MOV 15-5 | CC 19 | BS 14 | PH 13 | WIP 14 | ARM 5 | BTS 6 | W 2 | S 2`.

**Common equipment/skills:** Multispectral Visor L1; Courage, Hidden Deployment, Mimetism (-6), Stealth.

| Profile ID | Label | Points | SWC | Loadout / role |
|---:|---|---:|---:|---|
| 4 | HAC TAO (BS Attack +1B) | 60 | 1.5 | Missile Launcher (+1B), Nanopulser, Pistol, Shock CCW (PS=6) |
| 5 | HAC TAO (Hacker, Hacking Device) | 58 | 0.5 | MULTI Rifle (PS=6), Nanopulser, Pistol, Shock CCW (PS=6); Hacking Device |
| 7 | HAC TAO (NCO) | 59 | 1.5 | HMG, Nanopulser, Pistol, Shock CCW (PS=6); NCO |

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
| Johnny Kao | 1892 | 1 | — | all vanilla profiles | May join an otherwise legal main-force Yu Jing Fireteam; does not remove chart/team requirements |

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

## Transcript-backed tactics — Vanilla Yu Jing N5 (2026-10-22)

> **Interpretive research, not Army data.** The pinned **N5.3 / 2026-09-03** vanilla Army source controls unit availability, AVA, loadouts and Fireteam eligibility. Earlier N5 discussions (mainly April–June 2025) are opinions/strategies, not proof a profile has the same equipment in 2026. This reference remains **status: partial** because full vanilla loadout projections are still outstanding. Do not transplant an identically named Imperial Service, White Banner or Invincible Army profile without checking its *vanilla* projection. Main-force and Daebak Reinforcement charts are separate.

### Identity, priorities and list-building patterns

**Practical identity:** Vanilla Yu Jing has **excellent distributed heavy infantry, cheap defence, good enough midfield/hacking support, and LT/NCO/Tactical Awareness order efficiency**. Compared with a sectorial it exchanges big Core links for freedom to combine specialized units that never share a roster elsewhere. The main risks are concentrating 200+ points in hackable bodies, lacking a non-hackable route through enemy repeaters, and paying for troops that overlap roles.

1. **Start with the mission, then the LT/order engine:** **Dāoyīng Lieutenant(+1 Order)** is a widely preferred Camo LT supporting **NCO** Mówáng/Krit/Hac Tao or another eligible spender. The hacker LT becomes an important turn-three button-pusher but avoid revealing it near enemy KHD/Pitchers merely to save one Order. **Sun Tze/Strategos** offers a distinct plan: more Regular orders, deployment control and Counterintelligence; its substantial cost and Strategos conversion of LT Orders can *compete* with conventional LT→NCO sequencing rather than automatically stack.
2. **Buy two *different* attack angles:** e.g. **Mówáng NCO Disco Baller** (mobile pressure) + **Yān Huǒ HRMC** (long anti-armour), **Hac Tao** Hidden Deployment HMG/ML (surprise/long range) + **Sù-Jiàn** (rapid close assault), or **Shàng Jí Tactical Awareness** (extra orders) + **Hǎidào/Dokkaebi** (Pitcher/KHD/mission). A Red Fury alone is not a reliable TAG killer.
3. **Choose specialist / network reach:** **Zhēnchá** Camo Infiltrator KHD/FO/Minelayer, **Guìláng** Infiltration/repeater, **Dàofěi** sturdy Infiltrating attack/specialist, **Hǎidào 22-point KHD + Pitcher**, **Dokkaebi 22-point KHD+Spotlight/Pitcher**, **Wèibīng FO/Sensor/Repeater**, and **Liú Xīng or Tiger Soldier** AD diversify the way objectives are reached. Support your guided plan with actual Spotlight tools, not just a missile launcher.
4. **Insure against an alpha strike:** Usually 1–2 **Gūdǎn one-use Camo + Zapper/HFT**, **Shaolin 5/6-point Smoke**, and/or **Libertos** Camo, **Lóng Yá** Camo Panzerfaust/Minelayer, **Chaīyì** Flashbot, **Hùsòng** TR. Put mines/templates across the likely path to your real attacker. **Kuang Shi** are no longer a compulsory N4-style order-tax package; use them *only when* a genuinely top-heavy build needs cheap Regular Orders and can tolerate Impetuous complications.
5. **Allocate 15 slots and extra orders purposefully:** Long-range gun, mobile close/mid attacker, 2–3 specialists, a protected LT/NCO route, cheap screen, and a repair/anti-hacking line. More Tactical Awareness on different troops is not identical to more interchangeable Regular Orders; ensure the extra order falls on a profile with a job that turn.
6. **Current Fireteam restrictions are important:** **Core 0; Haris 1; Duo 2 maximum.** **FT-01** is a Duo menu, **FT-02** supports Duo/Haris. **Two Zúyǒng + Dokkaebi** in FT-02 can create a Haris and increase the hacker's effectiveness; **Mówáng + Hǎidào** FT-01 trades raw link attack bonuses for move-together economy and better active angles. **Gūijiă, Blue Wolf, Sù-Jiàn, Shàng Jí** have FT-01 access *as specified*; **Lóngwáng and Fēiquán are NOT linkable** here. **Johnny Kao alone is the source-defined main Wildcard**; **Húláng vanilla FTO IDs 3/4**, **Krit Kokram vanilla FTO IDs 2/3** only. *Their FTO-2 alternatives do not satisfy vanilla Fireteam restrictions.*
7. **Do not copy the sectorial's advantages:** Vanilla does **not** have White Banner's Haetae/Dokkaebi/Jujak huge Core, ISS's broad Celestial Guard teams, or Invincible Army's high-AVA Shàng Jí/Yān Huǒ Fireteam. Its benefit is mixing **unlinked Haetae fire support, ISS TAG/vehicles and IA infiltration/HI** in one roster.

### High-value decisions: reason plus competing view

| Role / option | Why it is good | Objection / when another choice wins |
|---|---|---|
| **Dāoyīng LT(+1 Order) + NCO** | Camouflaged LT supplies **two LT Orders** into a real NCO combat plan; hacker adds WIP14 scoring/hacking later. Shepherd's recommended default starting point for most N5 vanilla lists. | LT type is predictable from WIP roll, and a revealed hacker LT risks enemy KHD. Do not reveal until there is a payoff or safe recamouflage route. |
| **Sun Tze Strategos LT** | Powerful deployment/reserve manipulation and Regular Order economy, Counterintelligence, hard-to-shift late scoring body. Tactical Awareness explicitly builds around its ability to hold multiple attack assets in reserve. | Expensive order investment; Shepherd argues Strategos and multiple NCO slots can be redundant. Use when planning *several* efficient Regular-order users, not automatically with Dāoyīng-style NCO strategy. |
| **Mówáng NCO + Hǎidào KHD/Pitcher (FT-01 Duo)** | Mówáng ARM5/Mimetism(-3)/NWI, NCO and Disco Baller survives while crossing lanes; Hǎidào adds durable specialist, short-range template pressure, Pitcher and Trinity. Move both as a combined attack/support package. Shepherd's favorite utility Duo. | Mówáng **Red Fury** has lower anti-armour ceiling than AP HMG/HRMC; Duo movement does not automatically give a Haris Special Die. If the problem is a heavy TAG, bring an additional big gun. |
| **Hac Tao HMG NCO / ML / hacker** | Hidden Deployment, Mimetism(-6), ARM5/2W, surprise and durable firepower. **NCO HMG** exploits LT orders; **Missile(+1B)** is lethal hidden ARO *and* occasional active-turn gun; hacker challenges advanced hacking/classified jobs. **Vanilla-specific** base MSV1 differs from some sibling army projections. | 58–60 points in recorded source; Shepherd likes it but often prefers multiple threats. Hac Tao hacker competes with much cheaper **Zhēnchá/Dokkaebi** for routine buttons/Trinity. |
| **Sù-Jiàn** | Remote Presence/NWI and fast transformations/movement let a strong close-range shooting/shotgun piece survive dice variance and recover with an Engineer; among the most flexible Yu Jing attack options. **It is a remote-presence HI, not a TAG or generic REM.** | Hackable and expensive relative to cheap attack pieces; can be isolated/immobilized. Shepherd particularly praises N5 Heavy Shotgun(+1B); check *current vanilla* profile and seasonal Stealth rules before using 2025 combo advice. |
| **Yān Huǒ HRMC vs Haetae AP HMG / HRL Guided** | **Yān Huǒ** BS14, HRMC, Warhorse/Immunity ARM is pure long-distance anti-armour and tough ARO; **Haetae** adds Tactical Awareness, cheaper 36-point Guided HRL or 40-point AP HMG, making a flexible independent fire-support choice. | Shepherd prefers Yān Huǒ for 5-dice HRMC durability but willingly downgrades to Haetae when points matter. **Vanilla Haetae is unlinked**, so don't assume White Banner's linked Guided Special Die applies here. |
| **Hǎidào / Dokkaebi** | **Hǎidào KHD/Pitcher** efficient ARM3+NWI short-range attack/hacker; **Dokkaebi KHD+Spotlight/Pitcher** high BTS and Remote Presence/NWI gives good network projection even without a giant sectorial link. Two differently placed Pitchers force safer enemy movement and can enable Son-Bae/Haetae Guided. | Shepherd strongly favors Hǎidào KHD over niche CoC/Engineer variants with its **AVA1**; **Tactical Awareness** argues Dokkaebi often beats pricier Zhànyīng hacker in this role. Normal Dokkaebi Hacking Device/Carbonite offers different defence than KHD/Spotlight. |
| **Zúyǒng FT-02 Haris + Dokkaebi** | Two relatively affordable 2W Zúyǒng (e.g. Tactical Awareness/TinBot, Paramedic or short-range E/M) can qualify a 3-person Haris and boost a Dokkaebi attack/Spotlight via Fireteam rules. Adds cheap durable mission coverage. | Shepherd dislikes BS13 without visual mods and finds Shàng Jí relatively overpriced in Vanilla. Tactical Awareness likes the mixed **Bìxié + two Zúyǒng** alternative and the huge order economy. Confirm *exact* Army rules for the Special Die and profile membership. |
| **Zhēnchá / Guìláng / Dàofěi** | Zhēnchá is a tough Camo infiltrating HI specialist with KHD/mines; Guìláng delivers Infiltration/MSV1 and deployable repeater; Dàofěi is a 2W Camo infiltrating HI gun/specialist. Choose cheap network/mine, durable specialist, or major forward gun to suit mission. | Shepherd considers Guìláng pricey and Dàofěi too many points outside specialized missions; WIP12's experienced **White Banner** guest Axel prizes Guìláng LT/FO/hacker for independent area/objective play, applicable tactically but **AVA/profile availability must be vanilla-checked**. |
| **Shaolin, Gūdǎn, Libertos, Kuang Shi** | Smoke+MA3/Stealth Shaolin for advancing or CC trades; Gūdǎn Zapper/HFT one-use Camo for protecting pricey HI/TAGs; Libertos low-cost disposable Camo; Kuang Shi as emergency cheap order density. | Shepherd strongly rejects automatic 4-Kuang Shi spam in N5 because it crowds 15 trooper slots. Tactical Awareness deliberately uses 4 in its **TAG-heavy** list. Both strategies work for *different* points/slot budgets; Shaolin remain Irregular unless a rule changes that. |
| **Tiger Soldier vs Liú Xīng vs Léi Gōng** | Tiger: relatively inexpensive real Combat Jump specialist; Liú Xīng: durable explosive Combat Jump HI whose very availability forces DZ security; Léi Gōng: mobile MSV1/Albedo(-6) flank or FTO anti-visor/CoC role. | AD eats points and can fail landing; Léi Gōng Parachutist is *not* a Combat Jump substitute. Choose a true backline attack, survivable HI drop, or edge-entry specialist deliberately. |
| **Shàng Jí / Húláng / Krit / Bìxié / Hwarang** | Shàng Jí AP HMG/TacAware can carry orders in an FT-01 Duo; **vanilla Húláng** FTO has **MSV1/CrazyKoala/Mimetism(-3)/FD** (different sectorial version); **Krit** NCO Engineer protects TAG/HI as the FT-01/FT-02 FTO; Bìxié/ Hwarang gives mobile melee and a flexible FT-02 Haris slot. | Shepherd skeptical about price of Shàng Jí in vanilla given other guns; Tactical Awareness finds its TacAware and small links useful. Use **vanilla FTO**, not sectorial FTO-2: Húláng 3/4, Krit 2/3. |

### TAGs, VH and REMs — cross-sectorial lessons, adjusted for vanilla

**Vanilla actually has:** **Gūijiă AVA2**, **Blue Wolf AVA1**, **Lóngwáng AVA1** TAG families; **Fēiquán AVA1 VH vehicle**; and fast **RacerBots AVA2** alongside traditional Yu Jing REMs. **Sù-Jiàn is HI with Remote Presence, not a TAG**. This is very different from White Banner (no Lóngwáng, Blue Wolf AVA2) or ISS (different TAG/vehicle restrictions). Exact *vanilla loadouts* have to be verified in the vanilla source; the parent roster membership/AVA above are canonical.

| Platform | Practical job / why | Alternative view / support warning |
|---|---|---|
| **Lóngwáng TAG** | Mid-sized police TAG mixes credible shooting, **BS Attack(-3)** defence, close-range riot/adhesive control and **Biometric Visor** tech. Tactical Awareness builds it beside Blue Wolf: Lóngwáng for longer lanes/control, Wolf for up-close AP pressure. Cross-check **Sep 2026 vanilla source** before using 2025 HMG/Mark12 claims. | Shepherd: serviceable but does not outcompete spread-out HI. Tactical Awareness: very interesting control TAG when enemies struggle against immobilization. Don't assume an ISS Fireteam; **unlinked in vanilla**. |
| **Blue Wolf TAG** | **AP Spitfire with +1B**, heavy flamethrower/Panzerfaust fork, 3W/ARM6/TacAware and Shàngdiào ancillary: exceptional mid/short-range attack volume. Can be FT-01 Duo with eligible member, unlike unlinked Lóngwáng; consider **Krit Engineer FTO** support where legal. | **Direct disagreement:** Tactical Awareness likes Blue Wolf + Lóngwáng complementary ranged bands; **Loss of Lieutenant** rates it more highly than Guijia for AP Spitfire forks and Yu Jing LoF-control support; **Irregular Order Aug 2026** prefers Guijia, arguing Blue Wolf's short effective ranges force dangerous hacking/CC exposure. |
| **Gūijiă TAG** | ARM8, MULTI HMG, Tactical Awareness, Super-Jump, MA2/DA CCW, Shàngdiào: offers long-range fire and genuine counter-CC. **Vanilla FT-01 Duo access** allows engineer/mission companions where allowed; 77-point models are still a large investment. | Shepherd: all three Vanilla TAGs are fine but usually less effective than multiple HI; Loss of Lieutenant tags it middling due to expensive CC and lack of Remote Presence compared with other TAGs; **2026 Irregular Order** prefers it over Blue Wolf due to staying farther from hackers. Use repair support rather than assuming Remote Presence. |
| **Fēiquán VH** | 27/28-point aerial **Sensor**, high mobility, **E/M Carbine + Pitcher** or **MULTI Rifle + X-Visor**, plus adhesive/Blitzen control: hard-to-ignore forward network extension and Camo detector. Tactical Awareness explicitly demonstrates it in a multi-TAG Vanilla build to disable enemy heavy pieces so TAGs can finish them. | No Cover, ARM3, 2W, and **no Vanilla FT access**. Irregular Order notes the Pitcher variant matters more where hacking range is missing (ISS) than when Vanilla already has Hǎidào/Dokkaebi/Guìláng; alternative is cheaper X-Visor gun/Sensor piece. Not a TAG. |
| **Sù-Jiàn (Remote Presence HI)** | Fast attack/late objective unit with remote-state durability and repairability; sometimes a better points-efficient close brawler than dedicating 70+ points to a TAG. **FT-01 Duo menu** allows accompanying utility specialists. | Defensive hackability remains; N5 special seasonal rules referenced in Apr 2025 videos may no longer apply. It is not a generic REM for EVO target eligibility unless the applicable rules say so. |
| **RacerBot Mk-I / Mk-II (vanilla-only recorded profile)** | **9-point Regular, MOV20-10** REM alternatives for fast objective reach, lane interference/cheap Order and **Mk-II Mine Dispenser**. In a faction with a max 15-trooper limit, two cheap fast orders leave space for premium HI/TAGs. | Vanilla projection currently records several equipment/weapon IDs numerically. **Do not invent weapon names or special abilities** pending source normalization; not in FT-01/02. |
| **Rui Shi** | **MSV2 Spitfire** for smoke attack against Mimetism, or MSV1 Red Fury + Mine Dispenser for area denial. EVO Assisted Fire/Marksmanship can increase active shooting value. Combines with Shaolin smoke and cheap screening. | **Unlinked in vanilla**, unlike IA where it can join Invincible Fireteam. ARM1/1W means it is a follow-up gun, not a durable ARO. Shepherd's list uses it as lower-budget MSV2/Hsien substitute; IRregular Order doubts its routine inclusion without program support. |
| **Lù Duān** | Holoprojector, MSV1, extra-Burst and E/M Mine/Mk12 or Thunderbolt: an inexpensive decoy/independent flanking REM to expose mines and cover a second route; useful when a main HI spends the primary group Orders. | No vanilla link; weak armour means expensive Orders can disappear instantly. Tournament commentary from IA rates it as expendable *secondary* attacker, not primary fire support. |
| **Lóng Yá** | Cheap Camo Forward Deployment **Panzerfaust(+1B), Flammenspeer(+1B), AP Mine/Minelayer** to preserve expensive troops and threaten TAGs on first contact. Baggage reload and Engineer revive are possible. | **Opposing takes:** WIP12 tournament White Banner player Axel/Irregular Order call the price and threat excellent; Shepherd says BS11 makes them weaker than emerging N5 attackers who simply tank/destroy the REM; choose according to map and local attack profiles. Unlinked in vanilla. |
| **Wèibīng / Chaīyì / Hùsòng** | Wèibīng **Sensor+FO+Repeater** opens camo and Spotlight against elusive targets; Chaīyì cheap Flash Pulse Regular Order provides repeaters; Hùsòng **TR HMG or Thunderbolt** makes covering fire lanes manageable without an expensive HI ARO. | All unlinked; overlapping positions matter more than 3 static remotes on one roof. Shepherd uses Hùsòng+Engineer/Yáozăo with EVO to add a defensive counterweight to otherwise forward attack-heavy lists. |
| **Son-Bae / Haetae Guided / Pangguling** | Son-Bae Guided missile is a separate long-range payoff for Spotlight; **Haetae Guided HRL** is an independent gun with a secondary Guided option; Pangguling **Baggage** resupplies missiles/disposables and **EVO** can help AD and Assisted Fire. | **Vanilla Son-Bae is NOT in a Fireteam**; neither is Haetae, so **no White Banner linked Guided Special Die**. Buy only the network your list can afford; some games are won faster by killing the repeater threat than by elaborate counter-hacking. |
| **Johnny Kao / Krit / Mech-Engineer / Yáozăo / Qíshì TAGCom** | Preserve 2W/3-STR investments: **Johnny Kao** is a universal Wildcard, nonhackable engineer/utility platform; **Krit NCO Engineer FTO** moves in a vanilla team; Mech-Engineer + Yáozăo handles REM/TAG repairs, Qíshì can improve TAG operation. | A combat-group split can strand TAG support where it cannot repair. Don't infer that an *Engineer* gives automatic Remote Presence to Blue Wolf/Gūijiă/Lóngwáng; confirm exact repair/re-roll options per unit and current rules. |

### Build prototypes to test (roles only; verify legality/profile IDs in Army)

- **Distributed HI / command engine:** Dāoyīng LT(+1 Order) → **Mówáng NCO + Hǎidào KHD/Pitcher Duo**, independent **Haetae AP HMG or Yān Huǒ HRMC**, 1–2 inexpensive Camo/Smoke buffers and a Camo FO/KHD specialist. **Why:** orders, two shooting bands, hacking protection and objective coverage.
- **Haris specialist network:** Dāoyīng + **Zúyǒng/Zúyǒng/Dokkaebi Haris**, a solo **Hac Tao ML or Sù-Jiàn** attack, **Wèibīng/Son-Bae** where missions reward Spotlight. **Why:** modest link bonuses and usable hacking without a Core.
- **TAG police / combined arms:** **Lóngwáng ranged-control TAG + Blue Wolf short AP gun + Fēiquán E/M/Sensor VH** alongside Sun Tze or cheaper Dāoyīng, Engineer, Gūdǎn/Zapper, Shaolin smoke. **Why:** three different problems, complementary threat ranges. **Risk:** highly hackable/expensive; Tactical Awareness explores this for fun, not as universal strongest.
- **All-camo pressure:** Dāoyīng LT, **Zhēnchá/Guìláng/Dàofěi**, **Hac Tao Hidden Deployment**, **Gūdǎn/Libertos/Lóng Yá**, a real ranged armour-cracking gun, a disposable AD threat. **Why:** reduces link dependence; forces opponent to spend Orders discovering/bypassing markers. Tactical Awareness explicitly suggests Vanilla can be better at a majority-Camo game than its sectorials.
- **Low-cost objective/repair shell:** **9-point RacerBots**, Chaīyì/Kuang Shi where required, Baggage, Engineer+Yáozăo, one premium durable HI and multiple specialist vectors. **Why:** Vanilla can finally fund expensive HI without mandatory 4-Kuang Shi tax; **verify all candidate loadouts** rather than treating this as an encoded list.

### Actual disagreements (avoid flattening them)

1. **TAGs vs HI:** Shepherd: Lóngwáng, Gūijiă and Blue Wolf are viable but usually less efficient than independent **Hac Tao / Mówáng / Sù-Jiàn / Haetae** spread around the board. Tactical Awareness: a *triple-armoured* Sun Tze/Blue Wolf/Lóngwáng/Fēiquán shell creates complementary threats, reserve deployment trickery and hacking/E/M lockdown. Take TAGs to exploit specific table/mission matchups; not because Vanilla is automatically a TAG army.
2. **Blue Wolf vs Gūijiă:** Loss of Lieutenant rates Blue Wolf's extra-Burst AP Spitfire and disposable fork strongly; newer Aug 2026 Irregular Order prefers Gūijiă's ARM8 and long MULTI HMG, which lets it spend fewer Orders in enemy hacking radius. Both views account for opponent counter-tech, but weight *attacking volume vs safe threat range* differently.
3. **Yān Huǒ vs Haetae vs Hac Tao:** HRMC for volume/high ARM insurance; Haetae TacAware to save points while preserving a big gun and occasional Guided; Hac Tao ML/HMG for hidden surprise and modifier stacking. Do not confuse the independently useful Haetae with **White Banner's linked** Haetae Guided.
4. **Linked Haris vs solo problem solvers:** Shepherd considers a two-Zúyǒng+Dokkaebi Haris a niche *Spotlight/Pitcher Special Die* method but prioritizes solo Hǎidào/Mówáng plus other independent attack angles. Tactical Awareness favors its small link/TacAware economies. In Vanilla, a link trades *flexible independent orders* for small amounts of activation economy/bonuses—not huge 5-model Core output.
5. **Automatic Kuang Shi spam?** Shepherd says no: cheap Camo/HI costs improved enough that 4 Kuang Shi waste precious 15 troop slots in many lists. Tactical Awareness still uses 4 in TAG/Sun Tze budget builds to preserve premium firepower and smoke. Context, not a universal rule.
6. **Premium infowar vs cheap network:** **Hǎidào KHD** versus **Dokkaebi KHD/HD** versus **Hac Tao hacker**. Cheap linked/unlinked pitchers generally enable more board area than paying 58 points for hidden high-armour Trinity, but the latter offers different missions, gunfighting and Hidden Deployment.
7. **Lóng Yá decline vs value:** Shepherd believes current N5 firepower makes BS11 cheap attack remotes easy to remove; White Banner tournament player Axel and Irregular Order still rate Camo, AP mines and Panzerfaust as excellent cheap order drains. Table lanes determine the winner.

### Best videos/podcasts and what was actually checked

| Source | Direct transcript findings and status |
|---|---|
| **[Robert Shepherd — Infinity N5 Faction Focus: Yu Jing](https://www.youtube.com/watch?v=mn4yHSNxsnA)** (Apr 2025) | **YouTube MCP transcript retrieved and reviewed** (existing archive: [vYujing.txt](../../rules/Youtube%20factions/vYujing.txt)). Main detailed reasoned guide: post-N4 HI economics, order engine, Hac Tao/Mówáng/Sù-Jiàn/Yān Huǒ/Haetae, heavy-weapon roles, hacking and specialist Duos, cheap defence and sample list. |
| **[Tactical Awareness S3 Ep22 — Prime Yu Jing ZEROES & HEROES](https://open.spotify.com/episode/6SExmNQGYYnzbf8vsodN0A)** (Jun 3 2025) | **Podcast MCP complete transcript read.** Three competing archetypes (Sun Tze + Blue Wolf + Lóngwáng + Fēiquán; TAG/controller hybrid; many TacAware HI/HD hackers). Unusual role-based Duos, TAG pilot, Gūdǎn, Kuang Shi, confidence in all-Camo builds. **Most faction-specific podcast** found. |
| **[Loss of Lieutenant Ep142 — N5 TAG Tier List](https://open.spotify.com/episode/1h5CJfZC5zBPxdg66o7xIN)** (Apr 2025) | **Podcast MCP transcript read.** Detailed Gūijiă vs Blue Wolf comparison, melee survival, weapon bands, discounting non-Remote Presence, debates Blue Wolf's actual relative TAG tier. Opinionated rankings, not hard stats. |
| **[Loss of Lieutenant Ep141 — Tactical Armored Gear](https://open.spotify.com/episode/6zPRTbn2cilgMyuHtODvf7)** (Mar 2025) | **Podcast MCP transcript checked** for repair and hacking defence (kill enemy hackers, range management, Engineer; don't treat a lucky Speedball as guaranteed repair). Cross-faction TAG fundamentals. |
| **[Irregular Order Ep47 — White Banner Sectorial Guide](https://open.spotify.com/episode/2w4tX9v1goAozQSh7HqGUE)** (Aug 13 2026) | **Podcast MCP transcript reviewed:** fresher contrasting **Blue Wolf vs Gūijiă**, Fēiquán VH and common Yu Jing REM comparisons; White Banner profile/FT verdicts are **not imported into Vanilla**. |
| **[Tactical Awareness S3 Ep19 — Imperial Service](https://open.spotify.com/episode/0nIc1Ub4zoXpKxb1PyTJl3)** (May 2025) | **Podcast MCP transcript checked** for **Lóngwáng** gun/control and **Fēiquán** E/M/Pitcher/Sensor, Kuang Shi and cheap defence. Vanilla has less ISS Fireteam/AVA support. |
| **[Tactical Awareness S3 Ep20 — Invincible Army](https://open.spotify.com/episode/4uGhKYeMBabBftl1gwXhpS)** (May 2025) | **Podcast MCP transcript reviewed in the connected IA guide**: Hac Tao vs Zhēnchá, Mówáng, Yān Huǒ and Rui Shi/EVO. Sectorial link bonuses don't transfer automatically. |
| **[Corvus Belli forum N5 Yu Jing tactica index](https://forum.corvusbelli.com/threads/n5-recap-yu-jing-tacticas.43474/)**; **[Bureau Aegis N5 Yu Jing resources](https://www.bureau-aegis.org/forum/index.php?topic=17848.0)** | Discovery/date cross-check only; not substitutes for the actual MCP transcripts. |

**Update rule:** Comments from early-2025 N5 may describe earlier seasonal rules, points, equipment or Fireteams. The **2026-09-03 pinned vanilla source** and current FAQ are authoritative. Do not mark this file current or complete just because tactical research was added: the full inlined vanilla loadout projection remains outstanding.


## Tactical tags

Derived analysis aids, not official characteristics. These remain deliberately broad until all vanilla loadouts are inlined.

| Unit | Tags |
|---|---|
| Gūijiă | TAG, heavy gunfighter, CC mobility |
| Blue Wolf | TAG, mobile attack, close-range pressure |
| Lóngwáng | TAG, control weapons |
| Hac Tao | hidden deployment, Mimetism (-6), heavy gunfighter/hacker/NCO |
| Dàofěi | camouflaged/infiltrating HI, midfield attacker/specialist |
| Húláng | midfield/assault HI, strong CC, vanilla Duo option through FTO profiles |
| Mówáng | durable attack HI, vanilla Duo option |
| Shàng Jí | HI, vanilla Duo option |
| Zúyŏng | efficient HI, vanilla Duo/Haris anchor |
| Sulyong | mobile MI, vanilla Duo/Haris option |
| Hwarang | aggressive HI, vanilla Duo/Haris option |
| Dokkaebi | cyber/support HI, vanilla Duo/Haris option |
| Bìxié | mobile character, vanilla Duo/Haris option |
| Krit Kokram | Engineer/NCO, vanilla Duo/Haris option through exact FTO profiles |
| Sù-Jiàn | fast durable attack piece, vanilla Duo option |
| Shaolin | smoke/CC warband, vanilla Duo option |
| Johnny Kao | main-force Wildcard |
| Gŭiláng | camouflaged infiltrating specialist |
| Zhēnchá | camouflaged infiltrating HI specialist |
| Tiger Soldier | airborne attack/specialist |
| Liú Xīng | airborne HI attack/specialist |
| RacerBot | very fast utility REM; two 9-point variants in pinned vanilla source |
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

## N5.3 airborne / backline-strike archetypes and trades (2026-10-23)

**Tiger Soldier** provides cheap true **Combat Jump/Parachutist** angles where current Vanilla roster lists it; **Liú Xīng** offers pricier durable/explosive HI drop (confirm its selected printed Combat Jump modifiers, don't infer from N4). **Hac Tao Hidden HMG/NCO** and **Guilang/Zhencha** infiltrating models attack from concealed midfield; **Sù-Jiàn** is a fast *on-table* penetrator, not a drop troop. Compare cost of one high-variance landing to stable midfield/fast breach; preserving an LT/CoC is separate from choosing the dropper. This Vanilla summary links to the official current sectorial roster for legal loadouts.

[Full N5.3 apex/value and delivery-probability tier guide](../../notes/list-building/airborne-and-enemy-dz-attackers-apex-value.md). Current roster/profile restrictions and canonical Fireteam chart above govern legal choices.

## Active-turn gunfighter cross-reference (2026-10-23)

**Active-turn shooting choices:** **Hac Tao HMG59/1.5** buys BS14, Hidden/Camo, Mimetism(-6), MSV1 and ARM5/2W to reveal into a protected first premium shot; the price means it must remove a meaningful defender, not just one cheap objective body. **Tiger Soldier/Liu Xing** is a **deployment-route alternative**, creating weak backline attacks without frontal HMG exchanges. **Dàofěi/Zhēnchá** serve near-objective skirmishing instead of another expensive long gun. [Cross-faction non-TAG/TAG tiers and attack matchups](../../notes/list-building/active-turn-gunfighters-apex-and-value.md).

## Warband cheap trading / order economy — N5.3

The **pinned Vanilla Yu Jing** roster includes **Shaolin WB Irregular+Impetuous AVA4** and **Kuang Shi Regular+Impetuous AVA4** (different from Imperial Service Kuang Shi Monitor/Fireteam economy). **Shaolin 5/6pt Chain+Smoke** gives cheap MA3/CC and vision control; **Kuang Shi6pt Chain+Explode** is cheap template/Order-body but needs correct faction-specific restriction—do not import ISS Monitor mandatory team or its AVA8 as Vanilla. **Libertos one-use Camo/FD+20** offers a safer forward template option. **Sun Tze/Daoying LT** commands and actual CoC profiles are not 5pt expendables.

[Current cross-faction warband apex/value, opponent counters, Lt/CoC packages](../../notes/list-building/warbands-and-cheap-trading-units-apex-value.md). This faction's own pinned profile and Fireteam rows control legality.

## TAG tactical cross-reference (2026-10-23)

**Blue Wolf** is the more aggressive multi-angle/close-assault deterrent, **Gūijiă** the conventional durable gun platform, **Lóngwáng** the AP HMG + Adhesive/Riotstopper control TAG with optional NCO. Choose according to the exact range/control problem: a 10-inch Berserk threat does **not** make rushing anti-TAG enemies optimal. Current vanilla Duo/roster rules govern any actual partnering, not a sectorial's link chart.

Across all factions, compare **apex power** separately from **points value**, counterplay and mission fit: [N5.3 TAG guide](../../notes/list-building/tags.md). The current unit profiles and canonical Fireteam chart above take precedence over tactical opinions.

## Vehicle (VH) tactical cross-reference (2026-10-23)

**Fēiquán AVA1:** **28/0 Pitcher + Sensor + E/M Carbine(+1B) +1 Special Die** uniquely projects repeaters from aerial angles for KHD, Oblivion, Spotlight/Guided. **27/0 X-Visor MULTI Rifle(+1B)** is a limited alternative gun. The 28pt loadout lacks **lethal weapons**: never buy it as a sole attacker. ARM3/BTS3/W2/S7/No Cover demand safe routes; compare against cheaper ground repeater networks.

See [VH apex/value tier list and matchup guide](../../notes/list-building/vehicles-vh.md). **This sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative.**

## Hacker and KHD tactical cross-reference (2026-10-23)

**Hǎidào KHD + Pitcher** and **Dokkaebi KHD + Spotlight/Pitcher** (use actual Vanilla profiles) protect key **Mówáng/Shàng Jí/Blue Wolf** hackers while expanding the network; **Dāoyīng Camouflage LT/HD** can supply protected command/hacking without revealing the Lieutenant prematurely. **Guìláng Infiltration HD** provides immediate midfield access, while **Hac Tao Hidden HD+Trinity ~58pts** has a high attack/ambush ceiling but lower *pure hacking value*. **Fēiquán 28/0 VH Pitcher** uniquely projects a repeater behind vertical terrain, but needs an actual HD/KHD payoff. **Why:** combine a **cheap KHD counterhacker + HD Oblivion/Carbonite + TinBot** instead of leaving all expensive HI hackable behind one unprotected KHD.

See the [cross-game apex/value Hacker/KHD tier guide](../../notes/list-building/hackers-and-killer-hackers.md). **The sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative; device upgrades are profile-specific.**


## Cheerleader / Order-generation tactical cross-reference (2026-10-23)

See [Cheerleaders and Order Generators — N5.3 apex, points-value and matchup guide](../../notes/list-building/cheerleaders-and-order-generators.md) for complete comparative tables and verified transcript disagreements. The **current roster above controls** legality, AVA, Training and Fireteams.

- 7pt Chaīyì — Flash/Repeater Regular REM when AVA permits; S3 footprint and fragility limit repeats.
- 6pt Kuang Shi — Regular Chain Rifle but requires the 13pt/0.5SWC Celestial Guard Monitor for its Core package; four plus Monitor cost 37pt/0.5SWC and occupy five slots.
- Zhanshi — Regular S2 line with Fireteam/decoy utility; compare actual 7pt Flashbot and specialist upgrades before choosing expensive passive profiles.
- 9pt RacerBot — mobile Regular Order with adhesive/PARA control, not simply a passive safe S2 soldier.
- Warcor — 3pt Irregular Flash Pulse distraction, not a transferable Regular Order.

**Order audit:** add up only deployed eligible **Regular** Orders in each Combat Group; special LT/Tactical, Irregular and Peripheral activations are not transferable pool Orders. Buy the cheapest protected body that supplies the *second function the list truly needs*; consider large-base DZ crowding, expensive mandatory Fireteam slots, and whether another scoring specialist beats one more cheap Order.


## ARO apex/value cross-reference (2026-10-23)

See [Best ARO Units in N5.3 — apex, cost-value, Hidden Deployment, reactive traps, opposed podcast views](../../notes/list-building/aro-units-apex-and-value.md). **Only the legal roster above** establishes options, exact costs/AVA, upgrades and Fireteam permissions in this army.

- **Hùsòng TR** — 18pt/0SWC Thunderbolt (+1B) all-arc guard (where profile legal); ideally recoverable, not a sole ARO plan
- **Son-Bae FTO ML** — launcher for a *source-chart-authorized* team, not the same as 16pt Guided missile profile
- **Kuang Shi Chain Rifle** — 6pt regular/Impetuous order plus disposable close guard, must include Monitor/Fireteam obligations
- **Chaīyì 7pt Flash/Repeater** — cheap Regular anti-approach tax and network, not premium long-lane gun
- **Ninja hidden/camo** — anti-impersonation or corridor trap if positioned near scoring; may be more valuable unrevealed for own active turn

**List test:** a strong ARO consumes enemy Orders by forcing Smoke, rerouting, poor range, discoveries or risky trades. A robust list normally prefers *serial, different* defenders—a cheap visible or marker/template screen, a covered second gate, and a preserved attack/scoring unit—rather than two adjacent visible snipers. Plan for opponent pie-slicing, AD, anti-camo, hacking and recovery; evaluate whether extra SWC is better spent on mission attackers.
