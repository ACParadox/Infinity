---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 1103
sectorial_slug: oban
sectorial_name: Ōban
parent_faction: JSA
rules_baseline: N5.3
army_source_version: "7.26246.159"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-16
coverage: "Complete standard Ōban roster, standard loadouts/profile states and peripherals, canonical Fireteam chart, exact FTO/counts-as restrictions, reverse Fireteam access, optional-mode hooks, roster identity relations, and Reinforcements boundary. Generic Soldier of Fortune catalog entries are excluded."
---

# Ōban — N5.3 sectorial reference

## Overview and provenance
**Tactical companion:** [Ōban list-building, transcript-backed opposing opinions and TAG/REM/VH comparison](../../notes/factions/oban.md) (research updated 2026-10-23). Tactical evaluations are community commentary; **the Army profiles and Fireteam chart below remain canonical**.


This file is the repository reference for **Ōban** (Army sectorial ID `1103`), a sectorial of the **Japanese Secessionist Army / JSA** (parent Army ID `1101`). It is intended to be sufficient for ordinary roster, AVA, points/SWC, profile, dependency, and Fireteam-legality questions without reopening Army.

Primary data source:

- Corvus Belli Army data snapshot mirrored by `massayoshi/infinity-army-backup`.
- Pinned source commit: `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b` (`army: N5.3 + ITS18`).
- Army dataset: `n5/oban/7.26246.159.json`.
- Source blob: `ba108bd66ab38ff701f2aa823897e225ef0984d8`.
- Army version: **7.26246.159**.
- Sectorial ID: **1103**.
- Parent JSA ID: **1101**.
- Reinforcements list ID exposed by the dataset: **1199**.
- Cross-check/reference model commit: InfinityDB `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: **N5.3 + N5 FAQ v0.1**.

Version-selection note: the backup directory also contains `7.2668.375.json`, but that file was committed **2026-03-09** (`army: N5 ITS v1.0.2`). The selected `7.26246.159.json` was committed **2026-09-03** and is therefore the later N5.3 snapshot despite lexicographic filename ordering.

Coverage policy:

- The **35 standard logical roster records** whose faction availability includes Ōban are included below.
- Generic Soldier-of-Fortune catalog records present in the aggregate payload with `factions: []` are excluded.
- **Kaizoku Spec-Ops** and **JSA Team-Ops** are optional-mode hooks, not ordinary matched-play roster entries.
- Reinforcements (`army_id: 1199`) remain distinct from the normal Ōban roster and Fireteam chart.
- Composite states and Peripherals stay under their parent logical unit rather than being counted as separate roster entries.
- Fireteam legality comes from the canonical chart below, not from an `FTO` label alone.
- Where Army marks multiple entries `required: true`, this file follows repository convention and treats those entries as a **required source-choice set** unless the chart specifies otherwise.

## Sectorial summary

| Field | Value |
|---|---|
| Sectorial | Ōban |
| Parent faction | Japanese Secessionist Army / JSA |
| Army ID | 1103 |
| Rules baseline | N5.3 + N5 FAQ v0.1 |
| Army source | 7.26246.159 |
| Standard logical roster records | 35 |
| Optional-mode records | 2 |
| Reinforcement roster | yes — Army ID 1199 |
| Fireteam chart | yes |

## Fireteam limits and interpretation

| Constraint | Value / wording |
|---|---|
| Core | up to 1 Core |
| Haris | up to 1 Haris |
| Duo | effectively unlimited (`256` in Army source) |
| Fireteam families | Keisotsu; Domaru; Ōban; Banzai; Aragoto |
| Wildcards | Kempeitai; Yuriko Oda FTO |
| Main/Reinforcement mixing | Keep normal Ōban and Reinforcement charts distinct |

Important profile-level restrictions and equivalences:

- **Yuriko Oda Wildcard access is `YURIKO ODA FTO`**: only options `1` and `2`. Option `3` is not FTO and is not a Wildcard.
- **Miyamoto Mushashi access in Banzai Fireteams is FTO-only**: option `2` only. It counts as **Tankō** in that Fireteam. Option `1` is not Fireteam legal.
- **Kempeitai** are unrestricted Wildcards and count as **Keisotsu**.
- **Oyama** counts as **Domaru** in Domaru and Ōban Fireteams.
- **Tankō** count as **Domaru** in Domaru Fireteams.
- **Kuroshi Rider** counts as **Aragoto** in Aragoto Fireteams.
- The `PANGGULING FTO` profile has no row in the Ōban Fireteam chart; its FTO name alone does **not** grant Fireteam access.
- The Ōban-family source rows for **Domaru, Karakuri, and Shikami** are all marked `required: true`. Under repository required-choice semantics, a legal Ōban Fireteam must contain at least one member from that source set; it does not require one of each.

## Standard roster index

| Unit ID | Unit | AVA | Type | Classification | Regularity | Fireteam access / notes |
|---:|---|---:|---|---|---|---|
| 158 | Tokusetsu Butai | 2 | LI | Support Troops | Regular | — |
| 149 | Aragoto Senkenbutai | 4 | LI | Spec. Trained Troops | Regular, Impetuous | Aragoto |
| 161 | Yáozăo | 3 | REM | Support Troops | Peripheral | Servant |
| 1002 | Daiyōkai Dengekitai | 2 | HI | Headquarters Troops | Regular | Keisotsu; Domaru |
| 50 | Warcors | 1 | LI | Mercenary Troops | Irregular | — |
| 163 | Shinobu Kitsune | 1 | SK | Character | Regular | — |
| 147 | Kempeitai | 3 | LI | Spec. Trained Troops | Regular | Wildcard; counts as Keisotsu |
| 668 | Saito Tōgan | 1 | SK | Character | Regular | — |
| 1828 | Taguraidā, JSA TAG Support Pilots | 1 | LI | Support Troops | Regular | Keisotsu |
| 1834 | Yojimbo, Sword for Hire | 1 | WB | Character | Irregular, Impetuous | Mutually exclusive with Motorized Yojimbo |
| 135 | Ninjas | 3 | SK | Spec. Trained Troops | Regular | — |
| 152 | Domaru Butai | 5 | HI | Line Troops | Regular | Keisotsu; Domaru; Ōban |
| 999 | Tankō Zensenbutai | 3 | HI | Line Troops | Regular, Impetuous | Domaru; Banzai; counts as Domaru in Domaru FT |
| 1019 | Yuriko Oda | 1 | LI | Character | Regular | Wildcard, **FTO options 1/2 only**; counts as Keisotsu |
| 1683 | Freelance Operator Samsa | 1 | MI | Character | Regular | — |
| 159 | Yáoxiè Rui Shi | 2 | REM | Support Troops | Regular | Aragoto |
| 144 | Keisotsu Butai | 255 | LI | Line Troops | Regular | Keisotsu |
| 156 | O-Yoroi Kidobutai | 2 | TAG | Mechanized Troops | Regular | Includes Kobaruto Ancillary Remote |
| 1831 | Garon Aibōt | 1 | REM | Support Troops | Regular | — |
| 1832 | Uran Aibōt | 1 | REM | Support Troops | Regular | — |
| 996 | Ryūken Unit-9 | 3 | MI | Spec. Trained Troops | Regular | — |
| 1790 | Kyoshō Saibāyunitto | 1 | LI | Spec. Trained Troops | Regular | — |
| 157 | Oniwaban | 2 | SK | Elite Troops | Regular | — |
| 223 | Miyamoto Mushashi | 1 | WB | Character | Irregular or Regular by option | Banzai, **FTO option 2 only**; counts as Tankō |
| 1789 | Genbutai | 1 | MI | Veteran Troops | Regular | — |
| 773 | Shikami | 2 | HI | Elite Troops | Regular | Ōban |
| 224 | Yojimbo, Motorized Sword for Hire | 1 | WB | Character | Irregular, Impetuous | Mutually exclusive with foot Yojimbo |
| 162 | Yáopú Pangguling | 2 | REM | Support Troops | Regular | No Ōban Fireteam access, including FTO option 4 |
| 160 | Yáoxiè Lù Duān | 2 | REM | Support Troops | Regular | — |
| 1017 | Kuroshi Rider | 1 | LI | Character | Regular, Impetuous | Aragoto; counts as Aragoto |
| 378 | Yuan Yuan | 2 | WB | Mercenary Troops | Irregular, Impetuous | — |
| 154 | Karakuri Special Project | 3 | HI | Spec. Trained Troops | Regular | Ōban |
| 1830 | Atom Aibōt | 1 | REM | Support Troops | Regular | — |
| 1833 | Robio Aibōt | 1 | REM | Support Troops | Regular | — |
| 164 | Takeshi “Neko” Oyama | 1 | HI | Character | Regular | Keisotsu; Domaru; Ōban; counts as Domaru where marked |

### Optional-mode entries

| Unit ID | Unit | Mode | Fireteam hook |
|---:|---|---|---|
| 1924 | Kaizoku Spec-Ops | Infinity Spec-Ops | Up to 1 in Keisotsu Fireteams |
| 1938 | JSA Team-Ops | Infinity Team-Ops | Optional-mode only; no normal-roster Fireteam row |

## Unit details

Notation: stats are `MOV CC BS PH WIP ARM BTS VITA/STR S`. Source option IDs are retained because otherwise-similar loadouts and FTO legality can depend on them.

### Tokusetsu Butai — `tokusetsu-butai`

**Unit ID:** 158 — AVA 2 — LI, Support Troops.

- **Stats:** `10-10 15 11 10 13 1 0 1 2`.
- **Rules:** Courage.
- **Option 1:** **14 / 0** — Doctor, MediKit; Combi Rifle, Pistol, CC Weapon.
- **Option 2:** **14 / 0** — Engineer, Deactivator, GizmoKit; Combi Rifle, D-Charges, Pistol, CC Weapon.
- **Option 3:** **15 / 0** — Engineer, Deactivator, GizmoKit, Deployable Cover; option-2 weapons.
- **Option 4:** **17 / 0** — Engineer, Deactivator, GizmoKit; Combi Rifle, D-Charges, Armed Turret (Combi Rifle), Pistol, CC Weapon.

### Aragoto Senkenbutai — `aragoto-senkenbutai`

**Unit ID:** 149 — AVA 4 — LI, Spec. Trained Troops.

- **Stats:** `20-15 16 12 11 13 2 0 1 4`.
- **Rules/equipment:** Motorcycle, Limited Cover, Courage, Dodge (+5), Mimetism (-3), Impetuous.
- **Option 529:** **20 / 1** — Spitfire, Boarding Pistol, CC Weapon.
- **Option 530:** **13 / 0** — Boarding Shotgun, Boarding Pistol, CC Weapon.
- **Option 531:** **21 / 0.5** — Hacker, Hacking Device; Combi Rifle, Light Shotgun, Boarding Pistol, CC Weapon.
- **Option 532:** **19 / 0** — Hacker, Killer Hacking Device; Combi Rifle, Light Shotgun, Boarding Pistol, CC Weapon.
- **Fireteam:** Aragoto.

### Yáozăo — `yaozao`

**Unit ID:** 161 — AVA 3 — REM, Support Troops; Peripheral (Servant).

- **Stats:** `15-10 11 8 10 13 0 3 STR1 1`.
- **Rules:** Peripheral (Servant), Courage, Mimetism (-3).
- **Option 1:** **3 / 0** — PARA CC Weapon (-3); no Order of its own.

### Daiyōkai Dengekitai — `daiy-kai-dengekitai`

**Unit ID:** 1002 — AVA 2 — HI, Headquarters Troops.

- **Stats:** `10-10 21 13 14 13 5 3 2 5`.
- **Rules:** Martial Arts L2, BS Attack (SR-1), Courage, Stealth, No Wound Incapacitation, NCO.
- **Option 1:** **46 / 0** — MULTI Marksman Rifle, Panzerfaust, Pistol, AP + DA CC Weapon (PS=4).
- **Option 2:** **47 / 1** — Red Fury, Panzerfaust, Pistol, AP + DA CC Weapon (PS=4).
- **Option 3:** **50 / 1** — HMG, Panzerfaust, Pistol, AP + DA CC Weapon (PS=4).
- **Fireteams:** Keisotsu; Domaru.

### Warcors — `warcors-war-correspondents`

**Unit ID:** 50 — AVA 1 — LI, Mercenary Troops; Irregular.

- **Stats:** `10-10 11 9 11 13 0 0 1 2`.
- **Rules:** Journalist.
- **Option 1:** **3 / 0** — 360º Visor; Flash Pulse, Stun Pistol, PARA CC Weapon (-3).
- **Option 2:** **3 / 0** — Sixth Sense; Flash Pulse, Stun Pistol, PARA CC Weapon (-3).

### Shinobu Kitsune — `oniwaban-shinobu-kitsune`

**Unit ID:** 163 — AVA 1 — SK, Character.

- **Stats:** `10-10 25 12 13 14 1 3 1 2`.
- **Rules:** Martial Arts L5, Surprise Attack (-3), Camouflage, Courage, Hidden Deployment, Dodge (+5), Infiltration (PH=19), Mimetism (-6), Stealth, Terrain (Total), Climbing Plus.
- **Option 1:** **44 / 0.5** — Combi Rifle, Nanopulser, Smoke Grenades, Pistol, Monofilament CC Weapon.
- **Option 2 Lieutenant:** **44 / 0.5** — same loadout; Lieutenant.

### Kempeitai — `kempeitai`

**Unit ID:** 147 — AVA 3 — LI, Spec. Trained Troops.

- **Stats:** `10-10 17 12 10 14 1 0 1 2`.
- **Rules:** Courage, Number 2, Sixth Sense.
- **Option 1:** **22 / 1** — Spitfire, Pistol, CC Weapon, PARA CC Weapon (-3).
- **Option 3:** **20 / 0** — Combi Rifle; Chain of Command.
- **Option 4:** **17 / 0** — Boarding Shotgun; Chain of Command.
- **Option 5:** **22 / 1** — Shock Marksman Rifle; Multispectral Visor L2.
- **Fireteam:** Wildcard, all options; counts as Keisotsu.

### Saito Tōgan — `saito-togan`

**Unit ID:** 668 — AVA 1 — SK, Character.

- **Stats:** `10-10 24 11 13 13 1 0 1 2`.
- **Rules/equipment:** Martial Arts L4, Surprise Attack (-3), Camouflage, Courage, Hidden Deployment, Dodge (+2.5), Infiltration, Mimetism (-6), Stealth, Terrain (Total), Bangbomb (+4).
- **Option 1:** **33 / 0** — T2 Boarding Shotgun, Smoke Grenades, Pistol, EXP CC Weapon (PS=4).

### Taguraidā, JSA TAG Support Pilots — `taguraida-jsa-tag-support-pilots`

**Unit ID:** 1828 — AVA 1 — LI, Support Troops.

- **Stats:** `10-10 21 12 12 13 0 0 1 2`.
- **Rules:** Martial Arts L1, Courage, Stealth, TAGCom (Dodge PH+3; GizmoKit PH+1).
- **Option 2 — O-YOROI PILOT:** **11 / 0** — Forward Observer; Light Shotgun, Flash Pulse, D-Charges, Pistol, Shock CC Weapon (PS=7).
- **Fireteam:** Keisotsu.

### Yojimbo, Sword for Hire — `yojimbo-sword-for-hire`

**Unit ID:** 1834 — AVA 1 — WB, Character; Irregular, Impetuous.

- **Stats:** `15-5 24 12 14 13 1 3 1 2`.
- **Rules:** Martial Arts L4, Courage, Dodge (+2.5), Immunity (Critical), Minelayer, Stealth, No Cover, No Wound Incapacitation.
- **Option 1:** **19 / 0** — Contender (+1B), Nanopulser, Smoke Grenades, CrazyKoala, Pistol, DA CC Weapon (PS=3).
- **Identity restriction:** only one Yojimbo may be present in an Army List; mutually exclusive with Motorized Yojimbo (ID 224).

### Ninjas — `ninjas`

**Unit ID:** 135 — AVA 3 — SK, Spec. Trained Troops.

- **Stats:** `10-10 23 11 12 13 1 0 1 2`.
- **Rules:** Martial Arts L3, CC Attack (Shock), Surprise Attack (-3), Camouflage, Courage, Hidden Deployment, Dodge (+2.5), Infiltration, Mimetism (-6), Stealth, Terrain (Total), Climbing Plus.
- **Option 1:** **24 / 0** — Tactical Bow (+1SD), Shock Mine, Pistol, DA CC Weapon (PS=6).
- **Option 4:** **27 / 0** — Submachine Gun, Pistol, DA CC Weapon (PS=6).
- **Option 5:** **31 / 1.5** — MULTI Sniper Rifle, Pistol, DA CC Weapon (PS=6).
- **Option 6:** **33 / 0.5** — Hacker, Hacking Device; Submachine Gun, Pistol, DA CC Weapon (PS=6).
- **Option 7:** **26 / 0** — Hacker, Killer Hacking Device; Tactical Bow (+1SD), Shock Mine, Pistol, DA CC Weapon (PS=6).
- **Option 9:** **30 / 0.5** — Forward Observer; Boarding Shotgun, Flash Pulse, Pistol, DA CC Weapon (PS=6).

### Domaru Butai — `domaru-butai`

**Unit ID:** 152 — AVA 5 — HI, Line Troops.

- **Stats:** `15-5 24 12 14 13 3 3 2 2`.
- **Rules:** Martial Arts L3, CC Attack (Shock), BS Attack (SR-1), Courage, Dodge (+5), Frenzy, Stealth, Berserk.
- **Option 1:** **19 / 0** — Chain Rifle, Pistol, Contender, E/M Grenades, AP CC Weapon (PS=4).
- **Option 2:** **20 / 0** — Chain Rifle, Pistol, Contender, E/M Grenades, E/M CC Weapon (PS=4).
- **Option 3:** **23 / 0** — Boarding Shotgun, E/M Grenades, Pistol, E/M CC Weapon (PS=4).
- **Option 5:** **31 / 1.5** — Spitfire, Pistol, E/M CC Weapon (PS=4).
- **Option 6:** **27 / 0** — Forward Observer; Combi Rifle, E/M Grenades, Flash Pulse, Pistol, E/M CC Weapon (PS=4).
- **Option 7 Lieutenant (+1 Order):** **23 / 0** — option-2 weapons.
- **Option 8 Lieutenant (+1 Order):** **35 / 1.5** — Spitfire, Pistol, E/M CC Weapon (PS=4).
- **Fireteams:** Keisotsu; Domaru; Ōban.

### Tankō Zensenbutai — `tank-zensenbutai`

**Unit ID:** 999 — AVA 3 — HI, Line Troops; Regular, Impetuous.

- **Stats:** `15-5 23 13 13 13 3 3 2 2`.
- **Rules:** Martial Arts L2, Limited Cover, Courage, Dodge (+2.5), Stealth, Impetuous.
- **Option 1:** **18 / 0** — Blitzen, Light Shotgun, Pistol, Monofilament CC Weapon, Shock CC Weapon (PS=6).
- **Option 2:** **19 / 0** — Blitzen, Submachine Gun, Pistol, Monofilament CC Weapon, Shock CC Weapon (PS=6).
- **Option 3:** **19 / 0** — Flammenspeer, Contender, Pistol, Monofilament CC Weapon, Shock CC Weapon (PS=6).
- **Option 4:** **26 / 1.5** — Missile Launcher, Pistol, Monofilament CC Weapon, Shock CC Weapon (PS=6).
- **Option 7:** **19 / 0** — Blitzen, Light Shotgun, Disco Baller, Pistol, Monofilament CC Weapon, Shock CC Weapon (PS=6); Deactivator.
- **Fireteams:** Domaru (counts as Domaru); Banzai.

### Yuriko Oda — `keisotsu-kaizoku-yuriko-oda`

**Unit ID:** 1019 — AVA 1 — LI, Character.

- **Stats:** `10-10 15 12 11 13 1 3 1 2`.
- **Rules/equipment:** Courage, Dodge modifiers, Engineer, Mimetism (-3), Minelayer; Deactivator, GizmoKit.
- **Option 1 — YURIKO ODA FTO:** **25 / 0** — Combi Rifle, E/Mitter, D-Charges, Shock Mine, Pistol, CC Weapon. **Wildcard legal.**
- **Option 2 — YURIKO ODA FTO:** **23 / 0** — Combi Rifle, Panzerfaust, D-Charges, Shock Mine, Pistol, CC Weapon. **Wildcard legal.**
- **Option 3:** **28 / 0.5** — option-1 weapons; Forward Deployment (+20). **Not FTO.**
- **Fireteam:** Wildcard options 1/2 only; counts as Keisotsu.

### Freelance Operator Samsa — `freelance-operator-samsa`

**Unit ID:** 1683 — AVA 1 — MI, Character.

- **Stats:** `15-5 15 13 11 13 3 0 1 2`.
- **Rules:** Surprise Attack (-3), Dodge (+2.5), Exrah, Infiltration, Mimetism (-3), Specialist Operative, Decoy (1), Super-Jump.
- **Option 1:** **26 / 0** — Plasma Rifle, D-Charges, Pistol, CC Weapon.

### Yáoxiè Rui Shi — `yaoxie-rui-shi`

**Unit ID:** 159 — AVA 2 — REM, Support Troops.

- **Stats:** `15-10 13 12 10 13 1 6 STR1 4`.
- **Rules/equipment:** Remote Presence, Courage, Repeater.
- **Option 1:** **23 / 1** — Spitfire, PARA CC Weapon (-3); Multispectral Visor L2.
- **Option 2:** **21 / 0.5** — Red Fury, Mine Dispenser (Shock), PARA CC Weapon (-3); Multispectral Visor L1.
- **Fireteam:** Aragoto, max 1.

### Keisotsu Butai — `keisotsu`

**Unit ID:** 144 — AVA 255 — LI, Line Troops.

- **Stats:** `10-10 17 11 10 12 1 0 1 2`.
- **Rules:** Courage.
- **Option 1:** **10 / 0** — Combi Rifle, Pistol, CC Weapon.
- **Option 2:** **18 / 1** — HMG, Pistol, CC Weapon.
- **Option 3:** **15 / 1.5** — Missile Launcher, Pistol, CC Weapon.
- **Option 4:** **16 / 0.5** — Hacker, Hacking Device, ECM: Hacker (-6); Combi Rifle, CrazyKoala, Pistol, CC Weapon.
- **Option 7:** **11 / 0** — Forward Observer; Combi Rifle, Flash Pulse (PS=6), Pistol, CC Weapon.
- **Option 8:** **12 / 0** — Paramedic, MediKit; Combi Rifle, Pistol, CC Weapon.
- **Option 9 Lieutenant:** **10 / 0.5** — Combi Rifle, Pistol, CC Weapon.
- **Option 10:** **12 / 0** — Commlink (+1), Specialist Operative; Combi Rifle, Pistol, CC Weapon.
- **Option 11:** **9 / 0** — AP Rifle, Pistol, CC Weapon.
- **Option 12:** **12 / 0** — Thunderbolt, Pistol, CC Weapon; BS Attack (-3 source modifier).
- **Option 13 Lieutenant:** **9 / 0.5** — AP Rifle, Pistol, CC Weapon.
- **Fireteam:** Keisotsu; at least one Keisotsu is required by the canonical family row.

### O-Yoroi Kidobutai — `o-yoroi-kidobutai`

**Unit ID:** 156 — AVA 2 — TAG, Mechanized Troops.

- **Stats:** `15-10 23 14 16 13 7 6 STR3 7`.
- **Rules/equipment:** Martial Arts L2, BS Attack (SR-1), Courage, Dodge (+5), GizmoKit (PH=11), Minelayer, Tactical Awareness, Stealth, additional Dodge PH=13 source modifier; ECM: Guided (-6).
- **Option 1:** **78 / 1.5** — MULTI HMG, Heavy Flamethrower, CrazyKoala, EXP CC Weapon (PS=3); includes 1 Kobaruto.
- **Option 2 Lieutenant:** **78 / 1.5** — same loadout; Lieutenant; includes 1 Kobaruto.
- **Kobaruto Ancillary Remote:** `10-10 -1 -1 10 13 0 3 STR1 1`; Peripheral (Ancillary), Courage, Dodge (+3), Mimetism (-3), Specialist Operative.

### Garon Aibōt — `garon-aib-t`

**Unit ID:** 1831 — AVA 1 — REM, Support Troops.

- **Stats:** `15-10 13 11 10 13 0 3 STR1 3`.
- **Rules/equipment:** Courage, Remote Presence, Total Reaction; 360º Visor.
- **Option 1:** **23 / 1** — HMG, PARA CC Weapon (-3).
- **Option 2:** **21 / 0** — Mk12, PARA CC Weapon (-3).
- **Option 3:** **16 / 0** — Thunderbolt, Smoke Grenade Launcher, PARA CC Weapon (-3).

### Uran Aibōt — `uran-aib-t`

**Unit ID:** 1832 — AVA 1 — REM, Support Troops.

- **Stats:** `15-10 13 12 10 13 0 3 STR1 3`.
- **Rules:** BS Attack (Guided), Courage, Remote Presence.
- **Option 1:** **16 / 1.5** — Missile Launcher, PARA CC Weapon (-3).

### Ryūken Unit-9 — `ryuken-unit-9`

**Unit ID:** 996 — AVA 3 — MI, Spec. Trained Troops.

- **Stats:** `10-10 17 12 11 14 2 3 1 2`.
- **Rules/equipment:** X-Visor, Courage, Mimetism (-6), Minelayer, Decoy (1).
- **Option 1:** **23 / 1.5** — Heavy Rocket Launcher, Shock Mine, Heavy Pistol, CC Weapon; Surprise Attack (-3), Camouflage (1 Use).
- **Option 2:** **22 / 0.5** — Submachine Gun, Shock Mine, D-Charges, Breaker Pistol (+1B), CC Weapon; Forward Deployment (+20).
- **Option 3:** **25 / 0.5** — option-2 weapons; Killer Hacking Device, Hacker; Forward Deployment (+20).

### Kyoshō Saibāyunitto — `kyosh-saibayunitto`

**Unit ID:** 1790 — AVA 1 — LI, Spec. Trained Troops.

- **Stats:** `10-10 17 11 10 13 1 6 1 2`.
- **Base rule:** Hacker with source upgrade `Total Control (SR-2)`.
- **Option 1:** **20 / 0.5** — Hacking Device; Combi Rifle, Cybermine, Breaker Pistol, CC Weapon.
- **Option 2:** **20 / 0** — Killer Hacking Device; MULTI Rifle, Cybermine, Breaker Pistol, CC Weapon.

### Oniwaban — `oniwaban`

**Unit ID:** 157 — AVA 2 — SK, Elite Troops.

- **Stats:** `10-10 24 11 12 14 1 0 1 2`.
- **Rules:** Martial Arts L4, Surprise Attack (-3), Camouflage, Courage, Hidden Deployment, Dodge (+5), Infiltration (PH=18), Mimetism (-6), Stealth, Terrain (Total).
- **Option 1:** **30 / 0** — Boarding Shotgun, Nanopulser, Pistol, Monofilament CC Weapon, E/M CC Weapon (PS=5).
- **Option 2:** **29 / 0** — Submachine Gun, Nanopulser, Pistol, Monofilament CC Weapon, E/M CC Weapon (PS=5).
- **Option 3 Lieutenant:** **30 / 1** — option-1 weapons; Lieutenant.

### Miyamoto Mushashi — `miyamoto-mushashi`

**Unit ID:** 223 — AVA 1 — WB, Character.

- **Stats:** `15-10 25 9 14 15 1 3 1 2`.
- **Rules:** Martial Arts L5, CC Attack (AP), Courage, Dodge (+5), Immunity (ARM), Stealth, No Wound Incapacitation.
- **Option 1:** **21 / 0** — Irregular; Chain Rifle, Tactical Bow, Flash Pulse, Pistol, EXP CC Weapon (PS=4). **Not Fireteam legal.**
- **Option 2 — MIYAMOTO MUSHASHI FTO:** **25 / 0.5** — Regular; same weapons. **Banzai Fireteam legal and counts as Tankō.**

### Genbutai — `genbutai`

**Unit ID:** 1789 — AVA 1 — MI, Veteran Troops.

- **Stats:** `10-10 18 13 11 13 3 6 1 2`.
- **Rules:** BS Attack (SR-1), Warhorse, Immunity (AP), Immunity (Shock), Religious Troop.
- **Option 1:** **18 / 0** — Boarding Shotgun, Chain-colt, Breaker Pistol, PARA CC Weapon (-6).
- **Option 2:** **23 / 0** — Engineer, GizmoKit; Submachine Gun, Panzerfaust, D-Charges, Breaker Pistol, PARA CC Weapon (-6).
- **Option 3:** **26 / 0** — Specialist Operative; MULTI Rifle, Heavy Flamethrower, D-Charges, Breaker Pistol, PARA CC Weapon (-6).
- **Option 4:** **20 / 0** — Paramedic, MediKit; Boarding Shotgun, Chain-colt, Breaker Pistol, PARA CC Weapon (-6).
- **Option 5:** **29 / 1** — NCO; Red Fury, Breaker Pistol, PARA CC Weapon (-6).

### Shikami — `shikami`

**Unit ID:** 773 — AVA 2 — HI, Elite Troops.

- **Stats:** `15-5 23 13 14 13 3 3 2 2`.
- **Rules:** Martial Arts L3, Courage, Forward Deployment (+10), Dodge (+5), Mimetism (-6), Specialist Operative, Stealth, Climbing Plus, Super-Jump (+7.5).
- **Option 1:** **42 / 0** — Contender, Flash Pulse (+1B), Eclipse Grenades, Assault Pistol, AP + DA CC Weapon (PS=4).
- **Option 2:** **47 / 0** — MULTI Rifle, D-Charges, Eclipse Grenades, Pistol, AP + DA CC Weapon (PS=4).
- **Fireteam:** Ōban.

### Yojimbo, Motorized Sword for Hire — `yojimbo-motorized-sword-for-hire`

**Unit ID:** 224 — AVA 1 — WB, Character; Irregular, Impetuous.

- **Stats:** `20-15 24 12 14 13 1 3 1 4`.
- **Rules/equipment:** Motorcycle, Martial Arts L4, Limited Cover, Courage, Dodge (+5), Immunity (Critical), Mimetism (-3), Minelayer, No Wound Incapacitation.
- **Option 741:** **20 / 0** — Contender (+1B), Nanopulser, Smoke Grenades, Smoke Grenade Launcher, CrazyKoala, Pistol, DA CC Weapon (PS=3).
- **Identity restriction:** only one Yojimbo may be present in an Army List; mutually exclusive with foot Yojimbo (ID 1834).

### Yáopú Pangguling — `yaopu-pangguling`

**Unit ID:** 162 — AVA 2 — REM, Support Troops.

- **Stats:** `10-10 13 11 10 13 2 3 STR1 4`.
- **Rules/equipment:** Baggage, Remote Presence, Courage.
- **Option 1:** **8 / 0** — Deactivator, Repeater; PARA CC Weapon (-3).
- **Option 2:** **14 / 0.5** — EVO Hacking Device, Hacker; PARA CC Weapon (-3).
- **Option 3:** **17 / 0** — Repeater, Total Reaction; Combi Rifle, PARA CC Weapon (-3).
- **Option 4 — PANGGULING FTO:** **12 / 0** — Repeater; Light Shotgun, PARA CC Weapon (-3). **No Fireteam access in the Ōban chart.**

### Yáoxiè Lù Duān — `yaoxie-lu-duan`

**Unit ID:** 160 — AVA 2 — REM, Support Troops.

- **Stats:** `15-10 13 12 10 13 1 6 STR1 4`.
- **Rules/equipment:** Holoprojector, Multispectral Visor L1, Remote Presence, Courage, Surprise Attack (-3), BS Attack (+1B).
- **Option 1:** **24 / 0** — Mk12, Heavy Flamethrower, E/M Mine, PARA CC Weapon (-3).
- **Option 2:** **20 / 0** — Thunderbolt, E/M Carbine, E/M Mine, PARA CC Weapon (-3).

### Kuroshi Rider — `kuroshi-rider`

**Unit ID:** 1017 — AVA 1 — LI, Character; Regular, Impetuous.

- **Stats:** `20-15 23 12 13 14 2 3 1 4`.
- **Rules/equipment:** Motorcycle, Martial Arts L1, Limited Cover, Courage, Dodge (+7.5), Immunity (Shock), Mimetism (-3), Forward Observer, Dogged, Impetuous.
- **Option 3736:** **26 / 0** — Combi Rifle, Light Shotgun, Smoke Grenade Launcher, D-Charges, Breaker Pistol, AP + Shock CC Weapon (PS=6).
- **Option 3737 Lieutenant:** **26 / 0** — same loadout; Lieutenant.
- **Fireteam:** Aragoto; counts as Aragoto.

### Yuan Yuan — `yuan-yuan`

**Unit ID:** 378 — AVA 2 — WB, Mercenary Troops; Irregular, Impetuous.

- **Stats:** `10-10 22 10 14 13 0 0 1 2`.
- **Rules:** Booty, Parachutist, Combat Jump (PH=11), No Cover, Super-Jump (Jet Propulsion), Impetuous.
- **Option 2:** **6 / 0** — Chain Rifle, Smoke Grenades, Heavy Pistol, AP CC Weapon (PS=6).
- **Option 3:** **7 / 0** — Chain Rifle, Smoke Grenades, Pistol, DA CC Weapon (PS=6).
- **Option 4:** **11 / 0** — Boarding Shotgun, Smoke Grenades, Pistol, AP CC Weapon (PS=6).
- **Option 5:** **11 / 0** — Rifle, Smoke Grenades, Pistol, AP CC Weapon (PS=6).

### Karakuri Special Project — `karakuri-special-project`

**Unit ID:** 154 — AVA 3 — HI, Spec. Trained Troops; Structure 3.

- **Stats:** `10-10 10 13 10 13 3 6 STR3 2`.
- **Rules:** Courage, GizmoKit (PH=12), Immunity (Enhanced), Forward Observer, Remote Presence.
- **Option 1:** **31 / 0** — Heavy Shotgun, Chain Rifle, Panzerfaust, Flash Pulse, Pistol, CC Weapon.
- **Option 3:** **35 / 0** — MULTI Rifle, Chain Rifle, Panzerfaust, Flash Pulse, Pistol, CC Weapon.
- **Option 4:** **38 / 0** — Mk12, Chain Rifle, Panzerfaust, Flash Pulse, Pistol, CC Weapon.
- **Option 5:** **31 / 0** — E/Mitter, Chain Rifle, Panzerfaust, Flash Pulse, Pistol, CC Weapon.
- **Fireteam:** Ōban.

### Atom Aibōt — `atom-aib-t`

**Unit ID:** 1830 — AVA 1 — REM, Support Troops.

- **Stats:** `15-10 13 11 10 13 0 3 STR1 3`.
- **Rules/equipment:** Deactivator, Repeater, Triangulated Fire, Courage, Forward Observer, Remote Presence.
- **Option 1:** **15 / 0** — Combi Rifle, Flash Pulse, PARA CC Weapon (-3); Sensor.
- **Option 2:** **17 / 0** — Combi Rifle (source modifier retained), Flash Pulse (+1B), PARA CC Weapon (-3).

### Robio Aibōt — `robio-aib-t`

**Unit ID:** 1833 — AVA 1 — REM, Support Troops.

- **Stats:** `15-15 13 8 11 13 0 3 STR1 3`.
- **Rules/equipment:** Repeater, Courage, Mimetism (-3), Remote Presence.
- **Option 1:** **7 / 0** — Flash Pulse, PARA CC Weapon (-3).

### Takeshi “Neko” Oyama — `domaru-takeshi-neko-oyama`

**Unit ID:** 164 — AVA 1 — HI, Character.

- **Stats:** `15-5 24 12 14 14 3 6 2 2`.
- **Rules:** Martial Arts L3, CC Attack (Shock), BS Attack (SR-1), Courage, Dodge (+5), Frenzy, Tactical Awareness, Stealth, Berserk.
- **Option 1:** **28 / 0** — Chain Rifle, Contender, E/M Grenades, Breaker Pistol, E/M CC Weapon (PS=4), DA CC Weapon (PS=4).
- **Option 2 Lieutenant:** **28 / 0** — same loadout; Lieutenant.
- **Fireteams:** Keisotsu; Domaru (counts as Domaru); Ōban (counts as Domaru).

## Canonical Fireteams

The tables below are authoritative for Ōban Fireteam legality. Profile names such as `FTO` do not grant access by themselves.

### Keisotsu Fireteams

**Types:** Haris, Core.

| Member | Min | Max | Required / equivalence | Profile restriction |
|---|---:|---:|---|---|
| Keisotsu | 1 | 5 | Native required minimum | all options |
| Domaru | 0 | 1 | — | all options |
| Daiyōkai | 0 | 1 | — | all options |
| Oyama | 0 | 1 | — | all options |
| Taguraidā | 0 | 1 | — | option 2 (only standard profile) |
| Kaizoku Spec-Ops | 0 | 1 | Spec-Ops mode only | optional-mode record |

Wildcards may join subject to the Wildcard rules below.

### Domaru Fireteams

**Types:** Duo, Haris, Core.

| Member | Min | Max | Required / equivalence | Profile restriction |
|---|---:|---:|---|---|
| Domaru | 1 | 5 | Native required minimum | all options |
| Oyama | 0 | 1 | counts as Domaru | all options |
| Tankō | 0 | 3 | counts as Domaru | all options |
| Daiyōkai | 0 | 1 | — | all options |

Wildcards may join subject to the Wildcard rules below.

### Ōban Fireteams

**Types:** Duo, Haris.

The Army source marks Domaru, Karakuri, and Shikami rows `required: true`. Treat these as a **required source-choice set**: at least one member must come from that three-row source set.

| Member | Min | Max | Required / equivalence | Profile restriction |
|---|---:|---:|---|---|
| Domaru | 0 | 3 | required-source set | all options |
| Karakuri | 0 | 3 | required-source set | all options |
| Shikami | 0 | 2 | required-source set | all options |
| Oyama | 0 | 1 | counts as Domaru | all options |

Wildcards may join subject to the Wildcard rules below.

### Banzai Fireteams

**Types:** Duo, Haris.

| Member | Min | Max | Required / equivalence | Profile restriction |
|---|---:|---:|---|---|
| Tankō | 1 | 3 | Native required minimum | all options |
| Miyamoto Mushashi | 0 | 1 | counts as Tankō | **FTO option 2 only** |

Wildcards may join subject to the Wildcard rules below.

### Aragoto Fireteams

**Types:** Duo, Haris.

| Member | Min | Max | Required / equivalence | Profile restriction |
|---|---:|---:|---|---|
| Aragoto | 1 | 2 | Native required minimum | all options |
| Kuroshi Rider | 0 | 1 | counts as Aragoto | both options |
| Rui Shi | 0 | 1 | — | both options |

Wildcards may join subject to the Wildcard rules below.

## Wildcards

| Wildcard | Max | Counts as | Profile restriction |
|---|---:|---|---|
| Kempeitai | 3 | Keisotsu | all options |
| Yuriko Oda FTO | 1 | Keisotsu | **options 1/2 only** |

Wildcard means the listed profile may join any otherwise legal Ōban Fireteam unless another rule prevents it. The `Counts as` label is preserved separately because it can matter to composition requirements.

## Unit → Fireteam access index

This is a derivative lookup table. If it conflicts with the canonical Fireteam section above, the canonical section wins.

| Unit | Access |
|---|---|
| Aragoto | Aragoto — all options |
| Daiyōkai | Keisotsu; Domaru — all options |
| Domaru | Keisotsu; Domaru; Ōban — all options |
| Karakuri | Ōban — all options |
| Keisotsu | Keisotsu — all options |
| Kempeitai | Wildcard — all options; counts as Keisotsu |
| Kuroshi Rider | Aragoto — both options; counts as Aragoto |
| Miyamoto Mushashi | Banzai — **option 2 FTO only**; counts as Tankō |
| Oyama | Keisotsu; Domaru; Ōban — all options; counts as Domaru where chart marks it |
| Rui Shi | Aragoto — both options, max 1 |
| Shikami | Ōban — all options |
| Taguraidā | Keisotsu — option 2 |
| Tankō | Domaru; Banzai — all options; counts as Domaru in Domaru FT |
| Yuriko Oda | Wildcard — **options 1/2 FTO only**; counts as Keisotsu |
| Kaizoku Spec-Ops | Keisotsu — optional Spec-Ops mode only |

Explicit negative lookup notes:

- **Pangguling option 4 (`PANGGULING FTO`) has no Ōban Fireteam access.**
- Ordinary non-FTO **Miyamoto option 1** cannot join Banzai.
- **Yuriko option 3** cannot use the Wildcard row.
- No other standard roster unit gains Fireteam access merely from sharing JSA ancestry or from an FTO label outside this chart.

## Roster identity and dependency rules

### Yojimbo mutual exclusion

The Army source relates Yojimbo source records `224`, `1834`, `10224`, and `11834` with a maximum of one. In standard Ōban the available relevant records are:

- ID `1834`: Yojimbo, Sword for Hire.
- ID `224`: Yojimbo, Motorized Sword for Hire.

A list may therefore contain **at most one Yojimbo** across those available variants.

### Yuriko identity relation

The Army source also relates unit `1019` (this roster's Yuriko Oda) with source identity `1799`, maximum one. Unit `1799` is not a second ordinary standard Ōban roster entry here; preserve the relation when comparing against Reinforcement/alternate JSA data.

### Peripherals and composite records

- **Yáozăo** are Servant Peripherals and do not generate Orders independently.
- **O-Yoroi** options include one **Kobaruto Ancillary Remote**; the Kobaruto is not counted as a separate roster entry.
- Optional Spec-Ops / Team-Ops subprofiles and SpecBots remain inside their optional-mode records.

## Reinforcements boundary

The standard Ōban dataset exposes Reinforcements Army ID **1199**. It is deliberately not merged into this file's standard roster or canonical Fireteam chart. For ordinary Ōban list building, use the 35 standard roster records and Fireteams above; use a separate Reinforcements reference when Reinforcement mode is explicitly involved.

## Validation notes

Validated against Army snapshot `7.26246.159`:

- Standard roster membership was determined from faction availability containing sectorial ID `1103`.
- **35** standard logical roster records were identified.
- **2** optional-mode records were separated: Kaizoku Spec-Ops (`1924`) and JSA Team-Ops (`1938`).
- Generic `factions: []` Soldier-of-Fortune catalog entries were excluded.
- Fireteam limits are Core `1`, Haris `1`, Duo `256`.
- Canonical families are Keisotsu, Domaru, Ōban, Banzai, and Aragoto.
- Wildcards are Kempeitai and Yuriko Oda FTO.
- FTO restrictions were reconciled against profile option names: Yuriko `1/2`; Miyamoto `2`.
- `PANGGULING FTO` was intentionally **not** granted Fireteam access because no canonical chart row grants it.
- Counts-as relationships were preserved separately from ordinary membership.
- The Yojimbo mutual-exclusion relation was retained.
- Reinforcement Army ID `1199` remains distinct.

## Command-unit apex/value cross-reference (2026-10-23)

**Domaru LT(+1) 23/0** is a cheap route to extra personal Order pressure; **Kempeitai CoC 17/0 BSG / 20/0 Combi** is excellent budget insurance for aggressive Ōban commanders. A Kempeitai successor should guard **different ingress** from the LT's main assault. These are roster-legal Ōban options; don't infer that every other JSA sectorial has identical access.

See [cross-game Lieutenant, CoC and Order-economy tiers](../../notes/list-building/command-units-apex-and-value.md). **Refer to this pinned roster/Fireteam chart for profile legality.**

## Mission specialist / button-pusher selections (N5.3)

The most important choice is **how many independent turn-3 scoring routes survive the attack**, not the number of Samurai combat models. **Kempeitai CoC17/0** supplies inexpensive Specialist/command insurance for Domaru/Hatamoto-style attacking LT plans when roster-legal. **Ninja/Kurayami hidden specialists** shorten contested-console routes; **Aragoto KHD** is fast but more vulnerable. Do not import Vanilla JSA Shikami or other profile unless this Ōban roster lists them.

[Cross-faction apex and points-value guide](../../notes/list-building/mission-specialists-and-button-pushers-apex-value.md). Use **this roster and Fireteam chart** for exact availability.

## N5.3 airborne / backline-strike archetypes and trades (2026-10-23)

**Oniwaban29/0 and Shinobu44/.5** are near-deployment **Hidden/Infiltration Monofilament** enemies and force early opponent screening; the enemy-half roll is optional, not an automatic DZ start. **Oniwaban LT30/1 / Shinobu LT44/.5** must be on-table as Model/Marker at the LoL check—not sitting Hidden. **Kempeitai CoC17** protects a risky on-table LT but is not an airborne assassin. Check this **Ōban roster** for current **AD biker/other airborne** options; don't import Vanilla JSA Teishin by name unless listed.

[Full N5.3 apex/value and delivery-probability tier guide](../../notes/list-building/airborne-and-enemy-dz-attackers-apex-value.md). Current roster/profile restrictions and canonical Fireteam chart above govern legal choices.

## Active-turn gunfighter cross-reference (2026-10-23)

**Active-turn shooting choices:** **O-Yoroi MULTI HMG78/1.5** is a full **TAG** BS14/3STR/TacAware long-range firepower anchor with CrazyKoala/CC close protection; strong on open tables but poor value if the huge base must navigate tight hacker-controlled corridors. **Shikami42/0 or MULTI Rifle47/0** is a **non-TAG** Mimetism(-6), Climbing/Super-Jump/Eclipse mobile specialist that can win on **movement and scoring**, not raw HMG volume. The strongest melee trooper often opens the route **before** choosing whether the TAG's gun needs to fire. [Separate TAG/non-TAG rankings](../../notes/list-building/active-turn-gunfighters-apex-and-value.md).

## Warband cheap trading / order economy — N5.3

**Yuan Yuan6/0 Chain+Smoke or 7/0 DA CC, AVA2** gives Ōban *unique* ultra-low-cost Irregular/Impetuous airborne smoke/template/CC disruption; **PH11 Combat Jump only 55%** without actual support, normal Parachutist safer if an open edge. **Miyamoto Musashi Irregular Chain+EXP21/0** is apex melee **CC25/MA5** but cannot join Banzai; **FTO Regular25/.5** alone is Banzai/Counts-as-Tankō Fireteam legal, a different investment. **Aragoto bikes** move rapidly without smoke on their profiles. **Kempeitai CoC17** should survive LT loss, not be thrown away to trade.

[Current cross-faction warband apex/value, opponent counters, Lt/CoC packages](../../notes/list-building/warbands-and-cheap-trading-units-apex-value.md). This faction's own pinned profile and Fireteam rows control legality.

## TAG tactical cross-reference (2026-10-23)

**O-Yoroi** is the ranged/armored counterweight to Oban's infiltration and close-combat attacks. Preserve the Kobaruto/Engineer/support and enough mission specialists, rather than allowing one TAG to absorb all activation budget; use its long-range threats to clear lanes for the infiltration units. Assess Fireteam access from the Oban chart only.

Across all factions, compare **apex power** separately from **points value**, counterplay and mission fit: [N5.3 TAG guide](../../notes/list-building/tags.md). The current unit profiles and canonical Fireteam chart above take precedence over tactical opinions.

## Hacker and KHD tactical cross-reference (2026-10-23)

**Kyoshō KHD20/0 versus HD20/0.5**, **Keisotsu HD16/0.5** and **Ninja KHD26/0 (Hidden)/HD33/0.5** give Oban both inexpensive backline hacking and expensive *infiltrating* mission specialists. **Why:** Kyoshō KHD supplies Trinity/Cybermask and remains a scoring troop; choose HD if the main opponent threat is hackable TAG/HI instead. Ninja's higher cost is a **deployment/hidden scoring premium**, not superior bare hacking dice. Do not project Shindenbutai Tanuki/Nokizaru teams or White Banner KHD hybrid upgrades into Oban; use Oban's own canonical roster and Fireteam restrictions.

See the [cross-game apex/value Hacker/KHD tier guide](../../notes/list-building/hackers-and-killer-hackers.md). **The sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative; device upgrades are profile-specific.**


## Cheerleader / Order-generation tactical cross-reference (2026-10-23)

See the N5.3 [cross-game apex/value rankings and transcript-backed competing assessments](../../notes/list-building/cheerleaders-and-order-generators.md). The current roster and official Fireteam definitions above remain authoritative; unit access/cost may differ from vanilla.

- Keisotsu — inexpensive S2 Regular bodies, line-FT material and possible utility upgrades; optimize the cheapest legal role rather than premium heavy guns.
- Servant REM — does not generate a new Order, even when helping an Engineer cover more ground.
- Yuriko/Engineer — buy for recovery and mission support, not cheap generic Order generation.
- Karakuri — durable multiple-role attacker/specialist, not a minimal-cost backline cheerleader; compare total Order demand.
- 3pt Warcor — very useful Irregular Flash ARO/cheap screen, NOT an ordinary transferable Order.

**Selection rule:** Count deployed, transferable Regular Orders per Combat Group, not total models or restricted bonus Orders; choose the lowest-cost protected Regular profile that *also* contributes a relevant Repeater, Baggage, Fireteam, template, ARO or Specialist job. Check Group slots and DZ hiding space before buying a third large-base REM or replacing a needed scoring piece.


## ARO apex/value cross-reference (2026-10-23)

[Best ARO units across N5.3 — absolute apex vs points-value](../../notes/list-building/aro-units-apex-and-value.md) compares hidden reactive fire, TR/Neurocinetics, Flash/DTW/expendable defenders and why competing creators disagree. The **roster here** is authoritative for actual costs, Training, AVA and Fireteam construction.

- **Garon TR** — 16pt/0SWC Thunderbolt/smoke option shifts from passive guard to active smoke enablement where legal
- **Ryūken rocket launcher** — low-mid cost marker/ambush control; complement with mines and a second visible layer
- **Karakuri** — durable roadblock/scoring threat for close quarters; not cost-effective as an inert long-lane sniper
- **Warcor 3pt Flash** — disposable Irregular Stun/Orders tax, not a generic Regular cheerleader

**Best circumstance:** long exposed lanes justify a real sniper/missile/linked gun; dense tables, DZ landings and mission rooms favor E/M, mine, Shotgun, Riotstopper and hidden traps. Cover the destination/approach, layer serial threats rather than two pie-sliceable visible guns, and preserve scoring units for the active turn.

## N5.3 midfield area denial / speed bumps (tactical synthesis)

**Reactive deception, not universal infiltrator:** **Ryūken-9 HRL 23/1.5** begins with Minelayer Shock Mine, Decoy(1), one-use Camo and Mimetism(-6). Hold a long lane so enemy must Discover or detour. **Ryūken 22/.5 SMG** is the *separate* FD(+20) midfield denial option; cheaper SWC but poor long-distance reach. **Counterview:** its 1W/1.5SWC HRL may be bypassed by templates/Sensor or cost too much for objectives; consider durable Karakuri and other Camo instead. **O-Yoroi** Koala/Minelayer is a **TAG** and priced as a premium gun/armour package, not a cheap speed bump.

[Cross-game apex/value, matchups, and transcript disagreements](../../notes/list-building/midfield-area-denial-and-speed-bumps-apex-value.md). Tactical evaluation, not a modification to Army profiles or Fireteam legality.

## Doctor / Engineer / Recovery cross-reference (2026-10-23)

**Tokusetsu Engineer14 + Yáozăo3** is the baseline repair web for **O-Yoroi/Karakuri** where roster-legal; plan a servant within one safe Move of the TAG's fall-back turn lane. **Yuriko25** provides forward Mimetism/minelayer/Engineer utility only if both roles matter. **Tokusetsu Doctor14** instead serves VITA troops such as midfield infiltrators when recovering them is physically possible; a Shikami deep in enemy territory is not automatically inside the DZ Doctor's radius. [Doctor/Engineer apex and recovery odds](../../notes/list-building/doctors-engineers-and-recovery-apex-value.md).

## N5.3 DZ defense / anti-alpha-strike tactical choices

**Ryūken-9 HRL+Shock Mine Minelayer 23/1.5** offers a predeployed DZ mine plus 1-use Camo/Decoy(1)/Mimetism(-6) to threaten an attacker after entering; especially good against visible attackers who must cross a long lane. **The 22/.5 SMG+FD(+20)** is a **different** profile for closer approach control, not an equivalent HRL guard. **Warcor 360º3/0**, where selected, gives rear-angle Flash; standard **Keisotsu CrazyKoala Hacker 16/.5** is contingent on spending Order(s) to Place Deployable. **Counterpoint (Shepherd Ōban):** an HRL defender can be avoided/smoked; a useful Karakuri mission/counterattack often beats paying for several static reactive threats.

[Whole-game DZ defense value/apex and anti-IMP matchups](../../notes/list-building/dz-defenders-alpha-strike-and-impersonation-apex-value.md).

## Close-combat assassins and counter-CC — N5.3 (2026-10-23)

**Shinobu44/.5** (Hidden, Infiltration PH19, CC25/MA5, Monofilament) has the highest precision-assassin ceiling; **Oniwaban SMG29/0** is the value substitute (CC24/MA4, Mono/E/M). **Saito33/0** trades Mono for Smoke, T2 shotgun and EXP; **Musashi21 Irregular or 25 FTO Regular** wins pure CC25/MA5/EXP at cheap price but has to **walk**; **Shikami42** trades one-hit kill for Eclipse, Super-Jump, Climbing, 2W and scoring. **Yojimbo bike20 vs foot19** are defensive smoke/Koala counter-CC, not another Hidden killer. Transcript dispute: Musashi dice/value versus Shinobu delivery. [Cross-game CC assassin apex/value, Guard and delivery disputes](../../notes/list-building/dedicated-close-combat-assassins-apex-value.md).
