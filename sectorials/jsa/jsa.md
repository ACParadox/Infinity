---
schema_version: 1
reference_type: faction
status: current
sectorial_id: 1101
sectorial_slug: jsa
sectorial_name: Vanilla JSA
parent_faction: JSA
parent_faction_id: 1101
rules_baseline: N5.3
army_source_version: "7.26246.159"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-16
coverage: "43 standard Army-1101 logical units; complete standard profiles/loadouts and vanilla AVA; optional Kaizoku Spec-Ops and JSA Team-Ops hooks; complete Vanilla JSA Fireteam chart and reverse access index; roster identity/peripheral notes; linked JSA Reinforcements Army 1199 boundary"
---

# Vanilla JSA — N5.3 faction reference

## Overview and provenance
**Tactical companion:** [Vanilla JSA — transcript-reviewed list building, opposing opinions, TAGs/REMs and vehicle boundaries](../../notes/factions/vanilla-jsa.md) (research refresh **2026-10-23**). Unit, profile, AVA and Fireteam legality below remain **canonical**.


This file is the repository-native factual reference for **Vanilla JSA / Japanese Secessionist Army (Army ID `1101`)** under the N5.3 baseline. It records the standard Army-1101 roster, profiles/loadouts, vanilla AVA, the current limited vanilla Fireteam chart, optional game-mode hooks, identity/peripheral relations, and the linked JSA Reinforcements boundary.

Primary sources:

- Corvus Belli Army-derived snapshot mirrored by `massayoshi/infinity-army-backup`.
- Pinned source commit: `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b` (`army: N5.3 + ITS18`, committed 2026-09-03).
- Army dataset: `n5/jsa/7.26246.159.json`.
- Source blob: `4024c5e5584464243d28575f4459fefd46d2f8f3`.
- Army version: **7.26246.159**.
- Army ID: **1101**.
- Reinforcements list ID exposed by the dataset: **1199**.
- Cross-check/reference model: InfinityDB commit `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: **N5.3 + N5 FAQ v0.1**.

Version-selection note: the backup directory also contains `7.2668.375.json`, but that file was committed on 2026-03-09. The selected `7.26246.159.json` was committed on 2026-09-03 and is therefore the later N5.3 snapshot despite lexicographic filename ordering.

Coverage policy:

- The **43 standard logical roster records** whose source faction availability includes Army `1101` are included below.
- Generic Soldier-of-Fortune / mercenary-catalogue records carried in the aggregate payload with `factions: []` are **not** standard Vanilla JSA roster entries and are excluded.
- This means sectorial-only or catalogue-only records such as the current Ōban Yojimbo/Yuan Yuan/Samsa inclusions are not silently imported into Vanilla JSA.
- **Kaizoku Spec-Ops** (`1924`) and **JSA Team-Ops** (`1938`) are optional-mode hooks and are listed separately.
- Composite states and Peripherals stay under their parent logical unit rather than being counted as separate roster entries.
- Fireteam legality comes from the canonical Army-1101 chart below. Ōban and Shindenbutai Fireteam charts do not apply to Vanilla JSA.

## Faction summary

| Field | Value |
|---|---|
| Faction | Vanilla JSA |
| Parent faction | JSA |
| Army ID | `1101` |
| Rules baseline | N5.3 + FAQ v0.1 |
| Army source | `7.26246.159` |
| Standard logical roster records | 43 |
| Optional-mode records | Kaizoku Spec-Ops; JSA Team-Ops |
| Linked Reinforcement roster | JSA Reinforcements, Army ID `1199` |
| Fireteam chart | yes — limited vanilla chart |

## Fireteam chart limits and faction-level restrictions

| Constraint | Value / wording |
|---|---|
| Core | 0 |
| Haris | up to 1 |
| Duo | up to 2 |
| Standard Fireteam rows | JSA Fireteams I; JSA Fireteams II |
| Wildcards | none exposed separately by the pinned vanilla chart |
| Main/Reinforcement mixing | Keep standard Army `1101` and Reinforcement Army `1199` distinct |
| Shizoku restriction | JSA Fireteams I uses `SHIZOKU FTO`: profiles 1–2 only |
| Yuriko restriction | Fireteam access is `YURIKO ODA FTO`: profiles 1–2 only; profile 3 is excluded |

## Standard roster index

`Total` below represents source AVA `255`.

| Unit ID | Unit | AVA | Type | Classification | Regularity | Notes |
|---:|---|---:|---|---|---|---|
| 996 | Ryūken Unit-9 | 2 | MI | Spec. Trained Troops | Regular | Camo/FD attack profiles; KHD option |
| 157 | Oniwaban | 1 | SK | Elite Troops | Regular | Hidden Deployment infiltrator |
| 1789 | Genbutai | 1 | MI | Veteran Troops | Regular | Engineer / specialist / NCO options |
| 1822 | Shizoku Kōgeki-tai | 1 | HI | Veteran Troops | Regular | JSA Fireteams I, **FTO 1–2 only** |
| 50 | Warcors | 1 | LI | Mercenary Troops | Irregular | Journalist |
| 1791 | Sōhei Tsugekitai | 1 | MI | Veteran Troops | Regular | Frenzy; MA3 |
| 223 | Miyamoto Mushashi | 1 | WB | Character | profile-dependent | JSA Fireteams I |
| 1829 | Shurayuki | 1 | MI | Veteran Troops | Regular | JSA Fireteams I/II |
| 162 | Yáopú Pangguling | 2 | REM | Support Troops | Regular | Baggage / EVO / Repeater |
| 160 | Yáoxiè Lù Duān | 2 | REM | Support Troops | Regular | Holoprojector, MSV1 |
| 154 | Karakuri Special Project | 2 | HI | Spec. Trained Troops | Regular | JSA Fireteams II |
| 144 | Keisotsu Butai | Total | LI | Line Troops | Regular | cheap line infantry |
| 1830 | Atom Aibōt | 2 | REM | Support Troops | Regular | Sensor/FO/Repeater |
| 1832 | Uran Aibōt | 1 | REM | Support Troops | Regular | Guided Missile Launcher |
| 161 | Yáozăo | 3 | REM | Support Troops | Peripheral | Servant |
| 167 | Raiden Seibutai | 3 | MI | Elite Troops | Regular | Hidden Deployment heavy weapon |
| 163 | Shinobu Kitsune | 1 | SK | Character | Regular | elite Hidden Deployment infiltrator |
| 1940 | Ioann Bann | 1 | WB | Character | Irregular | JSA Fireteams I |
| 1790 | Kyoshō Saibāyunitto | 1 | LI | Spec. Trained Troops | Regular | HD/KHD |
| 158 | Tokusetsu Butai | 2 | LI | Support Troops | Regular | Doctor/Engineer |
| 1817 | Senku Troops | 5 | LI | Line Troops | Regular | Lt/FO/Paramedic/Commlink options |
| 1826 | Nokizaru Unit | 1 | SK | Spec. Trained Troops | Regular | MSV1; KHD/FO |
| 159 | Yáoxiè Rui Shi | 2 | REM | Support Troops | Regular | JSA Fireteams II |
| 1788 | Mechazoid Sōkōrentai | 1 | TAG | Mechanized Troops | Regular | JSA Fireteams I; Tactical Awareness |
| 1002 | Daiyōkai Dengekitai | 1 | HI | Headquarters Troops | Regular | JSA Fireteams I/II; NCO |
| 999 | Tankō Zensenbutai | 2 | HI | Line Troops | Regular, Impetuous | heavy ARO/assault infantry |
| 1823 | Hatamoto Imperial Guard | 1 | HI | Headquarters Troops | Regular | NCO; Lt +1 Order/+1 SWC options |
| 147 | Kempeitai | 2 | LI | Spec. Trained Troops | Regular | Chain of Command / MSV2 options |
| 668 | Saito Tōgan | 1 | SK | Character | Regular | Hidden Deployment, smoke |
| 1821 | Jizamurai Hanryodan | 1 | MI | Elite Troops | Regular | JSA Fireteams I |
| 156 | O-Yoroi Kidobutai | 1 | TAG | Mechanized Troops | Regular | JSA Fireteams I; Tactical Awareness |
| 1827 | Kyojin Killers | 1 | SK | Spec. Trained Troops | Irregular | FD assault skirmisher |
| 1833 | Robio Aibōt | 1 | REM | Support Troops | Regular | Repeater |
| 164 | Takeshi “Neko” Oyama | 1 | HI | Character | Regular | JSA Fireteams II; Tactical Awareness |
| 1019 | Yuriko Oda | 1 | LI | Character | Regular | JSA Fireteams I/II, **FTO 1–2 only** |
| 1820 | Teishin Guntai | 2 | MI | Spec. Trained Troops | Regular | Combat Jump; HD/KHD/FO |
| 1825 | Kurayami Ninjas | 1 | SK | Spec. Trained Troops | Regular | Hidden Deployment; HD |
| 1828 | Taguraidā, JSA TAG Support Pilots | 1 | LI | Support Troops | Regular | Mechazoid/O-Yoroi pilot profiles |
| 149 | Aragoto Senkenbutai | 2 | LI | Spec. Trained Troops | Regular, Impetuous | fast attack/hacker bike |
| 1831 | Garon Aibōt | 2 | REM | Support Troops | Regular | Total Reaction / smoke GL option |
| 135 | Ninjas | 2 | SK | Spec. Trained Troops | Regular | Hidden Deployment; HD/KHD/FO |
| 152 | Domaru Butai | 2 | HI | Line Troops | Regular | JSA Fireteams I/II |
| 773 | Shikami | 2 | HI | Elite Troops | Regular | Eclipse; mobile specialist |

### Optional-mode entries

| Unit ID | Unit | Mode | Standard roster status |
|---:|---|---|---|
| 1924 | Kaizoku Spec-Ops | Infinity Spec-Ops | optional only |
| 1938 | JSA Team-Ops | Infinity Team-Ops | optional only |

## Unit details

Notation: stats are `MOV CC BS PH WIP ARM BTS W/STR S`. Source option IDs are retained because profile legality and otherwise-similar loadouts can depend on them.

### Ryūken Unit-9 — `ryuken-unit-9`

**Unit ID:** 996 — **AVA:** 2 — MI, Spec. Trained Troops, Regular.  
**Stats:** `10-10 17 12 11 14 2 3 1 2`.  
**Rules/equipment:** X-Visor, Courage, Mimetism (-6), Minelayer, Decoy (1).

- **Option 1:** **23 / 1.5** — Heavy Rocket Launcher, Shock Mine, Heavy Pistol, CC Weapon; Surprise Attack (-3), Camouflage (1 Use).
- **Option 2:** **22 / 0.5** — Submachine Gun, Shock Mine, D-Charges, Breaker Pistol (+1B), CC Weapon; Forward Deployment (+20).
- **Option 3:** **25 / 0.5** — option-2 weapons; Killer Hacking Device, Hacker; Forward Deployment (+20).

### Oniwaban — `oniwaban`

**Unit ID:** 157 — **AVA:** 1 — SK, Elite Troops, Regular.  
**Stats:** `10-10 24 11 12 14 1 0 1 2`.  
**Rules:** Martial Arts L4, Surprise Attack (-3), Camouflage, Courage, Hidden Deployment, Dodge (+5), Infiltration (PH=18), Mimetism (-6), Stealth, Terrain (Total).

- **Option 1:** **30 / 0** — Boarding Shotgun, Nanopulser, Pistol, Monofilament CC Weapon, E/M CC Weapon (PS=5).
- **Option 2:** **29 / 0** — Submachine Gun, Nanopulser, Pistol, Monofilament CC Weapon, E/M CC Weapon (PS=5).
- **Option 3 Lieutenant:** **30 / 1** — option-1 weapons; Lieutenant.

### Genbutai — `genbutai`

**Unit ID:** 1789 — **AVA:** 1 — MI, Veteran Troops, Regular.  
**Stats:** `10-10 18 13 11 13 3 6 1 2`.  
**Rules:** BS Attack (SR-1), Warhorse, Immunity (AP), Immunity (Shock), Religious Troop.

- **Option 1:** **18 / 0** — Boarding Shotgun, Chain-colt, Breaker Pistol, PARA CC Weapon (-6).
- **Option 2:** **23 / 0** — Engineer, GizmoKit; Submachine Gun, Panzerfaust, D-Charges, Breaker Pistol, PARA CC Weapon (-6).
- **Option 3:** **26 / 0** — Specialist Operative; MULTI Rifle, Heavy Flamethrower, D-Charges, Breaker Pistol, PARA CC Weapon (-6).
- **Option 4:** **20 / 0** — Paramedic, MediKit; Boarding Shotgun, Chain-colt, Breaker Pistol, PARA CC Weapon (-6).
- **Option 5:** **29 / 1** — NCO; Red Fury, Breaker Pistol, PARA CC Weapon (-6).

### Shizoku Kōgeki-tai — `shizoku-kogeki-tai`

**Unit ID:** 1822 — **AVA:** 1 — HI, Veteran Troops, Regular.  
**Stats:** `15-5 22 13 14 13 5 6 2 2`.  
**Rules/equipment:** Hackable; Martial Arts L3, Berserk, Courage, Dodge (+5), Frenzy, Mimetism (-3), Stealth.

- **Option 1 — SHIZOKU FTO:** **43 / 1.5** — AP HMG, Chain Rifle, Pistol, AP + DA CC Weapon.
- **Option 2 — SHIZOKU FTO:** **33 / 1.5** — Heavy Rocket Launcher (+1B), Assault Pistol, AP + DA CC Weapon.
- **Option 3:** **38 / 1.5** — option-2 weapons; Strategic Deployment; non-FTO.
- **Fireteam:** JSA Fireteams I, **options 1–2 only**.

### Warcors — `warcors-war-correspondents`

**Unit ID:** 50 — **AVA:** 1 — LI, Mercenary Troops, Irregular.  
**Stats:** `10-10 11 9 11 13 0 0 1 2`. Journalist.

- **Option 1:** **3 / 0** — Flash Pulse, Stun Pistol, PARA CC Weapon (-3); 360º Visor.
- **Option 2:** **3 / 0** — Flash Pulse, Stun Pistol, PARA CC Weapon (-3); Sixth Sense.

### Sōhei Tsugekitai — `s-hei-tsugekitai`

**Unit ID:** 1791 — **AVA:** 1 — MI, Veteran Troops, Regular.  
**Stats:** `10-10 23 11 13 13 3 3 1 2`.  
**Rules:** Frenzy, Martial Arts L3, Dodge (+5), Immunity (Shock), Stealth, Religious Troop.

- **Option 1:** **16 / 0** — Submachine Gun, Grenades, Pistol, AP + Shock CC Weapon.
- **Option 2:** **16 / 0** — Pulzar, Grenades, Assault Pistol, AP + Shock CC Weapon.

### Miyamoto Mushashi — `miyamoto-mushashi`

**Unit ID:** 223 — **AVA:** 1 — WB, Character; regularity is option-dependent.  
**Stats:** `15-10 25 9 14 15 1 3 1 2`.  
**Rules:** Martial Arts L5, CC Attack (AP), Courage, Dodge (+5), Immunity (ARM), Stealth, No Wound Incapacitation.

- **Option 1:** **21 / 0** — Irregular; Chain Rifle, Tactical Bow, Flash Pulse, Pistol, EXP CC Weapon (PS=4).
- **Option 2 — MIYAMOTO MUSHASHI FTO:** **25 / 0.5** — Regular; same weapons.
- **Fireteam:** JSA Fireteams I. The vanilla chart names the unit without an FTO-only restriction.

### Shurayuki — `shurayuki`

**Unit ID:** 1829 — **AVA:** 1 — MI, Veteran Troops, Regular.  
**Stats:** `10-10 23 12 12 13 2 3 1 2`.  
**Rules/equipment:** Holomask, X-Visor; Martial Arts L4, Courage, Dodge (+5), Immunity (Shock), Stealth, No Wound Incapacitation, Religious Troop.

- **Option 1:** **30 / 0** — MULTI Rifle, Nanopulser, Pistol, Viral CC Weapon.
- **Fireteams:** JSA Fireteams I and II.

### Yáopú Pangguling — `yaopu-pangguling`

**Unit ID:** 162 — **AVA:** 2 — REM, Support Troops, Regular.  
**Stats:** `10-10 13 11 10 13 2 3 STR1 4`.  
**Rules/equipment:** Baggage, Remote Presence, Courage.

- **Option 1:** **8 / 0** — Deactivator, Repeater; PARA CC Weapon (-3).
- **Option 2:** **14 / 0.5** — EVO Hacking Device, Hacker; PARA CC Weapon (-3).
- **Option 3:** **17 / 0** — Repeater, Total Reaction; Combi Rifle, PARA CC Weapon (-3).
- **Option 4 — PANGGULING FTO:** **12 / 0** — Repeater; Light Shotgun, PARA CC Weapon (-3). The vanilla chart has no Pangguling row.

### Yáoxiè Lù Duān — `yaoxie-lu-duan`

**Unit ID:** 160 — **AVA:** 2 — REM, Support Troops, Regular.  
**Stats:** `15-10 13 12 10 13 1 6 STR1 4`.  
**Rules/equipment:** Holoprojector, Multispectral Visor L1, Remote Presence, Courage, Surprise Attack (-3), BS Attack (+1B).

- **Option 1:** **24 / 0** — Mk12, Heavy Flamethrower, E/M Mine, PARA CC Weapon (-3).
- **Option 2:** **20 / 0** — Thunderbolt, E/M Carbine, E/M Mine, PARA CC Weapon (-3).

### Karakuri Special Project — `karakuri-special-project`

**Unit ID:** 154 — **AVA:** 2 — HI, Spec. Trained Troops, Regular; Structure 3.  
**Stats:** `10-10 10 13 10 13 3 6 STR3 2`.  
**Rules:** Courage, GizmoKit (PH=12), Immunity (Enhanced), Forward Observer, Remote Presence.

- **Option 1:** **31 / 0** — Heavy Shotgun, Chain Rifle, Panzerfaust, Flash Pulse, Pistol, CC Weapon.
- **Option 3:** **35 / 0** — MULTI Rifle, Chain Rifle, Panzerfaust, Flash Pulse, Pistol, CC Weapon.
- **Option 4:** **38 / 0** — Mk12, Chain Rifle, Panzerfaust, Flash Pulse, Pistol, CC Weapon.
- **Option 5:** **31 / 0** — E/Mitter, Chain Rifle, Panzerfaust, Flash Pulse, Pistol, CC Weapon.
- **Fireteam:** JSA Fireteams II.

### Keisotsu Butai — `keisotsu`

**Unit ID:** 144 — **AVA:** Total (`255`) — LI, Line Troops, Regular.  
**Stats:** `10-10 17 11 10 12 1 0 1 2`. Courage.

- **Option 1:** **10 / 0** — Combi Rifle, Pistol, CC Weapon.
- **Option 2:** **18 / 1** — HMG, Pistol, CC Weapon.
- **Option 3:** **15 / 1.5** — Missile Launcher, Pistol, CC Weapon.
- **Option 4:** **16 / 0.5** — Hacker, Hacking Device, ECM: Hacker (-6); Combi Rifle, CrazyKoala, Pistol, CC Weapon.
- **Option 7:** **11 / 0** — Forward Observer; Combi Rifle, Flash Pulse, Pistol, CC Weapon.
- **Option 8:** **12 / 0** — Paramedic, MediKit; Combi Rifle, Pistol, CC Weapon.
- **Option 9 Lieutenant:** **10 / 0.5** — Combi Rifle, Pistol, CC Weapon.
- **Option 10:** **12 / 0** — Commlink (+1), Specialist Operative; Combi Rifle, Pistol, CC Weapon.
- **Option 11:** **9 / 0** — AP Rifle, Pistol, CC Weapon.
- **Option 12:** **12 / 0** — Thunderbolt, Pistol, CC Weapon; BS Attack (-3 source modifier).
- **Option 13 Lieutenant:** **9 / 0.5** — AP Rifle, Pistol, CC Weapon.

### Atom Aibōt — `atom-aib-t`

**Unit ID:** 1830 — **AVA:** 2 — REM, Support Troops, Regular.  
**Stats:** `15-10 13 11 10 13 0 3 STR1 3`.  
**Rules/equipment:** Deactivator, Repeater, Triangulated Fire, Courage, Forward Observer, Remote Presence.

- **Option 1:** **15 / 0** — Combi Rifle, Flash Pulse, PARA CC Weapon (-3); Sensor.
- **Option 2:** **17 / 0** — Combi Rifle (source modifier retained), Flash Pulse (+1B), PARA CC Weapon (-3).

### Uran Aibōt — `uran-aib-t`

**Unit ID:** 1832 — **AVA:** 1 — REM, Support Troops, Regular.  
**Stats:** `15-10 13 12 10 13 0 3 STR1 3`.  
**Rules:** BS Attack (Guided), Courage, Remote Presence.

- **Option 1:** **16 / 1.5** — Missile Launcher, PARA CC Weapon (-3).

### Yáozăo — `yaozao`

**Unit ID:** 161 — **AVA:** 3 — REM, Support Troops; Peripheral (Servant).  
**Stats:** `15-10 11 8 10 13 0 3 STR1 1`.  
**Rules:** Peripheral (Servant), Courage, Mimetism (-3).

- **Option 1:** **3 / 0** — PARA CC Weapon (-3); no Order of its own.

### Raiden Seibutai — `raiden-seibutai`

**Unit ID:** 167 — **AVA:** 3 — MI, Elite Troops, Regular.  
**Stats:** `10-10 16 13 11 13 3 3 1 2`.  
**Rules/equipment:** X-Visor; Hidden Deployment, Minelayer, Mimetism (-3), Surprise Attack (-3), Immunity (Shock), Courage.

- **Option 2:** **25 / 1.5** — Heavy Rocket Launcher, Shock Mine, Breaker Pistol, CC Weapon.
- **Option 3:** **33 / 2** — Missile Launcher, Shock Mine, Breaker Pistol, CC Weapon.

### Shinobu Kitsune — `oniwaban-shinobu-kitsune`

**Unit ID:** 163 — **AVA:** 1 — SK, Character, Regular.  
**Stats:** `10-10 25 12 13 14 1 3 1 2`.  
**Rules:** Martial Arts L5, Surprise Attack (-3), Camouflage, Courage, Hidden Deployment, Dodge (+5), Infiltration (PH=19), Mimetism (-6), Stealth, Terrain (Total), Climbing Plus.

- **Option 1:** **44 / 0.5** — Combi Rifle, Nanopulser, Smoke Grenades, Pistol, Monofilament CC Weapon.
- **Option 2 Lieutenant:** **44 / 0.5** — same loadout; Lieutenant.

### Ioann Bann, Varangian Dog-Warrior — `ioann-bann-varangian-dog-warrior`

**Unit ID:** 1940 — **AVA:** 1 — WB, Character, Irregular.

| State | MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Dogface | 15-10 | 22 | 11 | 14 | 13 | 2 | 3 | 3 | 2 |
| Dog-Warrior | 15-10 | 23 | 11 | 16 | 13 | 4 | 6 | 3 | 6 |

**Rules:** Martial Arts L3, Berserk, Dodge/Immunity transformation package, No Cover, Super-Jump, Religious Troop, Impetuous as encoded by the source states.

- **Option 2:** **30 / 0** — Chain Rifle (+1B), Viral Tactical Bow (+1SD), Grenades, AP Heavy Pistol (+1B), AP + T2 CC Weapon.
- **Fireteam:** JSA Fireteams I.

### Kyoshō Saibāyunitto — `kyosh-saibayunitto`

**Unit ID:** 1790 — **AVA:** 1 — LI, Spec. Trained Troops, Regular.  
**Stats:** `10-10 17 11 10 13 1 6 1 2`.  
**Base:** Hacker with source upgrade `Total Control (SR-2)`.

- **Option 1:** **20 / 0.5** — Hacking Device; Combi Rifle, Cybermine, Breaker Pistol, CC Weapon.
- **Option 2:** **20 / 0** — Killer Hacking Device; MULTI Rifle, Cybermine, Breaker Pistol, CC Weapon.

### Tokusetsu Butai — `tokusetsu-butai`

**Unit ID:** 158 — **AVA:** 2 — LI, Support Troops, Regular.  
**Stats:** `10-10 15 11 10 13 1 0 1 2`. Courage.

- **Option 1:** **14 / 0** — Doctor, MediKit; Combi Rifle, Pistol, CC Weapon.
- **Option 2:** **14 / 0** — Engineer, Deactivator, GizmoKit; Combi Rifle, D-Charges, Pistol, CC Weapon.
- **Option 3:** **15 / 0** — Engineer, Deactivator, GizmoKit, Deployable Cover; option-2 weapons.
- **Option 4:** **17 / 0** — Engineer, Deactivator, GizmoKit; Combi Rifle, D-Charges, Armed Turret (Combi Rifle), Pistol, CC Weapon.

### Senku Troops — `senku-troops`

**Unit ID:** 1817 — **AVA:** 5 — LI, Line Troops, Regular.  
**Stats:** `10-10 15 11 10 12 0 3 1 2`. Courage.

- **Option 1:** **9 / 0** — Combi Rifle, Pistol, CC Weapon.
- **Option 2:** **17 / 1** — HMG, Pistol, CC Weapon.
- **Option 3:** **11 / 0** — Shock Marksman Rifle, Pistol, CC Weapon.
- **Option 4:** **11 / 0** — Commlink, Specialist Operative; Combi Rifle, Pistol, CC Weapon.
- **Option 6:** **10 / 0** — Forward Observer; Combi Rifle, Flash Pulse, Pistol, CC Weapon.
- **Option 7:** **11 / 0** — Paramedic, MediKit; Combi Rifle, Pistol, CC Weapon.
- **Option 8 Lieutenant:** **9 / 0.5** — Combi Rifle, Pistol, CC Weapon.

### Nokizaru Unit — `nokizaru-unit`

**Unit ID:** 1826 — **AVA:** 1 — SK, Spec. Trained Troops, Regular.  
**Stats:** `10-10 23 12 12 13 0 6 1 2`.  
**Rules/equipment:** MSV1; Martial Arts L3, Courage, Forward Deployment (+2.5), Mimetism (-3), Stealth, Terrain (Zero-G), Climbing Plus.

- **Option 1:** **30 / 0** — MULTI Marksman Rifle, Silenced Pistol, Shock CC Weapon.
- **Option 2:** **27 / 0** — Submachine Gun, Shock Mine, D-Charges, Silenced Pistol, Shock CC Weapon; Killer Hacking Device.
- **Option 3:** **25 / 0** — Submachine Gun, Flash Pulse, Shock Mine, D-Charges, Silenced Pistol, Shock CC Weapon; Forward Observer.

### Yáoxiè Rui Shi — `yaoxie-rui-shi`

**Unit ID:** 159 — **AVA:** 2 — REM, Support Troops, Regular.  
**Stats:** `15-10 13 12 10 13 1 6 STR1 4`.  
**Rules/equipment:** Remote Presence, Courage, Repeater.

- **Option 1:** **23 / 1** — Spitfire, PARA CC Weapon (-3); Multispectral Visor L2.
- **Option 2:** **21 / 0.5** — Red Fury, Mine Dispenser (Shock), PARA CC Weapon (-3); Multispectral Visor L1.
- **Fireteam:** JSA Fireteams II, max 1.

### Mechazoid Sōkōrentai — `mechazoid-sokorentai`

**Unit ID:** 1788 — **AVA:** 1 — TAG, Mechanized Troops, Regular.  
**Stats:** `15-10 23 13 15 13 6 6 STR3 6`.  
**Rules/equipment:** Hackable; ECM: Guided (-6); Martial Arts L2, BS Attack (SR-1), Tactical Awareness, Combat Instinct, Stealth, Climbing Plus, Religious Troop.

- **Option 1:** **66 / 1.5** — AP HMG, Pulzar, Panzerfaust, EXP CC Weapon; Tactical Awareness; includes Kobaruto.
- **Option 2:** **69 / 1.5** — Spitfire MULTI, Pulzar, Panzerfaust, EXP CC Weapon; Tactical Awareness; includes Kobaruto.
- **Option 3 Lieutenant:** **69 / 1.5** — option-2 weapons; Lieutenant + Tactical Awareness; includes Kobaruto.
- **Kobaruto Hojo-Bot:** Ancillary Peripheral, `10-10 / PH10 / WIP13 / ARM0 / BTS3 / STR1 / S1`; Courage, Dodge (+3), Mimetism (-3), Specialist Operative, Climbing Plus.
- **Fireteam:** JSA Fireteams I.

### Daiyōkai Dengekitai — `daiy-kai-dengekitai`

**Unit ID:** 1002 — **AVA:** 1 — HI, Headquarters Troops, Regular.  
**Stats:** `10-10 21 13 14 13 5 3 2 5`.  
**Rules:** Martial Arts L2, BS Attack (SR-1), Courage, Stealth, No Wound Incapacitation, NCO.

- **Option 1:** **46 / 0** — MULTI Marksman Rifle, Panzerfaust, Pistol, AP + DA CC Weapon (PS=4).
- **Option 2:** **47 / 1** — Red Fury, Panzerfaust, Pistol, AP + DA CC Weapon (PS=4).
- **Option 3:** **50 / 1** — HMG, Panzerfaust, Pistol, AP + DA CC Weapon (PS=4).
- **Fireteams:** JSA Fireteams I and II.

### Tankō Zensenbutai — `tank-zensenbutai`

**Unit ID:** 999 — **AVA:** 2 — HI, Line Troops; Regular, Impetuous.  
**Stats:** `15-5 23 13 13 13 3 3 2 2`.  
**Rules:** Martial Arts L2, Limited Cover, Courage, Dodge (+2.5), Stealth, Impetuous.

- **Option 1:** **18 / 0** — Blitzen, Light Shotgun, Pistol, Monofilament CC Weapon, Shock CC Weapon (PS=6).
- **Option 2:** **19 / 0** — Blitzen, Submachine Gun, Pistol, Monofilament CC Weapon, Shock CC Weapon (PS=6).
- **Option 3:** **19 / 0** — Flammenspeer, Contender, Pistol, Monofilament CC Weapon, Shock CC Weapon (PS=6).
- **Option 4:** **26 / 1.5** — Missile Launcher, Pistol, Monofilament CC Weapon, Shock CC Weapon (PS=6).
- **Option 7:** **19 / 0** — Blitzen, Light Shotgun, Disco Baller, Pistol, Monofilament CC Weapon, Shock CC Weapon (PS=6); Deactivator.

### Hatamoto Imperial Guard — `hatamoto-imperial-guard`

**Unit ID:** 1823 — **AVA:** 1 — HI, Headquarters Troops, Regular.  
**Stats:** `15-5 23 13 13 13 2 6 2 2`.  
**Rules/equipment:** Hackable; Nanoscreen, X-Visor; Martial Arts L4, Natural Born Warrior, Combat Instinct, Mimetism (-3), Specialist Operative, Stealth, Frenzy. Every current loadout has NCO.

- **Option 1:** **34 / 0** — Plasma Carbine, Heavy Pistol, Monofilament CC Weapon, E/M CC Weapon; NCO.
- **Option 2:** **40 / 1** — Red Fury, Heavy Pistol, Monofilament CC Weapon, E/M CC Weapon; NCO.
- **Option 3:** **41 / 1.5** — Spitfire, Heavy Pistol, Monofilament CC Weapon, E/M CC Weapon; NCO.
- **Option 4 Lieutenant:** **36 / +1 SWC** — option-1 weapons; Lieutenant (+1 Order), NCO.
- **Option 5 Lieutenant:** **38 / +1 SWC** — option-2 weapons; Lieutenant (+1 Order), NCO.
- **Option 6 Lieutenant:** **39 / +1 SWC** — option-3 weapons; Lieutenant (+1 Order), NCO.

### Kempeitai — `kempeitai`

**Unit ID:** 147 — **AVA:** 2 — LI, Spec. Trained Troops, Regular.  
**Stats:** `10-10 17 12 10 14 1 0 1 2`.  
**Rules:** Courage, Number 2, Sixth Sense.

- **Option 1:** **22 / 1** — Spitfire, Pistol, CC Weapon, PARA CC Weapon (-3).
- **Option 3:** **20 / 0** — Combi Rifle; Chain of Command.
- **Option 4:** **17 / 0** — Boarding Shotgun; Chain of Command.
- **Option 5:** **22 / 1** — Shock Marksman Rifle; Multispectral Visor L2.

### Saito Tōgan — `saito-togan`

**Unit ID:** 668 — **AVA:** 1 — SK, Character, Regular.  
**Stats:** `10-10 24 11 13 13 1 0 1 2`.  
**Rules/equipment:** Martial Arts L4, Surprise Attack (-3), Camouflage, Courage, Hidden Deployment, Dodge (+2.5), Infiltration, Mimetism (-6), Stealth, Terrain (Total), Bangbomb (+4).

- **Option 1:** **33 / 0** — T2 Boarding Shotgun, Smoke Grenades, Pistol, EXP CC Weapon (PS=4).

### Jizamurai Hanryodan — `jizamurai-hanryodan`

**Unit ID:** 1821 — **AVA:** 1 — MI, Elite Troops, Regular.  
**Stats:** `15-5 23 12 13 13 3 3 1 2`.  
**Rules:** Martial Arts L3, Courage, Combat Instinct, Mimetism (-3), Stealth, Climbing Plus, Immunity (Shock).

- **Option 1:** **21 / 0** — Light Shotgun, Pistol, DA CC Weapon.
- **Option 2:** **21 / 0** — Light Shotgun, Pistol, E/M CC Weapon.
- **Option 3:** **24 / 0** — Light Shotgun, E/Mitter, Pistol, DA CC Weapon.
- **Option 4:** **24 / 0** — Light Shotgun, Thunderbolt, Pistol, DA CC Weapon.
- **Option 5:** **22 / 0** — Submachine Gun, Pistol, DA CC Weapon.
- **Fireteam:** JSA Fireteams I.

### O-Yoroi Kidobutai — `o-yoroi-kidobutai`

**Unit ID:** 156 — **AVA:** 1 — TAG, Mechanized Troops, Regular.  
**Stats:** `15-10 23 14 16 13 7 6 STR3 7`.  
**Rules/equipment:** Hackable; ECM: Guided (-6); Martial Arts L2, BS Attack (SR-1), Courage, Dodge (+5), GizmoKit (PH=11), Minelayer, Tactical Awareness, Stealth.

- **Option 1:** **78 / 1.5** — MULTI HMG, Heavy Flamethrower, CrazyKoala, EXP CC Weapon (PS=3); includes Kobaruto.
- **Option 2 Lieutenant:** **78 / 1.5** — same loadout; Lieutenant; includes Kobaruto.
- **Kobaruto Ancillary Remote:** `10-10 / PH10 / WIP13 / ARM0 / BTS3 / STR1 / S1`; Peripheral (Ancillary), Courage, Dodge (+3), Mimetism (-3), Specialist Operative.
- **Fireteam:** JSA Fireteams I.

### Kyojin Killers — `kyojin-killers`

**Unit ID:** 1827 — **AVA:** 1 — SK, Spec. Trained Troops, Irregular.  
**Stats:** `10-10 21 11 13 12 0 0 1 2`.  
**Rules:** CC Attack (+1B), Surprise Attack (-3), Camouflage (1 Use), Forward Deployment (+20), Mimetism (-3), Stealth, Super-Jump, Terrain (Total), Religious Troop.

- **Option 1:** **18 / 0** — Light Flamethrower, Contender, Pistol, DA CC Weapon.
- **Option 2:** **15 / 0** — Heavy Flamethrower, Flammenspeer, Pistol, DA CC Weapon.

### Robio Aibōt — `robio-aib-t`

**Unit ID:** 1833 — **AVA:** 1 — REM, Support Troops, Regular.  
**Stats:** `15-15 13 8 11 13 0 3 STR1 3`.  
**Rules/equipment:** Repeater, Courage, Mimetism (-3), Remote Presence.

- **Option 1:** **7 / 0** — Flash Pulse, PARA CC Weapon (-3).

### Takeshi “Neko” Oyama — `domaru-takeshi-neko-oyama`

**Unit ID:** 164 — **AVA:** 1 — HI, Character, Regular.  
**Stats:** `15-5 24 12 14 14 3 6 2 2`.  
**Rules:** Martial Arts L3, CC Attack (Shock), BS Attack (SR-1), Courage, Dodge (+5), Frenzy, Tactical Awareness, Stealth, Berserk.

- **Option 1:** **28 / 0** — Chain Rifle, Contender, E/M Grenades, Breaker Pistol, E/M CC Weapon (PS=4), DA CC Weapon (PS=4).
- **Option 2 Lieutenant:** **28 / 0** — same loadout; Lieutenant.
- **Fireteam:** JSA Fireteams II.

### Yuriko Oda — `keisotsu-kaizoku-yuriko-oda`

**Unit ID:** 1019 — **AVA:** 1 — LI, Character, Regular.  
**Stats:** `10-10 15 12 11 13 1 3 1 2`.  
**Rules/equipment:** Engineer, Mimetism (-3), Minelayer, Courage; Deactivator, GizmoKit.

- **Option 1 — YURIKO ODA FTO:** **25 / 0** — Combi Rifle, E/Mitter, D-Charges, Shock Mine, Pistol, CC Weapon.
- **Option 2 — YURIKO ODA FTO:** **23 / 0** — Combi Rifle, Panzerfaust, D-Charges, Shock Mine, Pistol, CC Weapon.
- **Option 3:** **28 / 0.5** — option-1 weapons; Forward Deployment (+20); non-FTO.
- **Fireteams:** JSA Fireteams I and II, **options 1–2 only**.

### Teishin Guntai — `teishin-guntai`

**Unit ID:** 1820 — **AVA:** 2 — MI, Spec. Trained Troops, Regular.  
**Stats:** `10-10 21 11 12 13 2 3 1 2`.  
**Rules:** Martial Arts L1, Combat Jump, Parachutist, Stealth, Super-Jump (Jet Propulsion).

- **Option 1:** **19 / 0** — Boarding Shotgun, D-Charges, Shock Mine, Pistol, Shock CC Weapon.
- **Option 2:** **23 / 0.5** — Boarding Shotgun, D-Charges, Pistol, Shock CC Weapon; Hacking Device.
- **Option 3:** **21 / 0** — Boarding Shotgun, D-Charges, Pistol, Shock CC Weapon; Killer Hacking Device.
- **Option 4:** **19 / 0** — Submachine Gun, Flash Pulse, D-Charges, Shock Mine, Pistol, Shock CC Weapon; Forward Observer.

### Kurayami Ninjas — `kurayami-ninjas`

**Unit ID:** 1825 — **AVA:** 1 — SK, Spec. Trained Troops, Regular.  
**Stats:** `10-10 22 11 13 13 0 3 1 2`.  
**Rules/equipment:** Bangbomb (+4); Martial Arts L2, Surprise Attack (-3), Courage, Hidden Deployment, Dodge (+2.5), Mimetism (-3), Infiltration, Stealth, Super-Jump, Terrain (Zero-G).

- **Option 1:** **22 / 0** — Submachine Gun, Viral Mine, Pistol, DA CC Weapon.
- **Option 2:** **26 / 0.5** — Light Shotgun, Viral Mine, D-Charges, Pistol, DA CC Weapon; Hacking Device.
- **Option 3:** **23 / 0.5** — Submachine Gun, Viral Mine, Pistol, DA CC Weapon; Minelayer.

### Taguraidā, JSA TAG Support Pilots — `taguraida-jsa-tag-support-pilots`

**Unit ID:** 1828 — **AVA:** 1 — LI, Support Troops, Regular.  
**Stats:** `10-10 21 12 12 13 0 0 1 2`.  
**Rules:** Martial Arts L1, Courage, Stealth, TAGCom (`Dodge PH+3`, `GizmoKit PH+1`).

- **Option 1 — MECHAZOID PILOT:** **12 / 0** — Light Shotgun, Pistol, DA CC Weapon; Specialist Operative, GizmoKit.
- **Option 2 — O-YOROI PILOT:** **11 / 0** — Light Shotgun, Flash Pulse, D-Charges, Pistol, Shock CC Weapon; Forward Observer.

### Aragoto Senkenbutai — `aragoto-senkenbutai`

**Unit ID:** 149 — **AVA:** 2 — LI, Spec. Trained Troops; Regular, Impetuous.  
**Stats:** `20-15 16 12 11 13 2 0 1 4`.  
**Rules/equipment:** Motorcycle, Limited Cover, Courage, Dodge (+5), Mimetism (-3), Impetuous.

- **Option 529:** **20 / 1** — Spitfire, Boarding Pistol, CC Weapon.
- **Option 530:** **13 / 0** — Boarding Shotgun, Boarding Pistol, CC Weapon.
- **Option 531:** **21 / 0.5** — Hacker, Hacking Device; Combi Rifle, Light Shotgun, Boarding Pistol, CC Weapon.
- **Option 532:** **19 / 0** — Hacker, Killer Hacking Device; Combi Rifle, Light Shotgun, Boarding Pistol, CC Weapon.

### Garon Aibōt — `garon-aib-t`

**Unit ID:** 1831 — **AVA:** 2 — REM, Support Troops, Regular.  
**Stats:** `15-10 13 11 10 13 0 3 STR1 3`.  
**Rules/equipment:** Courage, Remote Presence, Total Reaction; 360º Visor.

- **Option 1:** **23 / 1** — HMG, PARA CC Weapon (-3).
- **Option 2:** **21 / 0** — Mk12, PARA CC Weapon (-3).
- **Option 3:** **16 / 0** — Thunderbolt, Smoke Grenade Launcher, PARA CC Weapon (-3).

### Ninjas — `ninjas`

**Unit ID:** 135 — **AVA:** 2 — SK, Spec. Trained Troops, Regular.  
**Stats:** `10-10 23 11 12 13 1 0 1 2`.  
**Rules:** Martial Arts L3, CC Attack (Shock), Surprise Attack (-3), Camouflage, Courage, Hidden Deployment, Dodge (+2.5), Infiltration, Mimetism (-6), Stealth, Terrain (Total), Climbing Plus.

- **Option 1:** **24 / 0** — Tactical Bow (+1SD), Shock Mine, Pistol, DA CC Weapon (PS=6).
- **Option 4:** **27 / 0** — Submachine Gun, Pistol, DA CC Weapon (PS=6).
- **Option 5:** **31 / 1.5** — MULTI Sniper Rifle, Pistol, DA CC Weapon (PS=6).
- **Option 6:** **33 / 0.5** — Hacker, Hacking Device; Submachine Gun, Pistol, DA CC Weapon (PS=6).
- **Option 7:** **26 / 0** — Hacker, Killer Hacking Device; Tactical Bow (+1SD), Shock Mine, Pistol, DA CC Weapon (PS=6).
- **Option 9:** **30 / 0.5** — Forward Observer; Boarding Shotgun, Flash Pulse, Pistol, DA CC Weapon (PS=6).

### Domaru Butai — `domaru-butai`

**Unit ID:** 152 — **AVA:** 2 — HI, Line Troops, Regular.  
**Stats:** `15-5 24 12 14 13 3 3 2 2`.  
**Rules:** Martial Arts L3, CC Attack (Shock), BS Attack (SR-1), Courage, Dodge (+5), Frenzy, Stealth, Berserk.

- **Option 1:** **19 / 0** — Chain Rifle, Pistol, Contender, E/M Grenades, AP CC Weapon (PS=4).
- **Option 2:** **20 / 0** — Chain Rifle, Pistol, Contender, E/M Grenades, E/M CC Weapon (PS=4).
- **Option 3:** **23 / 0** — Boarding Shotgun, E/M Grenades, Pistol, E/M CC Weapon (PS=4).
- **Option 5:** **31 / 1.5** — Spitfire, Pistol, E/M CC Weapon (PS=4).
- **Option 6:** **27 / 0** — Forward Observer; Combi Rifle, E/M Grenades, Flash Pulse, Pistol, E/M CC Weapon (PS=4).
- **Option 7 Lieutenant (+1 Order):** **23 / 0** — option-2 weapons.
- **Option 8 Lieutenant (+1 Order):** **35 / 1.5** — Spitfire, Pistol, E/M CC Weapon (PS=4).
- **Fireteams:** JSA Fireteams I and II, max 2 in each row.

### Shikami — `shikami`

**Unit ID:** 773 — **AVA:** 2 — HI, Elite Troops, Regular.  
**Stats:** `15-5 23 13 14 13 3 3 2 2`.  
**Rules:** Martial Arts L3, Courage, Forward Deployment (+10), Dodge (+5), Mimetism (-6), Specialist Operative, Stealth, Climbing Plus, Super-Jump (+7.5).

- **Option 1:** **42 / 0** — Contender, Flash Pulse (+1B), Eclipse Grenades, Assault Pistol, AP + DA CC Weapon (PS=4).
- **Option 2:** **47 / 0** — MULTI Rifle, D-Charges, Eclipse Grenades, Pistol, AP + DA CC Weapon (PS=4).

## Canonical Fireteam definitions

The following two rows are the **Army-1101 vanilla chart**. They are authoritative for Vanilla JSA Fireteam legality; do not substitute Ōban or Shindenbutai sectorial charts.

### FT-01 — JSA Fireteams I

**Types:** Duo  
**Faction limit:** contributes to the faction-wide maximum of 2 Duos.  
**Required member:** none in the source row.

| Member | Unit ID | Required | Min | Max | Profile restriction | Notes |
|---|---:|---|---:|---:|---|---|
| Jizamurai Hanryodan | 1821 | no | 0 | 1 | all | — |
| Domaru Butai | 152 | no | 0 | 2 | all | — |
| Daiyōkai Dengekitai | 1002 | no | 0 | 1 | all | — |
| Shizoku Kōgeki-tai | 1822 | no | 0 | 1 | **FTO profiles 1–2 only** | source display name `SHIZOKU FTO` |
| O-Yoroi Kidobutai | 156 | no | 0 | 1 | all | — |
| Mechazoid Sōkōrentai | 1788 | no | 0 | 1 | all | — |
| Yuriko Oda | 1019 | no | 0 | 1 | **FTO profiles 1–2 only** | source display name `YURIKO ODA FTO` |
| Miyamoto Mushashi | 223 | no | 0 | 1 | all source-available options | no vanilla FTO-only marker in chart |
| Shurayuki | 1829 | no | 0 | 1 | all | — |
| Ioann Bann | 1940 | no | 0 | 1 | all | — |

### FT-02 — JSA Fireteams II

**Types:** Duo, Haris  
**Faction limits:** contributes to the faction-wide maximum of 2 Duos / 1 Haris.  
**Required member:** none in the source row.

| Member | Unit ID | Required | Min | Max | Profile restriction | Notes |
|---|---:|---|---:|---:|---|---|
| Domaru Butai | 152 | no | 0 | 2 | all | — |
| Karakuri Special Project | 154 | no | 0 | 2 | all | — |
| Yáoxiè Rui Shi | 159 | no | 0 | 1 | all | — |
| Daiyōkai Dengekitai | 1002 | no | 0 | 1 | all | — |
| Yuriko Oda | 1019 | no | 0 | 1 | **FTO profiles 1–2 only** | source display name `YURIKO ODA FTO` |
| Takeshi “Neko” Oyama | 164 | no | 0 | 1 | all | — |
| Shurayuki | 1829 | no | 0 | 1 | all | — |

### Fireteam negative lookups

- Vanilla JSA has **no Core** access in the pinned chart.
- `PANGGULING FTO` does not gain vanilla Fireteam access merely from its profile name.
- Yuriko profile 3 is non-FTO and cannot use either vanilla Fireteam row.
- Shizoku profile 3 (Strategic Deployment) is non-FTO and cannot use FT-01.
- Kempeitai are **not** vanilla Wildcards in this chart; their Ōban Wildcard status does not carry into generic JSA.
- Sectorial-specific counts-as or Wildcard rules from Ōban/Shindenbutai do not apply unless explicitly reproduced above.

## Unit → Fireteam access index

This table is derivative. If it conflicts with the canonical rows above, the canonical Fireteam definitions win.

| Unit | Fireteam | Type | Access | Profile restriction | Max |
|---|---|---|---|---|---:|
| Jizamurai Hanryodan | FT-01 JSA Fireteams I | Duo | native | all | 1 |
| Domaru Butai | FT-01 JSA Fireteams I | Duo | native | all | 2 |
| Domaru Butai | FT-02 JSA Fireteams II | Duo/Haris | native | all | 2 |
| Daiyōkai Dengekitai | FT-01 JSA Fireteams I | Duo | native | all | 1 |
| Daiyōkai Dengekitai | FT-02 JSA Fireteams II | Duo/Haris | native | all | 1 |
| Shizoku Kōgeki-tai | FT-01 JSA Fireteams I | Duo | native | **FTO 1–2 only** | 1 |
| O-Yoroi Kidobutai | FT-01 JSA Fireteams I | Duo | native | all | 1 |
| Mechazoid Sōkōrentai | FT-01 JSA Fireteams I | Duo | native | all | 1 |
| Yuriko Oda | FT-01 JSA Fireteams I | Duo | native | **FTO 1–2 only** | 1 |
| Yuriko Oda | FT-02 JSA Fireteams II | Duo/Haris | native | **FTO 1–2 only** | 1 |
| Miyamoto Mushashi | FT-01 JSA Fireteams I | Duo | native | all source-available options | 1 |
| Shurayuki | FT-01 JSA Fireteams I | Duo | native | all | 1 |
| Shurayuki | FT-02 JSA Fireteams II | Duo/Haris | native | all | 1 |
| Ioann Bann | FT-01 JSA Fireteams I | Duo | native | all | 1 |
| Karakuri Special Project | FT-02 JSA Fireteams II | Duo/Haris | native | all | 2 |
| Yáoxiè Rui Shi | FT-02 JSA Fireteams II | Duo/Haris | native | all | 1 |
| Takeshi “Neko” Oyama | FT-02 JSA Fireteams II | Duo/Haris | native | all | 1 |

## Roster identity, dependency, and peripheral notes

### Yuriko identity relation

The source relates unit `1019` (Yuriko Oda) with alternate/source identity `1799`, maximum one. Unit `1799` is not a second standard Army-1101 roster record here; retain the relation when comparing against alternate/Reinforcement JSA data.

### Yojimbo catalogue relation

The aggregate source carries the JSA character relation covering Yojimbo IDs `224`, `1834`, `10224`, and `11834`, maximum one. In the pinned generic Army-1101 data, the ordinary Yojimbo catalogue records are not standard roster records because their generic objects have no `1101` faction availability. They are therefore **not added to the 43-unit standard vanilla roster merely because the relation exists**.

### Peripherals and composite records

- **Yáozăo** are Servant Peripherals and do not generate Orders independently.
- **O-Yoroi** includes a **Kobaruto Ancillary Remote** with its TAG options; the Kobaruto is not a separate roster selection.
- **Mechazoid** likewise carries its Kobaruto Ancillary Remote as a subordinate profile.
- **Ioann Bann** uses Dogface/Dog-Warrior states under one logical roster record.
- Optional Spec-Ops / Team-Ops subordinate records remain within those optional game modes.

## Reinforcements boundary

The standard Vanilla JSA dataset exposes linked Reinforcements Army ID **1199**. It remains deliberately separate from the 43-unit standard Army-1101 roster and the two vanilla Fireteam rows above. Do not mix Main and Reinforcement roster/Fireteam permissions unless the relevant Reinforcement-mode rules explicitly allow it.

## Validation notes

Validated against Army snapshot `7.26246.159` on 2026-10-16:

- Standard roster membership is the set of logical unit objects whose faction availability includes Army `1101`.
- **43** standard logical roster records were identified.
- **2** optional-mode records were separated: Kaizoku Spec-Ops (`1924`) and JSA Team-Ops (`1938`).
- Generic `factions: []` Soldier-of-Fortune / mercenary-catalogue entries were excluded instead of being imported from JSA sectorials.
- Vanilla AVA values were taken from Army-1101 rather than copied from Ōban or Shindenbutai. Material examples: Ryūken 2, Oniwaban 1, Karakuri 2, Atom 2, Daiyōkai 1, Tankō 2, Hatamoto 1, Kempeitai 2, Jizamurai 1, O-Yoroi 1, Aragoto 2, Garon 2, Ninjas 2, Domaru 2.
- The vanilla Fireteam chart has **Core 0, Haris 1, Duo 2** and exactly two standard rows: JSA Fireteams I and JSA Fireteams II.
- Fireteam-specific FTO restrictions were retained for Shizoku and Yuriko.
- Sectorial-only Wildcard/counts-as semantics were not carried into the generic faction.
- Reinforcement Army ID `1199` remains distinct from standard Vanilla JSA.

## Command-unit apex/value cross-reference (2026-10-23)

**Hatamoto LT(+1) 36–39/+1 SWC** can be an efficient *attacking* commander because its extra Orders and SWC rebate pay for real fighting; **Kempeitai CoC 17/0 BSG / 20/0 Combi** is top raw backup value. **Domaru LT(+1) 23/0** offers a lower-cost alternative when a hidden/screened LT or different gun makes more sense. CoC is insurance only if the Kempeitai survives separately from the LT's assault.

See [cross-game Lieutenant, Chain of Command and Order-package tiers](../../notes/list-building/command-units-apex-and-value.md). **Use this roster/Fireteam chart above for exact legality.**

## Mission specialist / button-pusher selections (N5.3)

**Shikami SO42/0 (or gun/tool 47/0)** is an apex carry/turn-3 objective specialist: 15-5, FD+10, Mimetism(-6), 2W, Eclipse, Climbing Plus and Super-Jump. **Ninja KHD26/0, FO30/0** is the hidden infiltrating console-taker; **Aragoto KHD19/0 or HD21/.5** wins lateral reach but is exposed; **Hatamoto SO34 or LT36–39** fights and scores at cost/risk. **Kempeitai CoC17** is cheap mission specialist/succession, provided the selected CoC is not marked Non Specialist.

[Cross-faction apex and points-value guide](../../notes/list-building/mission-specialists-and-button-pushers-apex-value.md). Use **this roster and Fireteam chart** for exact availability.

## N5.3 airborne / backline-strike archetypes and trades (2026-10-23)

**Oniwaban29/0 (non-LT)** or **Shinobu Kitsune44/.5** is apex hidden **Infiltration/Monofilament**: the attacker can begin safely in its own half without a roll and stage toward enemy DZ; enemy-half attempt is **Oniwaban PH18−3 = 75%, Shinobu PH19−3 = 80%**, and **cannot deploy inside enemy DZ**. Failure returns model to own DZ edge and strips initial Marker/Hidden. **Teishin BSG19/0, FO19/0, KHD21/0** is the cheapest reliable *budget investment* AD scorer/striker: actual Combat Jump still needs its PH roll, alternate normal Parachutist only outside enemy DZ. **Oniwaban LT30/1 or Shinobu LT44/.5 left in Hidden Deployment triggers LoL at the check**; use on-table marker instead and **Kempeitai CoC17** as separate backup if chosen.

[Full N5.3 apex/value and delivery-probability tier guide](../../notes/list-building/airborne-and-enemy-dz-attackers-apex-value.md). Current roster/profile restrictions and canonical Fireteam chart above govern legal choices.

## Active-turn gunfighter cross-reference (2026-10-23)

**Active-turn shooting choices:** **Hatamoto** and **Oniwaban/Shinobu** are particularly efficient at **midfield/short-angle and CC** fights, not conventional 32in HMG FtF. **Hatamoto Plasma Carbine34/0** converts efficient close shots into scoring with Specialist Operative; **Red Fury40/1** buys more conventional midrange volume. **Teishin** is a cheap angled/backline threat, not a long ARO clearer. For open heavy lanes a suitable roster-specific **TAG** or separate long gun must carry that task instead of forcing a CC specialist into an unfavorable range band. [Non-TAG vs TAG gunfighter comparisons](../../notes/list-building/active-turn-gunfighters-apex-and-value.md).

## N5.3 cheap warband, template and CC trade decisions

**Aragoto Boarding Shotgun13/0** is a very fast **Regular+Impetuous, Mimetism(-3) bike** close-range trader; **20-15 MOV**, but no Smoke and remains vulnerable to mines/turret ARO. **Miyamoto Musashi Chain Rifle+EXP CCW21/0 Irregular** is a high-apex **CC25/MA5** killer who needs a real approach and is *not a disposable 5pt Chain*. His **25/.5 FTO Regular** is a different profile. **Oniwaban/Shinobu** Hidden assassins are expensive, safe deployment options, not warband swarms. **Kempeitai CoC17** protects an aggressive LT, avoid sacrificing it as a cheap CC attacker.

[Whole-game cheap-trading apex/value, specific targets and Lt/CoC notes](../../notes/list-building/warbands-and-cheap-trading-units-apex-value.md). Current unit loadouts and canonical Fireteam chart remain authoritative.

## TAG tactical cross-reference (2026-10-23)

**O-Yoroi** supplies the large-range armored shooting axis that JSA's close-range attackers otherwise lack; **Mechazoid** is an alternative TAG option with its own TacAware and Fireteam choices. Price the entire mission/support shell and available Kobaruto/ancillary tools. The best TAG is whichever covers the *opposite range band* to the ninjas/warbands already bought, not simply the largest gun.

Across all factions, compare **apex power** separately from **points value**, counterplay and mission fit: [N5.3 TAG guide](../../notes/list-building/tags.md). The current unit profiles and canonical Fireteam chart above take precedence over tactical opinions.

## Hacker and KHD tactical cross-reference (2026-10-23)

**Kyoshō HD20/0.5 vs KHD20/0**, **Teishin Combat Jump HD23/0.5 vs KHD21/0**, and **Keisotsu HD16/0.5** offer cheap regular hacking/specialist options; **Ninja Hidden KHD26/0** and **Nokizaru KHD27/0** pay for midfield camouflage/mission reach. **Kurayami Ninja HD26/0.5** can contribute a forward anti-HI program alongside JSA's melee threats. **Why:** against Hackers, KHD/Cybermask guards objectives; versus multiple HI/TAG without cyber opposition, a cheap HD/Carbonite/Oblivion is worth more than several basic KHDs. JSA's physical killers and perimeter tools should not be replaced by a Guided package unless Pitchers/Repeaters genuinely support it. **Only current JSA Fireteam rows** confer linked cyber bonuses.

See the [cross-game apex/value Hacker/KHD tier guide](../../notes/list-building/hackers-and-killer-hackers.md). **The sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative; device upgrades are profile-specific.**


## Cheerleader / Order-generation tactical cross-reference (2026-10-23)

See the N5.3 [cross-game apex/value rankings and transcript-backed competing assessments](../../notes/list-building/cheerleaders-and-order-generators.md). The current roster and official Fireteam definitions above remain authoritative; unit access/cost may differ from vanilla.

- Keisotsu — inexpensive S2 Regular bodies, line-FT material and possible utility upgrades; optimize the cheapest legal role rather than premium heavy guns.
- Yuriko/Engineer — buy for recovery and mission support, not cheap generic Order generation.
- Karakuri — durable multiple-role attacker/specialist, not a minimal-cost backline cheerleader; compare total Order demand.
- 3pt Warcor — very useful Irregular Flash ARO/cheap screen, NOT an ordinary transferable Order.

**Selection rule:** Count deployed, transferable Regular Orders per Combat Group, not total models or restricted bonus Orders; choose the lowest-cost protected Regular profile that *also* contributes a relevant Repeater, Baggage, Fireteam, template, ARO or Specialist job. Check Group slots and DZ hiding space before buying a third large-base REM or replacing a needed scoring piece.


## ARO apex/value cross-reference (2026-10-23)

[Best ARO units across N5.3 — absolute apex vs points-value](../../notes/list-building/aro-units-apex-and-value.md) compares hidden reactive fire, TR/Neurocinetics, Flash/DTW/expendable defenders and why competing creators disagree. The **roster here** is authoritative for actual costs, Training, AVA and Fireteam construction.

- **Garon TR** — 16pt/0SWC Thunderbolt/smoke option shifts from passive guard to active smoke enablement where legal
- **Raiden HRL/ML** — concealed surprise launcher + mine, high ambush ceiling; the ML can cost 2SWC, so choose the defended scoring lane carefully
- **Ryūken rocket launcher** — low-mid cost marker/ambush control; complement with mines and a second visible layer
- **Karakuri** — durable roadblock/scoring threat for close quarters; not cost-effective as an inert long-lane sniper
- **Warcor 3pt Flash** — disposable Irregular Stun/Orders tax, not a generic Regular cheerleader

**Best circumstance:** long exposed lanes justify a real sniper/missile/linked gun; dense tables, DZ landings and mission rooms favor E/M, mine, Shotgun, Riotstopper and hidden traps. Cover the destination/approach, layer serial threats rather than two pie-sliceable visible guns, and preserve scoring units for the active turn.

## Doctor / Engineer / Recovery cross-reference (2026-10-23)

**Tokusetsu Doctor14 / Engineer14 WIP13 + Yáozăo3** is a cheap recoverability net for VITA attack pieces and **Karakuri/O-Yoroi STR** respectively; Remote Presence repair may warrant token on expensive STR. **Yuriko Oda25** adds Mimetism/mines and a forward route; **Genbutai Engineer23** can remain with a legal team if applicable. Do not confuse one 14pt medical model with the separate 14pt repair profile: jobs are different. [Doctor/Engineer apex and recovery odds](../../notes/list-building/doctors-engineers-and-recovery-apex-value.md).

## N5.3 DZ defense / anti-alpha-strike tactical choices

**Warcor 360º Flash 3/0** is the cheap Irregular rear/edge arrival tax; **Robio Aibōt Flash+Repeater 7/0** gives a Regular Order and small network guard, **not** 360º. **Keisotsu Hacker+CrazyKoala 16/.5** is a Regular Hacker carrying a perimeter threat, **not a Minelayer**: Koala placement normally costs an Order and Boost **does not** trigger against Impersonation/Camo Markers. **Karakuri E/Mitter+Chain Rifle+Panzerfaust+FO 31/0** is a powerful 3STR counterpunch/short-range anchor if it also advances/scores, **not** an efficient disposable sentry. Split 9–10pt Keisotsu cheerleaders behind two independent corners instead of a single templatable cluster.

[Whole-game DZ-defense apex/value and anti-impersonation guide](../../notes/list-building/dz-defenders-alpha-strike-and-impersonation-apex-value.md).

## Close-combat assassins and counter-CC — N5.3 (2026-10-23)

**Oniwaban SMG29/0, Shinobu44/.5 and Saito33/0** are legal Hidden/Infiltration high-CC assassination alternatives; **Mono vs EXP** decides whether heavy target's vulnerability or multiple target options matter. **Shikami42/0** is the more reliable repeated assault/scoring model with Eclipse and high mobility, not the one-roll Mono specialist. **Hatamoto Plasma34/0** is 2W/MA4/NBW defensive duelist and specialist, vulnerable to being trapped by hacking/screening if forced into unsupported charge. This roster **does not automatically include the Ōban-specific 21pt Musashi** simply because other JSA factions have him. [Cross-game CC assassin apex/value, Guard and delivery disputes](../../notes/list-building/dedicated-close-combat-assassins-apex-value.md).

## N5.3 network projection — Pitchers, Repeaters, TinBots and disposable delivery

**Robio Aibōt7/0** is the ordinary **Regular native Repeater/Flash** source; **Pangguling8/0 Baggage+Repeater** is a second cheap regular Order with logistics/reload. **Keisotsu Hacker+CrazyKoala16/.5** does NOT bring a native Repeater or Minelayer by itself; Koala is a different Boost threat and needs placement. **Karakuri/other KHD/HD profiles** can only use projected net if the rules and target permit, and Vanilla JSA **does not inherit Shindenbutai's Tanuki Pitcher20/.5**. **Counter:** JSA can win through Hidden CC/fast assault rather than expensive extra Repeater/Guided packages; use 7–8pt support if it also protects flank.

[Whole-game apex/value network guide, current profiles, and opposing media views](../../notes/list-building/network-projection-repeaters-pitchers-apex-value.md).

## N5.3 rare abilities & unusual combinations — tactical synthesis

**Shikami42/0** merges **Eclipse+Mimetism(-6)+Climbing++Super-Jump(+7.5)+2W+FD+Specialist**, rare true turn-3 specialist/assassin able to cross MSV-covered rooftop lanes. **47/0** buys MULTI Rifle/D-Charges; both maintain Eclipse. **Oniwaban29/0 / Shinobu44/.5** are stronger monofilament delivery into the right target but do **not** have Shikami's independent Eclipse/2W specialist extraction package. **Opposing JSA 2026 event perspective:** spending 42 on Shikami is justified by hard objectives, not merely cheaper fight; a 20–30pt infiltrating Ninja+Smoke partner can be better on simple maps.

[Whole-game rare capability apex/value, rules, matchups and opposing MCP transcripts](../../notes/list-building/rare-capabilities-and-unique-combinations-apex-value.md). Use current profile and Fireteam chart above.

## Anti-TAG / Anti-HI without hacking — N5.3 (2026-10-23)

**Oniwaban SMG29/0, Shinobu44/.5** are apex anti-TAG **Hidden/Infiltration/Monofilament** *only if contact route survives screening*; **Hatamoto Plasma34/0 (Mono/E/M CCW)** is tougher 2W counter-CC but lacks Hidden. **Lù Duān20 E/M Carbine+E/M Mine**, legal **Tankō Blitzen/Monofilament** or **Karakuri Panzerfaust** offer non-hacking ranged/control alternatives. Don't rely exclusively on CC: TAG Guard/mines/cheap watchers may make E/M at 8–16in the better choice. [Cross-game non-hacking anti-armor apex/value guide](../../notes/list-building/anti-tag-anti-heavy-infantry-non-hacking-apex-value.md).

## N5.3 objective holding, zone domination & carried-objective choices

**Karakuri FO31/0** is the top practical **box holder**: STR3/ARM3/BTS6/Immunity(Enhanced)/Remote Presence, FO, Chain Rifle+Panzerfaust and 0 SWC; **35/0 MULTI** and **38/0 Mk12** pay for specific shooting, not better carrying. **Shikami42/0** is best at *delivering* the box (Eclipse, Mimetism-6, Climbing+, Super-Jump, 2W); loses Marker protection only where it has marker skills, not relevant here. **Hatamoto34/0** NCO+Nanoscreen is a strong Specialist 2W zone cleaner; **Daiyōkai46/0** NWI/ARM5 adds points but is **not an ordinary box Specialist**. **Opposing WIP12 JSA/Meta winner 2026:** defend Karakuri with an Engineer/nearby screens and use late objective-positioning rather than reckless multi-round fights; 31pt durable FO often beats 42pt Shikami when travel is easy.

[Cross-game zone-holder and carrier apex/value guide, rules, and transcript disagreements](../../notes/list-building/objective-holding-zone-domination-and-carriers-apex-value.md). Source roster/FT chart above wins over tactical comparisons.

## Anti-Tech — enemy visors, Mimetism, markers and Impersonation (2026-10-23)

**Atom Aibōt FO/Sensor15/0** is the budget regular **Camo/Hidden ZoC detector**, with Triangulated Fire for a revealed Mimetism target; a cheap REM search is usually more efficient than revealing a premier ninja to scout. **Kempeitai MSV2** or **Rui Shi MSV2** are separate *shoot-to-kill* tools that can also exploit rostered Yojimbo/Garon Smoke against opponents without MSV. **Eclipse/Disco** on a legal JSA body bypasses *enemy* MSV/Marksmanship better than a direct fight. Opponent sensor pressure and anti-IMP screening must be planned for your own marker assassins too.

[Anti-tech N5.3 whole-game apex/value and counter-matchups](../../notes/list-building/anti-tech-msv-mimetism-camo-impersonation-apex-value.md).
