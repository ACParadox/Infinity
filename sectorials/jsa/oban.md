---
schema_version: 1
reference_type: sectorial
status: partial
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

## November 2026 Army profile update

**Precedence:** These corrections replace conflicting archived profile values; unchanged fields retain the original pin. Roster indexes and Fireteam charts are not fully reconciled; status is partial.

Source: [SITREP 5.7.4](https://www.infinitytheclassifieds.com/sitrep), November 25; Army backup commit `e2a8532270a039796db45bd07b1d111dc7bc8311`, revision `7.26329.480` (initial release).

- **Ryūken:** Surprise Attack (-3) is common to all options, including both SMG options.


## Overview and provenance

**Faction pick/avoid research (23 Oct 2026):** [Transcript-backed three-JSA-sectorial must-have, go-to and avoid comparison](../../notes/factions/references/oban_refs.md#must-have--go-to--avoid--source-backed-recommendations-2026). Opinions are tactical evidence, not alterations to the canonical roster and Fireteam rules.

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

**November 25 profile correction (overrides archived fields):** Surprise Attack (-3) is common to all options, including both SMG options.

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

## Validated competitive Fireteam examples — 2026-11-19

**Calculation baseline:** [Pinned Army backup 7.26246.159](https://github.com/massayoshi/infinity-army-backup/tree/6b79f39a3abbf5cd3d837fb9dc65e411fc35244b/n5), N5.3/ITS 18; [Fireteam formation](https://infinitythewiki.com/Fireteams%3A_Basic_Rules), [levels](https://infinitythewiki.com/Fireteam_Bonuses), [chart restrictions](https://infinitythewiki.com/Fireteams_Chart), [Peripheral (Ancillary)](https://infinitythewiki.com/Peripheral). An exact option ID is provided for every model; each quoted price is **points/SWC**. Team total is not an entire 300-point roster. `+1 SWC` Lieutenant options **increase army SWC allowance** and are not expenditure.

**Bonus level = most models with the same Unit name or matching bracketed counts-as label**, not automatically the number of models. L1 linked Orders; L2 BS Attack (+1 SD); L3 +3 Discover/+1 Dodge; L4 +1 BS; L5 Sixth Sense. Duo is **2** at creation, Haris **3**, Core **3–5**. Surviving two-model Haris is still a Haris, not a newly created Duo. Same Combat Group, coherency, no eligible marker/infiltration/airborne/suppressive/Null/Isolated troopers; deployed active Peripherals and their Controllers cannot be in a team (Ancillary exception described below).

**Legality:** maximum **1 Core, 1 Haris, unlimited Duos**. Keisotsu Haris/Core requires ≥1 Keisotsu; Domaru Duo/Haris/Core requires ≥1 Domaru. Ōban Duo/Haris requires ≥1 from the **Domaru/Karakuri/Shikami source-choice set**. Banzai Duo/Haris needs Tankō; Aragoto Duo/Haris needs Aragoto. **Kempeitai (max 3)** and **Yuriko FTO options 1–2 (max 1)** are Wildcards and count as Keisotsu. Tankō and Oyama count as Domaru *in a Domaru team*; Mushashi **FTO 25/0.5** counts as Tankō *in Banzai*; Kuroshi counts as Aragoto. The **Irregular 21/0 Mushashi is not a Banzai option**. Do not infer that all named Wildcards boost a different team's level.

**Evidence:** [#109](../../notes/battle-reports/101-110-n5-battle-report-tactical-analysis.md) explicitly fielded five-person Keisotsu, double Karakuri and Kuroshi/Aragoto/Rui Shi; [#069](../../notes/battle-reports/061-070-n5-battle-report-tactical-analysis.md) fielded five-member Keisotsu (custom mission defeat); [#236](../../notes/battle-reports/231-240-n5-battle-report-tactical-analysis.md) explicitly had a **four**, not five, Keisotsu Core; [#113](../../notes/battle-reports/111-120-n5-battle-report-tactical-analysis.md) described Kuroshi/Aragoto Duo. [Ōban tactical guide](../../notes/factions/oban.md#battle-report-tested-oban-army-shells-and-fireteam-audit-2026-11-03).

**Evidence categories:** Explicit/Reported = a team was narrated in an indexed report; Adapted = rules-legal choice inspired by that report without asserting identical loadouts; Proposed = validated option and rules theorycraft, not a proven match result. **Best** is an editorial judgment, not win-rate data. Costs below are drawn from the pinned Army options, and level from the current chart's equivalence labels.

| Members | Formation | Exact profiles, per-member points/SWC and option ID | Team total | FT level | Tactical role and evidence |
|---:|---|---|---|:---:|---|
| 2 | Duo: ŌBAN Fireteams | **Best Karakuri Duo** — Karakuri E/Mitter FO **(31/0, option 5)**; Karakuri Mk12 FO **(38/0, option 4)** | **69 pts / 0 SWC** | **L2** | Structure 3 mission anchors with E/M and direct fire; L2. **Evidence:** Explicit #109. |
| 2 | Duo: ŌBAN Fireteams | **Shika-kuri Duo** — Shikami Eclipse Contender **(42/0, option 1)**; Karakuri Heavy Shotgun FO **(31/0, option 1)** | **73 pts / 0 SWC** | **L1** | Mobile vertical scorer and durable scorer; only L1. **Evidence:** Guide architecture, proposed. |
| 2 | Duo: Aragoto Fireteams | **Best budget bike Duo** — Kuroshi Smoke GL FO **(26/0, option 3736)**; Aragoto Boarding Shotgun **(13/0, option 530)** | **39 pts / 0 SWC** | **L2** | Kuroshi counts as Aragoto for L2. **Evidence:** Explicit #113. |
| 2 | Duo: Banzai Fireteams | **Disco/Mushashi delivery** — Tankō Disco Baller **(19/0, option 7)**; Mushashi FTO Regular **(25/0.5, option 2)** | **44 pts / 0.5 SWC** | **L2** | Only FTO Mushashi is legal; counts as Tankō for L2. **Evidence:** Guide architecture, proposed. |
| 2 | Duo: Domaru Fireteams | **LT/NCO attackers** — Domaru LT +1 Order E/M **(23/0, option 7)**; Daiyōkai HMG NCO **(50/1, option 3)** | **73 pts / 1 SWC** | **L1** | Command economy, but only L1: Daiyōkai does not count as Domaru. **Evidence:** Proposed. |
| 2 | Duo: Domaru Fireteams | **Cheap samurai/Disco** — Domaru Chain Rifle E/M **(20/0, option 2)**; Tankō Disco Baller **(19/0, option 7)** | **39 pts / 0 SWC** | **L2** | Tankō counts as Domaru in this chart; L2. **Evidence:** Proposed. |
| 3 | Haris: Aragoto Fireteams | **Best played smoke/MSV mobile Haris** — Kuroshi Smoke GL FO **(26/0, option 3736)**; Aragoto Boarding Shotgun **(13/0, option 530)**; Rui Shi MSV2 Spitfire **(23/1, option 1)** | **62 pts / 1 SWC** | **L2** | Two Aragoto-equivalent models for L2; Rui Shi shoots through ordinary Smoke, not Eclipse. **Evidence:** Explicit #109. |
| 3 | Haris: ŌBAN Fireteams | **Best Shika-kuri holding Haris** — Shikami Eclipse Contender **(42/0, option 1)**; Karakuri E/Mitter FO **(31/0, option 5)**; Karakuri Mk12 FO **(38/0, option 4)** | **111 pts / 0 SWC** | **L2** | Shikami crosses/handles terrain, two Karakuri hold; L2. **Evidence:** Guide architecture, proposed. |
| 3 | Haris: Domaru Fireteams | **Premium LT/NCO/Disco Haris** — Domaru LT +1 Order E/M **(23/0, option 7)**; Daiyōkai HMG NCO **(50/1, option 3)**; Tankō Disco Baller **(19/0, option 7)** | **92 pts / 1 SWC** | **L2** | Strong Order/visibility economy; Domaru+Tankō give L2, not L3. **Evidence:** Guide architecture, proposed. |
| 3 | Haris: Banzai Fireteams | **Full Banzai CC/ARO Haris** — Tankō Disco Baller **(19/0, option 7)**; Tankō Missile Launcher **(26/1.5, option 4)**; Mushashi FTO Regular **(25/0.5, option 2)** | **70 pts / 2 SWC** | **L3** | All three count as Tankō for L3. **Evidence:** Proposed. |
| 3 | Haris: Keisotsu Fireteams | **Cheap Keisotsu/CoC Haris** — Keisotsu Thunderbolt **(12/0, option 12)**; Keisotsu Forward Observer **(11/0, option 7)**; Kempeitai BSG CoC **(17/0, option 4)** | **40 pts / 0 SWC** | **L3** | Kempeitai counts as Keisotsu, therefore L3. **Evidence:** Proposed. |
| 3 | Haris: ŌBAN Fireteams | **Triple Karakuri scoring** — Karakuri E/Mitter FO **(31/0, option 5)**; Karakuri MULTI Rifle FO **(35/0, option 3)**; Karakuri Mk12 FO **(38/0, option 4)** | **104 pts / 0 SWC** | **L3** | All three match; L3, but expensive and Hackable. **Evidence:** Proposed. |
| 3 | Core: Keisotsu Fireteams | **Minimal three-model Core** — Keisotsu Thunderbolt **(12/0, option 12)**; Keisotsu Hacker CrazyKoala **(16/0.5, option 4)**; Kempeitai BSG CoC **(17/0, option 4)** | **45 pts / 0.5 SWC** | **L3** | A Core can begin at three; Kempeitai equivalence yields L3. **Evidence:** Proposed. |
| 4 | Core: Keisotsu Fireteams | **Best played four-model Core** — Keisotsu Combi Lieutenant **(10/0.5, option 9)**; Keisotsu Thunderbolt **(12/0, option 12)**; Keisotsu Thunderbolt **(12/0, option 12)**; Keisotsu Thunderbolt **(12/0, option 12)** | **46 pts / 0.5 SWC** | **L4** | Four-person L4, not a five-person Core, as in the match. **Evidence:** Explicit #236. |
| 5 | Core: Keisotsu Fireteams | **Best utility five-model Core** — Keisotsu Combi Lieutenant **(10/0.5, option 9)**; Keisotsu Hacker CrazyKoala **(16/0.5, option 4)**; Keisotsu Thunderbolt **(12/0, option 12)**; Keisotsu Paramedic **(12/0, option 8)**; Yuriko FTO Panzerfaust Engineer **(23/0, option 2)** | **73 pts / 1 SWC** | **L5** | Yuriko counts as Keisotsu; all five qualify for L5. **Evidence:** Adapted from #109. |
| 5 | Core: Keisotsu Fireteams | **Best reported defensive five-model Core** — Keisotsu Hacker CrazyKoala **(16/0.5, option 4)**; Keisotsu Thunderbolt **(12/0, option 12)**; Keisotsu Thunderbolt **(12/0, option 12)**; Keisotsu Paramedic **(12/0, option 8)**; Kempeitai BSG CoC **(17/0, option 4)** | **69 pts / 0.5 SWC** | **L5** | Five matching/Keisotsu-equivalent members yield L5. **Evidence:** Explicit #069 (custom mission, defeat). |
| 5 | Core: Domaru Fireteams | **Full Domaru-equivalent assault Core** — Domaru LT +1 Order E/M **(23/0, option 7)**; Tankō Disco Baller **(19/0, option 7)**; Tankō Missile Launcher **(26/1.5, option 4)**; Tankō Blitzen Light Shotgun **(18/0, option 1)**; Oyama Chain Rifle **(28/0, option 1)** | **114 pts / 1.5 SWC** | **L5** | Three Tankō + Oyama all count as Domaru, yielding L5. **Evidence:** Proposed. |
| 5 | Core: Keisotsu Fireteams | **Mixed Daiyōkai gun Core** — Keisotsu Combi Lieutenant **(10/0.5, option 9)**; Keisotsu Hacker CrazyKoala **(16/0.5, option 4)**; Keisotsu Thunderbolt **(12/0, option 12)**; Keisotsu Paramedic **(12/0, option 8)**; Daiyōkai HMG NCO **(50/1, option 3)** | **100 pts / 2 SWC** | **L4** | L4: Daiyōkai does NOT count as Keisotsu; gun ceiling traded for the final FT bonus. **Evidence:** Proposed. |

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

**Tactical and purchasing analysis:** [Ōban faction guide](../../notes/factions/references/oban_refs.md#n53-tactical-cross-references-battle-reports-and-purchasing-audit). This file remains authoritative for roster, profiles, Fireteams, provenance and validation.
