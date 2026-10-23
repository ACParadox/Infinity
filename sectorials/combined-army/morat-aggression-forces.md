---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 602
sectorial_slug: morat
sectorial_name: Morat Aggression Forces
parent_faction: Combined Army
rules_baseline: N5.3
army_source_version: "7.26246.158"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-15
coverage: "Morat Aggression Forces standard roster, AVA, profile stats and points/SWC, canonical Fireteam chart and reverse access index, optional Spec-Ops/Team-Ops hooks, and the separate Exrah Comissariat Reinforcement Fireteam chart."
---

# Morat Aggression Forces

## Overview and provenance

Repository-native reference for the **Morat Aggression Forces (MAF)** roster, profile stats, points/SWC, AVA, canonical Fireteams, and linked Reinforcements in the pinned N5 Army source.

Sources used:

- Army-derived Morat source revision `7.26246.158` from `massayoshi/infinity-army-backup` commit `d4329bb596ffea5d568eb2435f74366c305a7630`.
- InfinityDB Fireteam normalization/semantics at commit `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: N5.3 + N5 FAQ v0.1.

Coverage notes:

- Covers the **35-unit standard Morat roster** in the pinned Army source.
- `TREITAK SPEC-OPS` and `MORAT TEAM-OPS` are optional game-mode content and are listed separately rather than counted in the 35 standard entries.
- Generic Soldier of Fortune / `merc-*` catalogue entries with empty faction lists are excluded from the standard roster.
- Krakot Renegades are included because the ordinary Krakot entry explicitly lists Morat faction ID `602` and is part of the canonical Morat roster.
- Fireteam legality comes from the canonical Army chart, not from an `FTO` profile label alone.
- `DARTOK FTO`, `RINDAK FTO`, and `OZNAT FTO` are profile-restricted Fireteam entries. Their ordinary non-FTO profiles do not inherit that access.
- Multiple `required: true` entries in the same mixed Fireteam are preserved as a **required-choice set**, not interpreted as requiring every marked troop simultaneously.
- Army `spec.DUO = 256` is treated as **unlimited Duos**.
- Tarlok Fireteams have a source-level special note: **all members are considered to possess Terrain (Jungle)** while in that Fireteam.
- Linked Reinforcement army ID `699` is **The Exrah Comissariat**. Its Fireteam chart is recorded separately and is not merged into standard Morat Fireteams.

## Sectorial summary

| Field | Value |
|---|---|
| Sectorial | Morat Aggression Forces |
| Army ID | 602 |
| Army slug | `morat` |
| Parent faction | Combined Army, ID `601` |
| Discontinued | No |
| Rules baseline | N5.3 + FAQ v0.1 |
| Standard roster units | 35 |
| Optional-mode units | Treitak Spec-Ops; Morat Team-Ops |
| Reinforcement roster | The Exrah Comissariat, Army ID `699` |
| Fireteam limits | Core 1; Haris 2; Duo unlimited |

## Standard roster index

| Unit | ID | AVA | Type | Order / structure | Fireteam access |
|---|---:|---:|---|---|---|
| Kurgat Regiment of Assault Engineers | 517 | 3 | MI | Regular | Morat foundation, max 3 |
| Krakot Renegades, Morat Fugitives | 756 | 3 | LI | Regular + Impetuous | Rodok foundation, max 2 |
| Bultrak, Mobile Armored Regiment | 1577 | 2 | TAG | Regular + Tactical Awareness | Armored Duo foundation, max 2 |
| Q-Drones | 509 | 1 | REM | Regular | — |
| Sogarat Tempest Regiment | 522 | 3 | HI | Regular | Armored Duo foundation, max 2 |
| Dāturazi Witch-Soldiers | 504 | 5 | WB | Regular + Impetuous | Dāturazi Core/Haris/Duo |
| Zerat Special Missions Regiment | 525 | 3 | SK | Regular | — |
| Raktorak, Morat Sergeant Major | 529 | 2 | MI | Regular | Wildcard max 2; counts as Morat |
| Dropsuit Taryot | 1528 | 3 | REM | Regular | — |
| T-Drones | 510 | 1 | REM | Regular | — |
| R-Drones | 511 | 1 | REM | Regular | — |
| The Hungries: Gakis | 505 | 4 | WB | Irregular + Impetuous | Hungries Core/Haris |
| Yaogat Strike Infantry | 518 | 5 | MI | Regular | Morat + Tarlok foundation |
| Rasyat Diplomatic Division | 519 | 3 | MI | Regular | — |
| Rindak Emergency Brigade | 1575 | 2 | HI | Regular | **FTO profile only**, Morat max 2 |
| E-Drones | 741 | 1 | REM | Regular | — |
| Rodok, Morat Armed Imposition Detachment | 497 | 5 | MI | Regular | Rodok foundation, max 3 |
| Treitak Anyat | 536 | 1 | LI | Regular | Wildcard max 1; counts as Morat |
| The Hungries: Pretas | 506 | 4 | WB | Irregular + Impetuous | Hungries Core/Haris |
| Kornak Gazarot, Superior Warrior-Officer | 534 | 1 | MI | Regular; Lieutenant options | Wildcard max 1; counts as Morat |
| Zabuk, Morat Enslavers | 1576 | 1 | LI | Regular | Morat max 1; counts as Morat |
| Faredak, MAF TAG Support Pilots | 1858 | 1 | LI | Regular | Morat max 1 |
| Tyrok Hunters | 1571 | 2 | SK | Regular | — |
| M-Drones | 508 | 1 | REM | Regular | — |
| Slave Drones | 526 | 2 | REM | Peripheral | — |
| Morat Vanguard Infantry | 492 | TOTAL | LI | Regular | Morat + Tarlok foundation |
| Suryat Assault Heavy Infantry | 530 | 5 | HI | Regular; TacAware/Lt options | Morat + Tarlok foundation |
| Kyosot Killing Platoon | 1574 | 2 | MI | Regular | Morat max 2 |
| Oznat, Morat Hunting Regiment | 531 | 2 | WB | Regular + Impetuous | **FTO profiles only**, Hungries |
| Med-Tech Obsidon Medchanoids | 507 | 1 | LI | Regular | — |
| Ikadron Batroid | 532 | 2 | REM | Regular | — |
| Glyph Warcors, Ur Hegemony Journalists | 1873 | 1 | LI | Irregular | — |
| Dartok Cybercombat Team | 1572 | 2 | LI | Regular | **FTO profile only**, Morat + Tarlok |
| Kaitok Shock Regiment | 1573 | 3 | HI | Regular | Morat + Tarlok foundation |
| Raicho Armored Brigade | 499 | 2 | TAG | Regular + Tactical Awareness | Armored Duo foundation, max 2 |

## Optional game-mode units

| Unit | ID | Role / note |
|---|---:|---|
| Treitak Spec-Ops | 1919 | Infinity Spec-Ops; excluded from standard matched-play roster count |
| Morat Team-Ops | 1933 | Team-Ops package; optional chart row in Morat Fireteams, max 1 when enabled |

## Profile reference

The lines below preserve the pinned Morat profile stats and all standard option costs/SWC. Weapon text is abbreviated where the profile's tactical identity is more useful than reproducing the entire Army serialization.

### Kurgat Regiment of Assault Engineers

**ID 517 · AVA 3 · MI** — `MOV 10-10 | CC 18 | BS 12 | PH 12 | WIP 13 | ARM 2 | BTS 6 | W 1 | S 2`. Engineer; Warhorse; Religious Troop.

| Pts | SWC | Profile summary | FT |
|---:|---:|---|---|
| 30 | 1 | Portable Autocannon, D-Charges | Morat foundation |
| 19 | 0 | Boarding Shotgun, D-Charges, Drop Bears | same |
| 22 | 0 | Boarding Shotgun, AP Mine, Armed Turret | same |
| 19 | 0 | Boarding Shotgun utility profile | same |
| 25 | 0 | Engineer specialist / marksman package | same |

### Krakot Renegades, Morat Fugitives

**ID 756 · AVA 3 · LI** — `MOV 15-5 | CC 23 | BS 11 | PH 13 | WIP 12 | ARM 1 | BTS 0 | W 1 | S 2`. Regular + Impetuous; Berserk, MetaChemistry and aggressive mobility package.

**Options:** `14/0`, `16/0`, `17/0`, `24/1` (Red Fury). **FT:** Rodok required-choice foundation, max 2.

### Bultrak, Mobile Armored Regiment

**ID 1577 · AVA 2 · TAG** — `MOV 15-10 | CC 21 | BS 13 | PH 15 | WIP 12 | ARM 5 | BTS 6 | W 3 | S 7`. Tactical Awareness; Rakdron ancillary remote.

| Pts | SWC | Profile summary | FT |
|---:|---:|---|---|
| 69 | 1.5 | Hyper-Rapid Magnetic Cannon | Armored Duo foundation |
| 69 | 1.5 | Portable Autocannon (+1B) | Armored Duo foundation |

### Q-Drones

**ID 509 · AVA 1 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Remote Presence, Total Reaction.

**Options:** HMG `25/1`; Plasma Rifle `24/1`; Thunderbolt (+1B) `20/0.5`. No standard Fireteam access.

### Sogarat Tempest Regiment

**ID 522 · AVA 3 · HI** — `MOV 10-10 | CC 21 | BS 13 | PH 14 | WIP 13 | ARM 6 | BTS 6 | W 2 | S 5`.

**Options:** `52/1.5`, `56/1.5`, `54/1.5` NCO, `58/1.5` NCO, `56/1` Lieutenant, `56/0.5` Lieutenant. Heavy-gun profiles include AP HMG / Feuerbach families. **FT:** Armored Duo foundation, max 2.

### Dāturazi Witch-Soldiers

**ID 504 · AVA 5 · WB** — `MOV 10-10 | CC 23 | BS 11 | PH 14 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Regular + Impetuous; smoke and strong close combat.

**Options:** `14/0`, `15/0`, `18/0.5`. **FT:** dedicated Dāturazi Core/Haris/Duo, 1–5.

### Zerat Special Missions Regiment

**ID 525 · AVA 3 · SK** — `MOV 10-10 | CC 16 | BS 11 | PH 12 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Infiltration/midfield specialist family.

**Options:** `28/0`, `29/1`, `29/0.5`, `27/0`, `22/0`, `25/0`. No standard Fireteam access.

### Raktorak, Morat Sergeant Major

**ID 529 · AVA 2 · MI** — `MOV 10-10 | CC 17 | BS 12 | PH 12 | WIP 13 | ARM 2 | BTS 6 | W 1 | S 2`. Number 2; Combat Instinct; NCO.

**Options:** `23/0`, `25/0` Chain of Command, `27/1` Red Fury, `23/0`. **FT:** Wildcard max 2, counts as Morat.

### Dropsuit Taryot

**ID 1528 · AVA 3 · REM** — `MOV 15-5 | CC 15 | BS 11 | PH 12 | WIP 13 | ARM 1 | BTS 6 | W 1 | S 2`. Airborne/jet-propulsion attack remote.

**Options:** `18/0`, `16/0`, `18/0`. No standard Fireteam access.

### T-Drones

**ID 510 · AVA 1 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Missile Launcher, Guided.

**Option:** `16/1.5`. No standard Fireteam access.

### R-Drones

**ID 511 · AVA 1 · REM** — `MOV 15-15 | CC 13 | BS 8 | PH 11 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Repeater / Flash Pulse support.

**Option:** `7/0`. No standard Fireteam access.

### The Hungries: Gakis

**ID 505 · AVA 4 · WB** — `MOV 15-15 | CC 20 | BS 9 | PH 14 | WIP 12 | ARM 0 | BTS 0 | W 1 | S 2`. Irregular + Impetuous.

**Option:** `4/0`. **FT:** Hungries Core/Haris with Oznat FTO.

### Yaogat Strike Infantry

**ID 518 · AVA 5 · MI** — `MOV 10-10 | CC 16 | BS 12 | PH 12 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`. MSV2.

**Options:** `24/0`, `21/0`, `32/1.5` MULTI Sniper, `29/1.5` Spitfire, `29/0.5` Hacker, `24/0` Lieutenant. **FT:** Morat and Tarlok foundation.

### Rasyat Diplomatic Division

**ID 519 · AVA 3 · MI** — `MOV 10-10 | CC 21 | BS 12 | PH 13 | WIP 13 | ARM 2 | BTS 0 | W 1 | S 2`. Combat Jump / Parachutist; Eclipse access.

**Options:** `25/0`, `34/1.5` Spitfire, `31/0`. No standard Fireteam access.

### Rindak Emergency Brigade

**ID 1575 · AVA 2 · HI** — `MOV 15-5 | CC 16 | BS 12 | PH 13 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`.

| Pts | SWC | Profile summary | FT |
|---:|---:|---|---|
| 24 | 0 | **RINDAK FTO**, Paramedic / Flash / adhesive package | **Morat max2; FTO only** |
| 32 | 0 | ordinary Rindak | — |
| 33 | 0 | ordinary Rindak | — |
| 26 | 0 | ordinary Rindak | — |
| 32 | 0.5 | ordinary Rindak | — |

### E-Drones

**ID 741 · AVA 1 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. EVO Hacking Device.

**Option:** `17/0.5`. No standard Fireteam access.

### Rodok, Morat Armed Imposition Detachment

**ID 497 · AVA 5 · MI** — `MOV 10-10 | CC 17 | BS 12 | PH 12 | WIP 13 | ARM 3 | BTS 6 | W 1 | S 2`.

**Options:** `29/1.5` Missile Launcher, `23/0` Thunderbolt, `24/0`, `24/0` Hacker, `21/0` Paramedic, `29/1.5` Spitfire. **FT:** Rodok required-choice foundation, max 3.

### Treitak Anyat

**ID 536 · AVA 1 · LI** — `MOV 10-10 | CC 19 | BS 12 | PH 12 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`.

**Option:** `22/0` — K1 Combi Rifle, Chain-colt, Smoke Grenades, E/M Grenades. **FT:** Wildcard max 1, counts as Morat.

### The Hungries: Pretas

**ID 506 · AVA 4 · WB** — `MOV 15-15 | CC 20 | BS 9 | PH 14 | WIP 12 | ARM 0 | BTS 0 | W 1 | S 2`. Irregular + Impetuous.

**Option:** `7/0`. **FT:** Hungries Core/Haris with Oznat FTO.

### Kornak Gazarot, Superior Warrior-Officer

**ID 534 · AVA 1 · MI** — `MOV 10-10 | CC 22 | BS 14 | PH 13 | WIP 14 | ARM 3 | BTS 9 | W 1 | S 2`. NWI; command profiles.

**Options:** `35/0`; `38/0` Lieutenant; `42/0` Lieutenant with +1 Order. **FT:** Wildcard max 1, counts as Morat.

### Zabuk, Morat Enslavers

**ID 1576 · AVA 1 · LI** — `MOV 10-10 | CC 19 | BS 11 | PH 12 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`.

**Options:** `14/0`, `14/0`. **FT:** Morat max 1, counts as Morat.

### Faredak, Morat Aggression Forces TAG Support Pilots

**ID 1858 · AVA 1 · LI** — `MOV 10-10 | CC 17 | BS 12 | PH 12 | WIP 12 | ARM 0 | BTS 0 | W 1 | S 2`. TAGCom.

| Pts | SWC | Profile | FT |
|---:|---:|---|---|
| 14 | 0 | Raicho Pilot | Morat max1 |
| 14 | 0 | Bultrak Pilot | Morat max1 |

### Tyrok Hunters

**ID 1571 · AVA 2 · SK** — `MOV 10-10 | CC 23 | BS 11 | PH 14 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Midfield hunter; optional Skurgot peripheral.

**Options:** `22/0`, `23/0.5`, `26/0` with Skurgot. No standard Fireteam access.

### M-Drones

**ID 508 · AVA 1 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Repeater, Sensor, Forward Observer, Triangulated Fire.

**Options:** `15/0`; `18/0` with Tactical Awareness. No standard Fireteam access.

### Slave Drones

**ID 526 · AVA 2 · REM / Peripheral** — `MOV 15-10 | CC 11 | BS 8 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 1`.

**Option:** `3/0`. Servant peripheral; no Fireteam access.

### Morat Vanguard Infantry

**ID 492 · AVA TOTAL · LI** — `MOV 10-10 | CC 15 | BS 11 | PH 12 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`.

**Options:** `14/0` Combi; `23/1` HMG; `17/1` K1 Sniper; `19/1.5` Missile Launcher; `15/0` Forward Observer; `16/0` Paramedic; `16/0` Commlink (+1) Specialist; `14/0` Lieutenant. **FT:** Morat + Tarlok foundation.

### Suryat Assault Heavy Infantry

**ID 530 · AVA 5 · HI** — `MOV 10-10 | CC 17 | BS 13 | PH 13 | WIP 13 | ARM 4 | BTS 6 | W 2 | S 2`.

**Options:** `34/0`, `36/0`, `36/1.5`, `43/1.5` HMG Tactical Awareness, `44/1.5` HMG Tactical Awareness + TinBot, `45/1.5` Lieutenant + HMG/TinBot. **FT:** Morat + Tarlok foundation.

### Kyosot Killing Platoon

**ID 1574 · AVA 2 · MI** — `MOV 10-10 | CC 19 | BS 13 | PH 12 | WIP 13 | ARM 3 | BTS 6 | W 1 | S 2`.

**Options:** `31/0`, `23/0`, `28/0`. **FT:** Morat max 2.

### Oznat, Morat Hunting Regiment

**ID 531 · AVA 2 · WB** — `MOV 15-10 | CC 21 | BS 11 | PH 13 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Regular + Impetuous.

| Pts | SWC | Profile summary | FT |
|---:|---:|---|---|
| 15 | 0 | **OZNAT FTO** | **Hungries; FTO only** |
| 17 | 0 | **OZNAT FTO**, Vulkan Shotgun / smoke package | **Hungries; FTO only** |
| 25 | 0 | ordinary Oznat + synchronized Preta | — |

### Med-Tech Obsidon Medchanoids

**ID 507 · AVA 1 · LI** — `MOV 15-10 | CC 16 | BS 11 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 3`. Doctor + Engineer.

**Options:** `21/0`, `22/0`, `24/0`, `25/0`. No standard Fireteam access.

### Ikadron Batroid

**ID 532 · AVA 2 · REM** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 6 | W 1 | S 2`. Baggage, Repeater.

**Option:** `11/0`. No standard Fireteam access.

### Glyph Warcors, Ur Hegemony Journalists

**ID 1873 · AVA 1 · LI** — `MOV 10-10 | CC 11 | BS 9 | PH 11 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Irregular Journalist.

**Options:** `4/0`, `4/0`. No standard Fireteam access.

### Dartok Cybercombat Team

**ID 1572 · AVA 2 · LI** — `MOV 10-10 | CC 15 | BS 11 | PH 12 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`.

| Pts | SWC | Profile summary | FT |
|---:|---:|---|---|
| 18 | 0.5 | **DARTOK FTO**, SMG, Pitcher, E/M Grenades; Hacker | **Morat + Tarlok; FTO only** |
| 23 | 0.5 | ordinary Dartok, Combi/Pitcher/Cybermine hacker | — |

### Kaitok Shock Regiment

**ID 1573 · AVA 3 · HI** — `MOV 15-5 | CC 16 | BS 12 | PH 14 | WIP 13 | ARM 5 | BTS 3 | W 2 | S 5`.

**Options:** `19/0` Chain Rifle / Flammenspeer; `20/1.5` Heavy Rocket Launcher; `34/1.5` Feuerbach + TinBot. **FT:** Morat + Tarlok foundation.

### Raicho Armored Brigade

**ID 499 · AVA 2 · TAG** — `MOV 15-10 | CC 17 | BS 14 | PH 16 | WIP 12 | ARM 8 | BTS 6 | W 3 | S 7`. Tactical Awareness; Rakdron ancillary remote.

| Pts | SWC | Profile summary | FT |
|---:|---:|---|---|
| 85 | 1.5 | MULTI HMG, Heavy Shotgun (+1B), Mine Dispenser | Armored Duo foundation |
| 75 | 2 | MULTI HMG, Heavy Flamethrower; NCO | Armored Duo foundation |

## Canonical Fireteam chart

### Global limits

| Type | Limit |
|---|---:|
| Core | 1 |
| Haris | 2 |
| Duo | Unlimited (`256` sentinel in Army source) |

### Morat Fireteams

**Types:** Duo, Haris, Core

| Entry | Min | Max | Required / note |
|---|---:|---:|---|
| MORAT VANGUARD | 0 | 5 | `required: true`; counts as Morat |
| KURGAT | 0 | 3 | `required: true`; counts as Morat |
| YAOGAT | 0 | 5 | `required: true`; counts as Morat |
| SURYAT | 0 | 5 | `required: true`; counts as Morat |
| KAITOK | 0 | 3 | `required: true`; counts as Morat |
| DARTOK FTO | 0 | 2 | counts as Morat; **FTO profile only** |
| RINDAK FTO | 0 | 2 | **FTO profile only** |
| KYOSOT | 0 | 2 | — |
| ZABUK | 0 | 1 | counts as Morat |
| FAREDAK | 0 | 1 | — |
| Morat Team-Ops | 0 | 1 | Spec-Ops / optional mode only |

**Required-choice interpretation:** Vanguard, Kurgat, Yaogat, Suryat, and Kaitok are the chart's five marked foundation alternatives. They are treated as a required-choice set, not as a requirement to include all five troop types.

### Tarlok Fireteams

**Types:** Duo, Haris, Core

> Source rule: all members of a Tarlok Fireteam are considered to possess **Terrain (Jungle)**.

| Entry | Min | Max | Required / note |
|---|---:|---:|---|
| MORAT VANGUARD | 0 | 5 | `required: true`; counts as Tarlok |
| YAOGAT | 0 | 5 | `required: true`; counts as Tarlok |
| SURYAT | 0 | 5 | `required: true`; counts as Tarlok |
| KAITOK | 0 | 3 | `required: true`; counts as Tarlok |
| DARTOK FTO | 0 | 2 | counts as Tarlok; **FTO profile only** |

**Required-choice interpretation:** Vanguard, Yaogat, Suryat, and Kaitok are the marked Tarlok foundation alternatives.

### Rodoks Fireteams

**Types:** Duo, Haris

| Entry | Min | Max | Required / note |
|---|---:|---:|---|
| RODOK | 0 | 3 | `required: true` |
| KRAKOT RENEGADE | 0 | 2 | `required: true` |

The two marked entries are preserved as a required-choice set.

### Dāturazi Fireteams

**Types:** Duo, Haris, Core

| Entry | Min | Max | Note |
|---|---:|---:|---|
| DĀTURAZI | 1 | 5 | Dedicated Fireteam |

### Hungries Fireteams

**Types:** Haris, Core

| Entry | Min | Max | Note |
|---|---:|---:|---|
| OZNAT FTO | 1 | 2 | **FTO profiles only**; anchor |
| GAKI | 0 | 4 | — |
| PRETA | 0 | 4 | — |

The ordinary Oznat profile with synchronized Preta is not an `OZNAT FTO` profile and does not receive this Fireteam access.

### Morat Armored Fireteams

**Type:** Duo

| Entry | Min | Max | Required / note |
|---|---:|---:|---|
| RAICHO | 0 | 2 | `required: true` |
| BULTRAK | 0 | 2 | `required: true` |
| SOGARAT | 0 | 2 | `required: true` |

The three marked armored entries form a required-choice set.

### Wildcards

| Entry | Min | Max | Counts as / note |
|---|---:|---:|---|
| RAKTORAK | 0 | 2 | Morat |
| KORNAK | 0 | 1 | Morat |
| ANYAT | 0 | 1 | Morat |

## Reverse Fireteam access index

| Troop / profile | Pool | Types | Max | Notes |
|---|---|---|---:|---|
| Morat Vanguard | Morat / Tarlok | Core, Haris, Duo | 5 | Required-choice foundation in both |
| Kurgat | Morat | Core, Haris, Duo | 3 | Required-choice foundation |
| Yaogat | Morat / Tarlok | Core, Haris, Duo | 5 | Required-choice foundation |
| Suryat | Morat / Tarlok | Core, Haris, Duo | 5 | Required-choice foundation |
| Kaitok | Morat / Tarlok | Core, Haris, Duo | 3 | Required-choice foundation |
| Dartok FTO | Morat / Tarlok | Core, Haris, Duo | 2 | **FTO profile only** |
| Rindak FTO | Morat | Core, Haris, Duo | 2 | **FTO profile only** |
| Kyosot | Morat | Core, Haris, Duo | 2 | — |
| Zabuk | Morat | Core, Haris, Duo | 1 | Counts as Morat |
| Faredak | Morat | Core, Haris, Duo | 1 | — |
| Rodok | Rodoks | Haris, Duo | 3 | Required-choice foundation |
| Krakot Renegade | Rodoks | Haris, Duo | 2 | Required-choice foundation |
| Dāturazi | Dāturazi | Core, Haris, Duo | 5 | Min 1 |
| Oznat FTO | Hungries | Core, Haris | 2 | **FTO profile only; min 1** |
| Gaki | Hungries | Core, Haris | 4 | — |
| Preta | Hungries | Core, Haris | 4 | — |
| Raicho | Armored | Duo | 2 | Required-choice foundation |
| Bultrak | Armored | Duo | 2 | Required-choice foundation |
| Sogarat | Armored | Duo | 2 | Required-choice foundation |
| Raktorak | Wildcard | Any legal standard Morat Fireteam | 2 | Counts as Morat |
| Kornak | Wildcard | Any legal standard Morat Fireteam | 1 | Counts as Morat |
| Anyat | Wildcard | Any legal standard Morat Fireteam | 1 | Counts as Morat |
| Morat Team-Ops | Morat | Core, Haris, Duo | 1 | Optional mode only |

All standard roster entries absent from this reverse index have no Fireteam access in the pinned Morat chart.

## Reinforcement Fireteams — The Exrah Comissariat

Linked Reinforcement army: **The Exrah Comissariat (Army ID 699)**, source revision `7.26246.158`.

The Reinforcement source exposes global `fireteamChart.spec` values of **Core 0; Haris 0; Duo 0**, while its team rows explicitly declare Fireteam types. Both facts are preserved rather than inventing non-zero global caps.

### Reinforcement roster index

| Unit | ID |
|---|---:|
| Reinf. Nexus Operatives | 1619 |
| Reinf. WCD Base Operators | 1614 |
| Reinf. T-Drones | 1623 |
| Reinf. Q-Drones | 1622 |
| Reinf. M-Drones | 1621 |
| Reinf. WCD Void Operators | 1613 |
| Reinf. EXOs, Exrah Executive Officers | 1615 |
| Reinf. Caskuda | 1618 |
| Reinf. Umbra Legates | 1620 |
| Reinf. WCD Vector Operators | 1612 |
| Reinf. Special Operative Ko Dali | 1616 |
| Reinf. Slave Drones | 1617 |

### Void Reinforcement Fireteams

**Types explicitly listed by Army:** Duo, Haris

| Entry | Min | Max |
|---|---:|---:|
| VOID OPERATOR REINF | 1 | 3 |
| VECTOR REINF. | 0 | 1 |
| NEXUS REINF | 0 | 1 |

### Base Reinforcement Fireteams

**Types explicitly listed by Army:** Duo, Haris, Core

| Entry | Min | Max |
|---|---:|---:|
| BASE OPERATORS REINF | 1 | 5 |
| VOID OPERATOR REINF | 0 | 2 |
| NEXUS REINF | 0 | 1 |

### Caskuda Fireteam

**Type explicitly listed by Army:** Duo

| Entry | Min | Max |
|---|---:|---:|
| CASKUDA REINF | 1 | 1 |
| BASE OPERATORS REINF | 0 | 1 |

### Reinforcement Wildcards

| Entry | Max | Counts as / note |
|---|---:|---|
| EXO REINF | 1 | Base Operator / Void Operator |
| M-DRONE REINF | 2 | — |
| KO DALI REINF | 1 | — |

## Validation notes

- Standard roster count reconciled to **35** ordinary Morat entries after excluding optional `TREITAK SPEC-OPS`, optional `MORAT TEAM-OPS`, and generic empty-faction `merc-*` catalogue entries.
- Morat Army metadata is current and not marked discontinued in the pinned source.
- Global Fireteam limits reconcile to **Core 1 / Haris 2 / Duo unlimited** (`256`).
- The full standard chart is represented: Morat, Tarlok, Rodoks, Dāturazi, Hungries, Morat Armored, and Wildcards.
- Multiple `required: true` rows in Morat, Tarlok, Rodoks, and Armored teams are preserved as required-choice sets rather than incorrectly made cumulative.
- `DARTOK FTO`, `RINDAK FTO`, and `OZNAT FTO` access is profile-specific. Ordinary profiles of those units are not granted that access.
- Tarlok's Terrain (Jungle) team rule is preserved verbatim in meaning.
- Raktorak, Kornak, and Anyat are the canonical standard Wildcards and retain their Morat counts-as labels.
- Linked Reinforcement army resolves to **The Exrah Comissariat (699)**. Its chart is kept separate, including the source combination of global `spec` 0/0/0 and explicitly typed Fireteam rows.
- Source data and Fireteam normalization were rechecked on **2026-10-15** against the pinned Army snapshot and InfinityDB commit listed in the front matter.

## TAG tactical cross-reference (2026-10-23)

**Raicho (75 NCO HFT / 85 Mine Dispenser)** is the durable ARM8 MULTI HMG attacker; NCO turns available LT Orders into attacks. **Bultrak (69)** offers HRMC/autocannon and an Armored Duo option but is only ARM5: don't treat it as equally durable. Evaluate the two full Duo builds and keep Engineer/second scoring routes. In an anti-armor meta, cheaper Bultrak is not automatically safer.

Across all factions, compare **apex power** separately from **points value**, counterplay and mission fit: [N5.3 TAG guide](../../notes/list-building/tags.md). The current unit profiles and canonical Fireteam chart above take precedence over tactical opinions.
