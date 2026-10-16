---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 905
sectorial_slug: starco-free-company-of-the-star
sectorial_name: StarCo. Free Company of the Star
parent_faction: Non-Aligned Armies
rules_baseline: N5.3
army_source_version: "7.26246.159"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-16
coverage: "Complete standard StarCo roster, standard loadouts/profile states and peripherals, canonical Fireteam chart, exact FTO/counts-as restrictions, reverse Fireteam access, optional-mode hooks, and Reinforcements boundary. Generic Soldier of Fortune catalog entries are excluded."
---

# StarCo. Free Company of the Star — N5.3 sectorial reference

## Overview and provenance

This file is the repository reference for **StarCo. Free Company of the Star** (Army sectorial ID `905`), a sectorial of the **Non-Aligned Armies / NA2** (parent Army ID `901`). It is intended to be sufficient for ordinary roster, AVA, points/SWC, profile, dependency, and Fireteam-legality questions without reopening Army.

Primary data source:

- Corvus Belli Army data snapshot mirrored by `massayoshi/infinity-army-backup`.
- Pinned source commit: `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b` (`army: N5.3 + ITS18`).
- Army dataset: `n5/starco-free-company-of-the-star/7.26246.159.json`.
- Source blob: `2cde2a4e10ed912bb32d3e6e441ace255fac4d8b`.
- Army version: **7.26246.159**.
- Sectorial ID: **905**.
- Parent Non-Aligned Armies ID: **901**.
- Reinforcements list ID exposed by the dataset: **999**.
- Cross-check/reference model commit: InfinityDB `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: **N5.3 + N5 FAQ v0.1**.

Coverage policy:

- The **33 standard logical roster records** whose faction availability includes StarCo are included below.
- Generic Soldier-of-Fortune catalog records present in the aggregate payload with `factions: []` are excluded.
- **Rumbler Spec-Ops** and **NA2 Team-Ops** are optional-mode hooks, not ordinary matched-play roster entries.
- Reinforcements (`army_id: 999`) remain distinct from the normal StarCo roster and Fireteam chart.
- Composite states and Peripherals stay under their parent logical unit rather than being counted as separate roster entries.
- Fireteam legality comes from the canonical chart below, not from an `FTO` label alone.
- Where Army marks multiple entries `required: true`, this file follows repository convention and treats those entries as a **required source-choice set** unless the chart specifies otherwise.
- Parenthetical labels from the Fireteam chart are preserved as `Counts as` / equivalence labels. They are not broadened beyond their source wording.

## Sectorial summary

| Field | Value |
|---|---|
| Sectorial | StarCo. Free Company of the Star |
| Parent faction | Non-Aligned Armies / NA2 |
| Army ID | 905 |
| Rules baseline | N5.3 + N5 FAQ v0.1 |
| Army source | 7.26246.159 |
| Standard logical roster records | 33 |
| Optional-mode records | 2 |
| Reinforcement roster | yes — Army ID 999 |
| Fireteam chart | yes |

## Fireteam limits and interpretation

| Constraint | Value / wording |
|---|---|
| Core | up to 1 Core |
| Haris | up to 1 Haris |
| Duo | effectively unlimited (`256` in Army source) |
| Fireteam families | StarCo; Riot Grrls; PMC; Armored; Outrage |
| Wildcards | Diggers; Raoul Spector FTO; Emily Handelman; Uhahu; Knauf FTO |
| Main/Reinforcement mixing | Keep normal StarCo and Reinforcement charts distinct |

Important profile-level restrictions and equivalences:

- **Fiddler access in Riot Grrls Fireteams is FTO-only:** option `1` only. It counts as **Riot Grrl** there. Options `2` and `3` are not Fireteam legal.
- **Tsyklon access in Armored Fireteams is FTO-only:** options `1` and `2`. Options `4` and `5` are not Fireteam legal.
- **Raoul Spector Wildcard access is FTO-only:** option `3` only. It carries the source equivalence label **PMC**. Option `1` is not Fireteam legal.
- **Knauf access is FTO-only:** option `2` only, both in Outrage and through its Wildcard row. It carries the source equivalence label **Outrage**. Option `1` is not Fireteam legal.
- **Daktari** counts as **Alguacil** in StarCo Fireteams.
- **Avicenna** counts as **Riot Grrl** in Riot Grrls Fireteams.
- **Brawlers** and **CSU** carry **PMC** equivalence in PMC Fireteams.
- **Emily Handelman** carries source equivalence labels **Brawlers, PMC, Outrage** through the Wildcard row, and **Outrage** in the native Outrage row.
- **Uhahu** carries **Outrage** equivalence through both the Outrage and Wildcard rows.
- **Diggers** carry the source labels **Brawlers, PMC** through the Wildcard row.
- The StarCo family marks both **Alguaciles** and **Mobile Brigada** `required: true`; under repository required-choice semantics at least one source member must come from that set.
- The PMC family marks both **Brawlers** and **CSU** `required: true`; treat them as a required source-choice set.
- The Armored family marks both **Anaconda** and **Triphammer** `required: true`; treat them as a required source-choice set.
- The Outrage family marks both **Emily** and **Uhahu** `required: true`; treat them as a required source-choice set.

## Standard roster index

| Unit ID | Unit | AVA | Type | Classification | Regularity | Fireteam access / notes |
|---:|---|---:|---|---|---|---|
| 248 | Highlander Caterans | 1 | LI | Spec. Trained Troops | Irregular | — |
| 50 | Warcors | 1 | LI | Mercenary Troops | Irregular | — |
| 400 | Corregidor Bandits | 2 | SK | Spec. Trained Troops | Irregular | — |
| 122 | CSU, Corporate Security Unit | 3 | LI | Mercenary Troops | Regular | PMC |
| 382 | Mobile Brigada | 5 | HI | Veteran Troops | Regular | StarCo; Armored |
| 491 | Avicenna | 1 | LI | Character | Regular | Riot Grrls; counts as Riot Grrl |
| 300 | Anaconda | 2 | TAG | Mercenary Troops | Regular | Armored; embedded Operator state |
| 405 | Daktaris | 1 | LI | Support Troops | Regular | StarCo; counts as Alguacil |
| 265 | Wardrivers | 1 | LI | Mercenary Troops | Regular | — |
| 331 | Al Hawwa' Unit | 1 | SK | Spec. Trained Troops | Regular | — |
| 412 | Transductor Zonds | 1 | REM | Support Troops | Regular | — |
| 1071 | Uhahu | 1 | LI | Character | Regular | Outrage; Wildcard; counts as Outrage |
| 1569 | Triphammer | 1 | TAG | Mercenary Troops | Regular | Armored; includes Turtlemek Ancillary Remote |
| 431 | Riot Grrls | 5 | HI | Spec. Trained Troops | Regular | Riot Grrls |
| 1568 | Diggers | 2 | HI | Mercenary Troops | Regular, Impetuous | Wildcard; source labels Brawlers, PMC |
| 1072 | Emily Handelman | 1 | LI | Character | Regular | Outrage; Wildcard; source labels Brawlers, PMC, Outrage |
| 409 | Reaktion Zonds | 1 | REM | Support Troops | Regular | — |
| 462 | Señor Massacre | 1 | MI | Character | Regular | StarCo |
| 236 | Hardcases | 1 | SK | Spec. Trained Troops | Irregular | — |
| 1069 | Raoul Spector | 1 | LI | Character | Irregular or Regular by option | Wildcard, **FTO option 3 only**; source label PMC |
| 394 | Hellcats | 2 | MI | Elite Troops | Regular | — |
| 1564 | Fiddler | 1 | LI | Character | Regular | Riot Grrls, **FTO option 1 only**; counts as Riot Grrl |
| 423 | Tsyklon Sputnik | 1 | REM | Support Troops | Regular | Armored, **FTO options 1/2 only** |
| 404 | Corregidor Jaguars | 4 | WB | Line Troops | Regular | — |
| 240 | Irmandinhos | 1 | WB | Line Troops | Irregular, Impetuous | Armored |
| 406 | Clockmakers | 1 | LI | Support Troops | Regular | — |
| 410 | Vertigo Zonds | 1 | REM | Support Troops | Regular | — |
| 425 | Zondbots | 2 | REM | Support Troops | Peripheral | Servant |
| 426 | Salyut Zonds | 1 | REM | Support Troops | Regular | — |
| 939 | Knauf | 1 | LI | Character | Regular | Outrage/Wildcard, **FTO option 2 only**; counts as Outrage |
| 987 | Brawlers, Mercenary Enforcers | 5 | MI | Spec. Trained Troops | Regular | StarCo; PMC; Armored |
| 408 | Stempler Zonds | 1 | REM | Support Troops | Regular | No StarCo Fireteam access despite option 3 FTO label |
| 296 | Corregidor Alguaciles | 255 | LI | Line Troops | Regular | StarCo |

### Optional-mode entries

| Unit ID | Unit | Mode | Fireteam hook |
|---:|---|---|---|
| 1925 | Rumbler Spec-Ops | Infinity Spec-Ops | Up to 1 in StarCo, PMC, or Armored Fireteams |
| 1939 | NA2 Team-Ops | Infinity Team-Ops | Optional-mode only; no normal-roster Fireteam row |

## Unit details

Notation: stats are `MOV CC BS PH WIP ARM BTS VITA/STR S`. Source option IDs are retained because otherwise-similar loadouts and FTO legality can depend on them.

### Highlander Caterans — `highlander-caterans`

**Unit ID:** 248 — AVA 1 — LI, Spec. Trained Troops; Irregular.

- **Stats:** `10-10 22 12 13 12 0 0 1 2`.
- **Rules:** Surprise Attack (-3), Camouflage (1 Use), Mimetism (-3), Stealth, Climbing Plus.
- **Option 1:** **21 / 1** — T2 Sniper Rifle, Pistol, AP CC Weapon (PS=7).
- **Option 2:** **21 / 0.5** — AP Sniper Rifle, Pistol, AP CC Weapon (PS=7).
- **Option 3:** **23 / 1** — T2 Sniper Rifle, Pistol, AP CC Weapon (PS=7); Forward Deployment (+10).

### Warcors — `warcors-war-correspondents`

**Unit ID:** 50 — AVA 1 — LI, Mercenary Troops; Irregular.

- **Stats:** `10-10 11 9 11 13 0 0 1 2`.
- **Rules:** Journalist.
- **Option 1:** **3 / 0** — 360º Visor; Flash Pulse, Stun Pistol, PARA CC Weapon (-3).
- **Option 2:** **3 / 0** — Sixth Sense; Flash Pulse, Stun Pistol, PARA CC Weapon (-3).

### Corregidor Bandits — `corregidor-bandits`

**Unit ID:** 400 — AVA 2 — SK, Spec. Trained Troops; Irregular.

- **Stats:** `10-10 22 12 13 12 1 3 1 2`.
- **Rules/equipment:** Bangbomb (+4), Martial Arts L2, Surprise Attack (-3), Camouflage, Courage, Mimetism (-3), Stealth, Terrain (Total), BS Attack (+1SD), Infiltration (ReRoll).
- **Option 3:** **23 / 0** — Light Shotgun, Adhesive Launcher Rifle, Boarding Pistol, DA CC Weapon (PS=6).
- **Option 5:** **28 / 0.5** — Hacker, Hacking Device; Light Shotgun, Adhesive Launcher Rifle, D-Charges, Boarding Pistol, DA CC Weapon (PS=6).
- **Option 6:** **26 / 0** — Hacker, Killer Hacking Device; same option-5 weapons.
- **Option 7:** **25 / 0.5** — Minelayer, Deployable Repeater; Submachine Gun, Shock Mine, Boarding Pistol, DA CC Weapon (PS=6).
- **Option 8:** **24 / 0** — Forward Observer; Light Shotgun, Adhesive Launcher Rifle, Flash Pulse, Boarding Pistol, DA CC Weapon (PS=6).

### CSU, Corporate Security Unit — `csu-corporate-security-unit`

**Unit ID:** 122 — AVA 3 — LI, Mercenary Troops.

- **Stats:** `10-10 16 12 10 12 0 3 1 2`.
- **Rules:** MetaChemistry, Sixth Sense.
- **Option 1:** **10 / 0** — Breaker Rifle, Nanopulser (+1B), MULTI Pistol, PARA CC Weapon (-6).
- **Option 2:** **11 / 0** — Combi Rifle, Nanopulser (+1B), MULTI Pistol, PARA CC Weapon (-6).
- **Option 3:** **11 / 0** — Boarding Shotgun, Adhesive Launcher Rifle (+1B), MULTI Pistol, PARA CC Weapon (-6).
- **Option 4:** **11 / 0** — Specialist Operative; Rifle, Light Shotgun, MULTI Pistol, PARA CC Weapon (-6).
- **Option 5:** **13 / 0** — Specialist Operative; Breaker Combi Rifle, Nanopulser (+1B), MULTI Pistol, PARA CC Weapon (-6).
- **Fireteam:** PMC; source equivalence `PMC`.

### Mobile Brigada — `mobile-brigada`

**Unit ID:** 382 — AVA 5 — HI, Veteran Troops.

- **Stats:** `15-5 18 13 13 13 5 3 2 2`.
- **Rules/equipment:** 360º Visor, Courage, Jump (+7.5).
- **Option 1:** **33 / 0** — TinBot: Firewall (-6); MULTI Rifle, Boarding Pistol (+1B), CC Weapon.
- **Option 2:** **38 / 1.5** — HMG, Boarding Pistol (+1B), CC Weapon.
- **Option 3:** **27 / 0** — Boarding Shotgun, Boarding Pistol (+1B), CC Weapon.
- **Option 5:** **35 / 1.5** — Missile Launcher, Boarding Pistol (+1B), CC Weapon.
- **Option 9:** **36 / 0.5** — Hacker, Hacking Device, TinBot: Firewall (-6); Combi Rifle, D-Charges, Boarding Pistol (+1B), CC Weapon.
- **Option 10 Lieutenant:** **33 / 0** — option-1 loadout; Lieutenant.
- **Option 11 Lieutenant:** **27 / 0** — option-3 loadout; Lieutenant.
- **Fireteams:** StarCo; Armored.

### Avicenna — `avicenna-mercenary-doctor`

**Unit ID:** 491 — AVA 1 — LI, Character.

- **Stats:** `15-5 16 11 11 15 2 3 1 2`.
- **Rules/equipment:** MediKit, Courage, Immunity (ARM), Doctor (+3), No Wound Incapacitation.
- **Option 1:** **28 / 0** — Combi Rifle, Flash Pulse, Nanopulser, Pistol, CC Weapon.
- **Fireteam:** Riot Grrls; counts as Riot Grrl.

### Anaconda — `anaconda-merc-tag-squad`

**Unit ID:** 300 — AVA 2 — TAG, Mercenary Troops.

- **TAG stats:** `15-5 21 13 16 13 7 6 STR3 7`.
- **Rules/equipment:** ECM: Guided (-6), BS Attack (SR-1), Courage, Dodge (PH=11), GizmoKit (PH=11), Tactical Awareness, Transmutation (Escape System -2), Warhorse, Immunity (AP).
- **Option 1:** **59 / 1.5** — AP Spitfire, Heavy Flamethrower (+1B), Thunderbolt (AP), DA CC Weapon (PS=4).
- **Option 2:** **59 / 1.5** — HMG, Light Shotgun (+2B), Panzerfaust, DA CC Weapon (PS=4).
- **Operator state:** `10-10 13 12 10 13 1 3 3 2`; Courage, Specialist Operative, Tactical Awareness, Warhorse, Mimetism (-3); Spitfire, Smoke Grenade Launcher, Boarding Pistol, CC Weapon.
- **Fireteam:** Armored.

### Daktaris — `daktaris`

**Unit ID:** 405 — AVA 1 — LI, Support Troops.

- **Stats:** `10-10 14 11 10 13 1 0 1 2`.
- **Rules/equipment:** Doctor, MediKit.
- **Option 1:** **14 / 0** — Combi Rifle, Pistol, CC Weapon.
- **Fireteam:** StarCo; counts as Alguacil.

### Wardrivers — `wardrivers-merc-hackers`

**Unit ID:** 265 — AVA 1 — LI, Mercenary Troops.

- **Stats:** `10-10 13 11 10 13 0 3 1 2`.
- **Rules:** Sixth Sense.
- **Option 4:** **14 / 0** — Hacker (Zero Pain), Commlink; Boarding Shotgun, Flash Pulse, Pistol, CC Weapon.

### Al Hawwa' Unit — `al-hawwa-unit`

**Unit ID:** 331 — AVA 1 — SK, Spec. Trained Troops.

- **Stats:** `10-10 14 11 11 14 1 0 1 2`.
- **Rules:** Surprise Attack (-3), Camouflage, Infiltration, Mimetism (-3), Stealth, Terrain (Total).
- **Option 1:** **24 / 0.5** — Hacker, Hacking Device; Boarding Shotgun, D-Charges, Cybermine, Silenced Pistol, CC Weapon.
- **Option 2:** **22 / 0.5** — Minelayer; Shock Marksman Rifle, Shock Mine, Silenced Pistol, CC Weapon.
- **Option 3:** **19 / 0** — Forward Observer; Boarding Shotgun, Flash Pulse, D-Charges, Silenced Pistol, CC Weapon.
- **Option 4:** **22 / 0** — Hacker, Killer Hacking Device; Boarding Shotgun, D-Charges, Cybermine, Silenced Pistol, CC Weapon.
- **Option 5:** **21 / 0.5** — Minelayer; Submachine Gun, Grenade Launcher, Shock Mine, Silenced Pistol, CC Weapon.

### Transductor Zonds — `transductor-zonds`

**Unit ID:** 412 — AVA 1 — REM, Support Troops.

- **Stats:** `15-15 13 8 11 13 0 3 STR1 3`.
- **Rules/equipment:** Repeater, Remote Presence, Courage, Mimetism (-3).
- **Option 1:** **7 / 0** — Flash Pulse, PARA CC Weapon (-3).

### Uhahu — `uhahu-hacker-for-hire`

**Unit ID:** 1071 — AVA 1 — LI, Character.

- **Stats:** `10-10 12 11 10 14 1 3 1 2`.
- **Rules/equipment:** Hacker, Hacking Device Plus with Total Control (SR-2), Courage, No Wound Incapacitation, Immunity (Shock).
- **Option 1:** **19 / 0.5** — Pitcher, D-Charges, Assault Pistol, CC Weapon.
- **Fireteam:** Outrage; Wildcard; source equivalence `Outrage`.

### Triphammer — `triphammers-repurposed-industrial-tags`

**Unit ID:** 1569 — AVA 1 — TAG, Mercenary Troops.

- **Full-power stats:** `15-10 17 13 16 12 7 3 STR3 7`.
- **Battle-ravaged stats:** `10-10 15 12 14 12 4 0 STR3 7`.
- **Rules:** CC Attack (Antimaterial), BS Attack (SR-1), Booty, Dodge (PH=9), GizmoKit, Tactical Awareness, Transmutation, CC Attack (+2B).
- **Option 2:** **53 / 1.5** — AP Spitfire, Heavy Flamethrower, AP CC Weapon (PS=4); includes Turtlemek.
- **Option 3:** **52 / 1.5** — AP Spitfire, Chain-colt (+1B), AP CC Weapon (PS=4); includes Turtlemek.
- **Option 4:** **52 / 0** — Heavy Shotgun, Thunderbolt (+1B), AP CC Weapon (PS=4); includes Turtlemek.
- **Option 5:** **48 / 0** — Heavy Shotgun, Heavy Rocket Launcher, Panzerfaust (+1B), AP CC Weapon (PS=4); includes Turtlemek.
- **Turtlemek state:** `15-10 -  - 10 12 0 3 STR1 1`; Courage, Dodge (+3), Mimetism (-3), Specialist Operative, Peripheral (Ancillary).
- **Fireteam:** Armored.

### Riot Grrls — `riot-grrls`

**Unit ID:** 431 — AVA 5 — HI, Spec. Trained Troops.

- **Stats:** `15-5 17 13 13 13 3 3 2 2`.
- **Rules/equipment:** Multispectral Visor L1, Frenzy, Dodge (+3), BS Attack (SR-1), Combat Instinct.
- **Option 3:** **24 / 0** — TinBot: Firewall (-6); Boarding Shotgun, Boarding Pistol, CC Weapon.
- **Option 4:** **29 / 0** — MULTI Rifle, Disco Baller, Boarding Pistol, CC Weapon.
- **Option 5:** **30 / 1.5** — Missile Launcher, Boarding Pistol, CC Weapon.
- **Option 6:** **31 / 1.5** — Spitfire, Boarding Pistol, CC Weapon.
- **Option 7:** **29 / 0** — Specialist Operative; Combi Rifle, E/Mitter, Boarding Pistol, CC Weapon.
- **Fireteam:** Riot Grrls.

### Diggers — `diggers-armed-prospectors`

**Unit ID:** 1568 — AVA 2 — HI, Mercenary Troops; Impetuous.

- **Full-power stats:** `10-10 21 11 13 12 3 0 2 2`.
- **Battle-ravaged stats:** `10-10 21 10 12 12 2 0 2 2`.
- **Rules:** CC Attack (+1B), Booty, Courage, Dodge (+2.5), Natural Born Warrior, Impetuous, Transmutation, No Cover.
- **Option 1:** **18 / 0** — Rifle, Light Shotgun, Grenades, Pistol, AP CC Weapon (PS=6).
- **Option 2:** **14 / 0** — Chain Rifle (+1B), Grenades, Pistol, AP CC Weapon (PS=6).
- **Fireteam:** Wildcard; source equivalence labels `Brawlers, PMC`.

### Emily Handelman — `emily-handelman-intel-agent`

**Unit ID:** 1072 — AVA 1 — LI, Character.

- **Stats:** `10-10 17 13 10 14 1 3 1 2`.
- **Rules/equipment:** X-Visor, Courage, Mimetism (-3), Number 2, Forward Observer, Dogged.
- **Option 1:** **22 / 0** — Breaker Combi Rifle, Nanopulser, Flash Pulse, Assault Pistol, CC Weapon.
- **Option 3:** **24 / 0** — Combi Rifle, Grenade Launcher, E/M Grenade Launcher, Nanopulser, Flash Pulse (+1B), Assault Pistol, CC Weapon.
- **Fireteam:** Outrage native row; Wildcard; source equivalence labels `Brawlers, PMC, Outrage`.

### Reaktion Zonds — `reaktion-zonds`

**Unit ID:** 409 — AVA 1 — REM, Support Troops.

- **Stats:** `15-10 13 11 10 13 0 3 STR1 3`.
- **Rules/equipment:** 360º Visor, Remote Presence, Courage, Total Reaction, Climbing Plus.
- **Option 1:** **24 / 1** — HMG, PARA CC Weapon (-3).
- **Option 2:** **19 / 0** — Thunderbolt (+1B), PARA CC Weapon (-3).

### Señor Massacre — `senor-massacre`

**Unit ID:** 462 — AVA 1 — MI, Character.

- **Stats:** `10-10 24 12 13 13 2 3 1 2`.
- **Rules:** Martial Arts L3, Courage, Dodge (+5), Natural Born Warrior, Immunity (Shock), Regeneration, Stealth.
- **Option 1:** **27 / 0** — Breaker Combi Rifle, Eclipse Grenades, E/M Grenades, Boarding Pistol, Shock CC Weapon (PS=5), E/M CC Weapon (PS=5).
- **Option 2:** **25 / 0** — Boarding Shotgun (+1B), E/M Grenades, Eclipse Grenades, Boarding Pistol, Shock CC Weapon (PS=5), E/M CC Weapon (PS=5).
- **Fireteam:** StarCo.

### Hardcases — `hardcases`

**Unit ID:** 236 — AVA 1 — SK, Spec. Trained Troops; Irregular.

- **Stats:** `10-10 15 11 13 12 0 0 1 2`.
- **Rules:** Surprise Attack (-3), Camouflage, Infiltration, Mimetism (-3), Terrain (Total), Decoy (1), Stealth.
- **Option 1:** **12 / 0** — Tactical Bow (+1SD), Light Shotgun, Boarding Pistol, CC Weapon.
- **Option 2:** **14 / 0** — Tactical Bow (+1SD), Rifle, Boarding Pistol, CC Weapon.

### Raoul Spector — `raoul-spector-mercenary-operative`

**Unit ID:** 1069 — AVA 1 — LI, Character.

- **Stats:** `15-5 22 12 13 13 2 3 2 2`.
- **Rules/equipment:** Bangbomb (+4), Martial Arts L3, Courage, Mimetism (-6), Specialist Operative, Stealth, Super-Jump (Jet Propulsion), Natural Born Warrior, Dodge (+5).
- **Option 1:** **33 / 0** — Irregular; Parachutist, Combat Jump; Boarding Shotgun (+1B), Drop Bears (+1SD), Boarding Pistol, E/M CC Weapon (PS=6).
- **Option 3 FTO:** **34 / 0** — Regular; MULTI Rifle, Drop Bears (+1SD), Boarding Pistol, E/M CC Weapon (PS=6).
- **Fireteam:** Wildcard, **option 3 only**; source equivalence `PMC`.

### Hellcats — `hellcats`

**Unit ID:** 394 — AVA 2 — MI, Elite Troops.

- **Stats:** `10-10 14 12 12 13 2 3 1 2`.
- **Rules:** Courage, Parachutist, Combat Jump (+3), Terrain (Zero-G), Super-Jump (Jet Propulsion).
- **Option 3:** **19 / 0** — Boarding Shotgun, Adhesive Launcher Rifle, D-Charges, Pistol, CC Weapon.
- **Option 5:** **26 / 1.5** — Spitfire, Pistol, CC Weapon.
- **Option 6:** **22 / 0.5** — Hacker, Hacking Device; Boarding Shotgun, D-Charges, Pistol, CC Weapon.
- **Option 8:** **23 / 0** — Paramedic, MediKit, Deployable Repeater; Combi Rifle, Pistol, CC Weapon.

### Fiddler — `fiddler-aristeia-s-ex-toymaker`

**Unit ID:** 1564 — AVA 1 — LI, Character.

- **Stats:** `15-10 18 12 12 14 1 3 STR1 2`.
- **Rules/equipment:** GizmoKit, CC Attack (+1B), Dodge bonuses, Engineer, Immunity (Critical), No Wound Incapacitation.
- **Option 1 FTO:** **29 / 0** — Super-Jump; Contender (+1B), Drop Bears, D-Charges, Breaker Pistol, PARA CC Weapon (-3).
- **Option 2:** **36 / 0** — Climbing Plus; same weapons; includes 1 Jackbot.
- **Option 3:** **43 / 0** — Climbing Plus; same weapons; includes 2 Jackbots.
- **Jackbot state:** `15-10 16 11 10 12 0 3 STR1 1`; Peripheral (Synchronized), Courage, Explode, Climbing Plus; Vulkan Shotgun.
- **Fireteam:** Riot Grrls, **option 1 only**; counts as Riot Grrl.

### Tsyklon Sputnik — `tsyklon-sputniks`

**Unit ID:** 423 — AVA 1 — REM, Support Troops.

- **Stats:** `15-10 14 12 10 13 3 6 STR1 4`.
- **Rules/equipment:** Repeater, 360º Visor, X-Visor, Remote Presence, Courage, Climbing Plus.
- **Option 1 FTO:** **26 / 1** — Spitfire, Chain Rifle, Pitcher, PARA CC Weapon (-6).
- **Option 2 FTO:** **29 / 1** — Feuerbach, Chain Rifle, Pitcher, PARA CC Weapon (-6).
- **Option 4:** **31 / 1** — Feuerbach, Chain Rifle, Pitcher, PARA CC Weapon (-6); Forward Deployment (+10).
- **Option 5:** **31 / 1** — Spitfire, Chain Rifle, Pitcher, Crazykoala, PARA CC Weapon (-6); Forward Deployment (+10), Minelayer.
- **Fireteam:** Armored, **options 1/2 only**.

### Corregidor Jaguars — `corregidor-jaguars`

**Unit ID:** 404 — AVA 4 — WB, Line Troops.

- **Stats:** `10-10 22 11 13 12 1 0 1 2`.
- **Rules:** Frenzy, Martial Arts L1, Courage, Dogged.
- **Option 1:** **10 / 0** — Chain Rifle, Smoke Grenades, Kobra Pistol, DA CC Weapon (PS=7).
- **Option 2:** **11 / 0** — Light Shotgun, Smoke Grenades, Kobra Pistol, E/M CC Weapon (PS=7).
- **Option 3:** **11 / 0** — Adhesive Launcher Rifle, Panzerfaust, Smoke Grenades, Kobra Pistol, DA CC Weapon (PS=7).

### Irmandinhos — `irmandinhos`

**Unit ID:** 240 — AVA 1 — WB, Line Troops; Irregular, Impetuous.

- **Stats:** `10-10 21 10 14 13 1 0 1 2`.
- **Rules/equipment:** Deactivator, Booty, Engineer, Impetuous, No Cover.
- **Option 2:** **8 / 0** — Chain Rifle, D-Charges, Smoke Grenades, Pistol, AP CC Weapon (PS=6).
- **Option 3:** **14 / 0** — Boarding Shotgun, D-Charges, Smoke Grenades, Pistol, AP CC Weapon (PS=6).
- **Fireteam:** Armored.

### Clockmakers — `clockmakers`

**Unit ID:** 406 — AVA 1 — LI, Support Troops.

- **Stats:** `10-10 14 11 10 15 1 3 1 2`.
- **Rules/equipment:** Deactivator, GizmoKit (+1B), Engineer.
- **Option 1:** **18 / 0** — Combi Rifle, D-Charges, Pistol, CC Weapon.
- **Option 2:** **19 / 0** — Deployable Cover; option-1 weapons.
- **Option 3:** **21 / 0** — Combi Rifle, D-Charges, Armed Turret (Combi Rifle), Pistol, CC Weapon.

### Vertigo Zonds — `vertigo-zonds`

**Unit ID:** 410 — AVA 1 — REM, Support Troops.

- **Stats:** `15-10 13 12 10 13 0 3 STR1 3`.
- **Rules:** Remote Presence, BS Attack (Guided), Courage.
- **Option 1:** **16 / 1.5** — Missile Launcher, PARA CC Weapon (-3).

### Zondbots — `zondbots`

**Unit ID:** 425 — AVA 2 — REM, Support Troops; Peripheral (Servant).

- **Stats:** `15-10 11 8 10 13 0 3 STR1 1`.
- **Rules:** Peripheral (Servant), Courage, Mimetism (-3).
- **Option 1:** **3 / 0** — PARA CC Weapon (-3); no Order of its own.

### Salyut Zonds — `salyut-zonds`

**Unit ID:** 426 — AVA 1 — REM, Support Troops.

- **Stats:** `10-10 13 11 10 13 2 3 STR1 4`.
- **Rules/equipment:** Baggage, Remote Presence, Courage.
- **Option 1:** **8 / 0** — Deactivator, Repeater; PARA CC Weapon (-3).
- **Option 2:** **14 / 0.5** — Hacker, EVO Hacking Device; PARA CC Weapon (-3).
- **Option 3:** **17 / 0** — Repeater, Total Reaction; Combi Rifle, PARA CC Weapon (-3).

### Knauf — `knauf-outlaw-sniper`

**Unit ID:** 939 — AVA 1 — LI, Character.

- **Stats:** `10-10 21 13 11 13 1 0 1 2`.
- **Rules/equipment:** Multispectral Visor L1, BS Attack bonuses, Courage, Mimetism (-3), Stealth, Terrain (Total).
- **Option 1:** **31 / 1.5** — Surprise Attack (-3), Decoy (1); MULTI Sniper Rifle, AP Heavy Pistol, CC Weapon.
- **Option 2 FTO:** **30 / 1.5** — MULTI Sniper Rifle, AP Heavy Pistol, Shock CC Weapon (PS=7).
- **Fireteam:** Outrage and Wildcard, **option 2 only**; source equivalence `Outrage`.

### Brawlers, Mercenary Enforcers — `brawlers-mercenary-enforcers`

**Unit ID:** 987 — AVA 5 — MI, Spec. Trained Troops.

- **Stats:** `10-10 17 12 11 12 2 3 1 2`.
- **Rules:** Sixth Sense.
- **Option 1:** **15 / 0** — Rifle, Light Shotgun (+1B), Pistol, CC Weapon.
- **Option 2:** **15 / 1.5** — X-Visor; Heavy Rocket Launcher, Assault Pistol, CC Weapon.
- **Option 3:** **25 / 1.5** — Multispectral Visor L2; MULTI Sniper Rifle, AP Mine, Pistol, CC Weapon.
- **Option 5:** **16 / 0.5** — Hacker, Hacking Device; Submachine Gun, Cybermine, Pistol, CC Weapon.
- **Option 6:** **19 / 0** — Engineer, Deactivator, GizmoKit; Rifle, Light Shotgun (+1B), D-Charges, Pistol, CC Weapon.
- **Option 7:** **19 / 0** — Doctor, MediKit; Rifle, Light Shotgun (+1B), Pistol, CC Weapon.
- **Option 9 Lieutenant:** **15 / 0** — Rifle, Light Shotgun (+1B), Pistol, CC Weapon; Lieutenant.
- **Fireteams:** StarCo; PMC; Armored.

### Stempler Zonds — `stempler-zonds`

**Unit ID:** 408 — AVA 1 — REM, Support Troops.

- **Stats:** `15-10 13 11 10 13 0 3 STR1 3`.
- **Rules/equipment:** Deactivator, Repeater, Remote Presence, Triangulated Fire, Courage, Forward Observer, Sensor, Climbing Plus.
- **Option 1:** **15 / 0** — Combi Rifle, Flash Pulse, PARA CC Weapon (-3).
- **Option 2:** **18 / 0** — option-1 weapons; Tactical Awareness.
- **Option 3 FTO:** **17 / 0** — option-1 weapons; Super-Jump.
- **Option 4:** **22 / 0** — Thunderbolt (+1B), Flash Pulse, PARA CC Weapon (-3); BS=12, Tactical Awareness.
- **Fireteam:** none in the StarCo chart. The option-3 `FTO` name does not itself grant access.

### Corregidor Alguaciles — `corregidor-alguaciles`

**Unit ID:** 296 — AVA 255 — LI, Line Troops.

- **Stats:** `10-10 14 11 10 13 1 0 1 2`.
- **Option 1:** **10 / 0** — Combi Rifle, Pistol, CC Weapon.
- **Option 2:** **18 / 1** — HMG, Pistol, CC Weapon.
- **Option 5:** **15 / 1.5** — Missile Launcher, Pistol, CC Weapon.
- **Option 6:** **15 / 0.5** — Hacker, Hacking Device; Combi Rifle, Pistol, CC Weapon.
- **Option 8:** **12 / 0** — Forward Observer, Deployable Repeater; Combi Rifle, Flash Pulse, Pistol, CC Weapon.
- **Option 9:** **12 / 0** — Paramedic, MediKit; Combi Rifle, Pistol, CC Weapon.
- **Option 10 Lieutenant:** **10 / 0** — Combi Rifle, Pistol, CC Weapon; Lieutenant.
- **Fireteam:** StarCo.

## Fireteams

The tables below are authoritative for StarCo Fireteam legality. Profile names such as `FTO` do not grant access by themselves.

### StarCo Fireteams

**Types:** Haris, Core.

The Army source marks Alguaciles and Mobile Brigada `required: true`. Treat them as a **required source-choice set**: at least one source member must come from those two rows.

| Member | Min | Max | Required / equivalence | Profile restriction |
|---|---:|---:|---|---|
| Alguacil | 0 | 5 | required-source set | all options |
| Mobile Brigada | 0 | 5 | required-source set | all options |
| Brawler | 0 | 2 | — | all options |
| Daktari | 0 | 1 | counts as Alguacil | option 1 |
| Señor Massacre | 0 | 1 | — | both options |
| Rumbler Spec-Ops | 0 | 1 | Spec-Ops mode only | optional-mode record |

Wildcards may join subject to the Wildcard rules below.

### Riot Grrls Fireteams

**Types:** Duo, Haris, Core.

| Member | Min | Max | Required / equivalence | Profile restriction |
|---|---:|---:|---|---|
| Riot Grrl | 1 | 5 | native source | all options |
| Avicenna | 0 | 1 | counts as Riot Grrl | option 1 |
| Fiddler FTO | 0 | 1 | counts as Riot Grrl | **option 1 only** |

Wildcards may join subject to the Wildcard rules below.

### PMC Fireteams

**Types:** Duo, Haris.

The Army source marks Brawlers and CSU `required: true`. Treat them as a **required source-choice set**.

| Member | Min | Max | Required / equivalence | Profile restriction |
|---|---:|---:|---|---|
| Brawler | 0 | 3 | required-source set; counts as PMC | all options |
| CSU | 0 | 3 | required-source set; counts as PMC | all options |
| Rumbler Spec-Ops | 0 | 1 | Spec-Ops mode only | optional-mode record |

Wildcards may join subject to the Wildcard rules below.

### Armored Fireteams

**Types:** Duo, Haris.

The Army source marks Anaconda and Triphammer `required: true`. Treat them as a **required source-choice set**.

| Member | Min | Max | Required / equivalence | Profile restriction |
|---|---:|---:|---|---|
| Anaconda | 0 | 2 | required-source set | both options |
| Triphammer | 0 | 1 | required-source set | all options |
| Brawler | 0 | 2 | — | all options |
| Mobile Brigada | 0 | 1 | — | all options |
| Irmandinho | 0 | 1 | — | both options |
| Tsyklon FTO | 0 | 1 | — | **options 1/2 only** |
| Rumbler Spec-Ops | 0 | 1 | Spec-Ops mode only | optional-mode record |

Wildcards may join subject to the Wildcard rules below.

### Outrage Fireteams

**Types:** Duo, Haris.

The Army source marks Emily and Uhahu `required: true`. Treat them as a **required source-choice set**.

| Member | Min | Max | Required / equivalence | Profile restriction |
|---|---:|---:|---|---|
| Emily Handelman | 0 | 1 | required-source set; counts as Outrage | both options |
| Uhahu | 0 | 1 | required-source set; counts as Outrage | option 1 |
| Knauf FTO | 0 | 1 | counts as Outrage | **option 2 only** |

Wildcards may join subject to the Wildcard rules below.

## Wildcards

| Wildcard | Max | Counts as / source comment | Profile restriction |
|---|---:|---|---|
| Digger | 2 | `Brawlers, PMC` | both options |
| Raoul Spector FTO | 1 | `PMC` | **option 3 only** |
| Emily Handelman | 1 | `Brawlers, PMC, Outrage` | both options |
| Uhahu | 1 | `Outrage` | option 1 |
| Knauf FTO | 1 | `Outrage` | **option 2 only** |

Wildcard means the listed profile may join any otherwise legal StarCo Fireteam unless another rule prevents it. The source `Counts as` labels are preserved separately because they can matter to composition requirements.

## Unit → Fireteam access index

This is a derivative lookup table. If it conflicts with the canonical Fireteam section above, the canonical section wins.

| Unit | Access |
|---|---|
| Alguaciles | StarCo — all options |
| Anaconda | Armored — both options |
| Avicenna | Riot Grrls — option 1; counts as Riot Grrl |
| Brawlers | StarCo; PMC; Armored — all options; PMC equivalence in PMC |
| CSU | PMC — all options; counts as PMC |
| Daktari | StarCo — option 1; counts as Alguacil |
| Diggers | Wildcard — both options; source labels Brawlers, PMC |
| Emily Handelman | Outrage native + Wildcard — both options; source labels Brawlers, PMC, Outrage |
| Fiddler | Riot Grrls — **option 1 FTO only**; counts as Riot Grrl |
| Irmandinhos | Armored — both options |
| Knauf | Outrage + Wildcard — **option 2 FTO only**; counts as Outrage |
| Mobile Brigada | StarCo; Armored — all options |
| Raoul Spector | Wildcard — **option 3 FTO only**; source label PMC |
| Riot Grrls | Riot Grrls — all options |
| Señor Massacre | StarCo — both options |
| Triphammer | Armored — all options |
| Tsyklon | Armored — **options 1/2 FTO only** |
| Uhahu | Outrage native + Wildcard — option 1; counts as Outrage |
| Rumbler Spec-Ops | StarCo; PMC; Armored — optional Spec-Ops mode only |

Explicit negative lookup notes:

- **Fiddler options 2/3** cannot use the Riot Grrls row.
- **Tsyklon options 4/5** cannot use the Armored row.
- **Raoul Spector option 1** cannot use the Wildcard row.
- **Knauf option 1** cannot use Outrage or the Wildcard row.
- **Stempler Zond option 3 (`STEMPLER ZOND FTO`) has no StarCo Fireteam access.**
- No other standard roster unit gains Fireteam access merely from a profile name containing `FTO` or from sharing Nomad/NA2 ancestry.

## Peripherals and composite records

- **Anaconda** has an embedded Operator state and is counted as one logical roster record.
- **Triphammer** options include one **Turtlemek Ancillary Remote**; the Turtlemek is not counted as a separate roster entry.
- **Fiddler** options 2/3 include one or two **Jackbots**; those Peripherals are not separate roster records.
- **Zondbots** are Servant Peripherals and do not generate Orders independently.
- Optional Spec-Ops / Team-Ops subprofiles and SpecBots remain inside their optional-mode records.

## Reinforcements boundary

The standard StarCo dataset exposes Reinforcements Army ID **999**. It is deliberately not merged into this file's standard roster or canonical Fireteam chart. For ordinary StarCo list building, use the 33 standard roster records and Fireteams above; use a separate Reinforcements reference when Reinforcement mode is explicitly involved.

## Validation notes

Validated against Army snapshot `7.26246.159`:

- Standard roster membership was determined from faction availability containing sectorial ID `905`.
- **33** standard logical roster records were identified.
- **2** optional-mode records were separated: Rumbler Spec-Ops (`1925`) and NA2 Team-Ops (`1939`).
- Generic `factions: []` Soldier-of-Fortune catalog entries were excluded.
- Fireteam limits are Core `1`, Haris `1`, Duo `256`.
- Canonical families are StarCo, Riot Grrls, PMC, Armored, and Outrage.
- Wildcards are Diggers, Raoul Spector FTO, Emily Handelman, Uhahu, and Knauf FTO.
- FTO restrictions were reconciled against profile option names: Fiddler `1`; Tsyklon `1/2`; Raoul Spector `3`; Knauf `2`.
- `STEMPLER ZOND FTO` was intentionally **not** granted Fireteam access because no canonical chart row grants it.
- Required-source sets and source `Counts as` labels were preserved separately.
- Reinforcement Army ID `999` remains distinct.

## Provenance

- Corvus Belli Army source revision: `7.26246.159`.
- Army data changed on: 2026-09-03.
- Source backup commit: `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b` (`army: N5.3 + ITS18`).
- Source blob: `2cde2a4e10ed912bb32d3e6e441ace255fac4d8b`.
- InfinityDB reference commit: `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Fireteam source: Army `fireteamChart` normalized into repository semantics.
- Generated/verified: 2026-10-16.
