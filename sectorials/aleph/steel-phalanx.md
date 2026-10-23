---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 702
sectorial_slug: steel-phalanx
sectorial_name: Steel Phalanx
parent_faction: ALEPH
rules_baseline: N5.3
army_source_version: "7.26246.159"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-15
coverage: "Standard Steel Phalanx roster, profiles/loadouts, canonical Fireteam chart, reverse Fireteam access, optional-mode hooks, and Reinforcements boundary."
---

# Steel Phalanx — N5.3 sectorial reference

## Overview and provenance

This file is the repository reference for **Steel Phalanx** (Army sectorial/faction ID `702`). It is intended to be sufficient for list-building analysis without reopening Army for ordinary profile, AVA, cost, SWC, or Fireteam questions.

Primary data source:

- Corvus Belli Army data snapshot mirrored by `massayoshi/infinity-army-backup`.
- Pinned source commit: `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b`.
- Army dataset: `n5/steel-phalanx/steel-phalanx.json`.
- Army version: **7.26246.159**.
- Sectorial ID: **702**.
- Parent ALEPH ID: **701**.
- Reinforcements list ID exposed by the dataset: **799**.
- Cross-check/reference model commit: InfinityDB `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: **N5.3 + N5 FAQ v0.1**.

Coverage policy:

- The **35 standard roster entries** whose faction availability includes Steel Phalanx are included below.
- Generic mercenary-catalog entries present in the aggregate Army payload but not assigned to faction `702` are excluded.
- **Chandra Spec-Ops** and **ALEPH Team-Ops** are optional-mode hooks, not normal matched-play roster entries.
- Reinforcements are kept distinct from the normal Steel Phalanx roster and Fireteam chart.
- Army option IDs are retained where they help distinguish otherwise similar loadouts.

## Sectorial summary

Steel Phalanx is a character-heavy ALEPH sectorial built around Myrmidon visual control and close assault, durable elite pieces, unusually flexible small Fireteams, and a strong set of specialist/attack characters. Its N5.3 Army chart has a sectorial-specific Fireteam constraint that materially changes list construction:

> **Steel Phalanx Core Fireteams have a maximum of 4 members.**

Army exposes Core, Haris, and Duo as available Fireteam types, but the canonical chart below controls which units may actually form each family.

## Fireteam limits and interpretation

- **Core maximum:** 4 members in this sectorial.
- **Myrmidons:** Core.
- **Dactyls:** Duo or Haris.
- **Steel Phalanx:** Duo or Haris.
- **Thorakitai:** Core.
- **Heavy:** Duo.
- **Wildcards:** Hector, Hippolyta, Thrasymedes FTO, Alkê, Thamyris, and Arjuna FTO.
- Where Army marks multiple chart entries `required: true`, treat them as a **required source-choice set**: the team must contain a legal member from that source set; it does not mean every marked entry must be present simultaneously.
- `FTO` restrictions are profile/loadout restrictions, not aliases for the whole unit entry.
- Count-as comments such as `(Myrmidon)`, `(Thorakites)`, `(Dactyl)`, and `(Steel Phalanx)` are preserved below.

## Standard roster index

| Unit | Army ID | AVA | Type | Fireteam access |
|---|---:|---:|---|---|
| Acmon, Sergeant of Dactyls | 744 | 1 | MI | Myrmidon Core; Dactyl Duo/Haris; Thorakitai Core |
| Agamemnon the Atreides | 1594 | 1 | TAG | Heavy Duo |
| Agêma Marksmen | 602 | 2 | MI | — |
| Ajax the Great | 610 | 1 | HI | Myrmidon Core, **FTO profile only** |
| Andromeda | 788 | 1 | MI | — |
| Arjuna Unit | 1178 | 1 | MI | Wildcard, **FTO profiles only** |
| Atalanta | 605 | 1 | MI | — |
| Chandra Sergeant Thrasymedes | 615 | 1 | MI | Wildcard, **FTO profile only**, counts as Thorakites |
| Dactyls | 616 | 2 | MI | Myrmidon Core; Dactyl Duo/Haris; Steel Phalanx Duo/Haris; Thorakitai Core; Heavy Duo |
| Daleth Rebots | 590 | 2 | REM | — |
| Ekdromoi | 603 | 4 | MI | — |
| Eudoros | 609 | 1 | HI | Myrmidon Core; counts as Myrmidon |
| Hector | 754 | 1 | HI | Wildcard |
| Hippolyta | 1471 | 1 | WB | Wildcard; counts as Myrmidon |
| Hoplites | 1591 | 3 | HI | Steel Phalanx Duo/Haris; Heavy Duo |
| K2 Auxiliars | 1856 | 2 | HI | Dactyl/Steel Phalanx/Thorakitai, **FTO profiles only** |
| Lamedh Rebots | 593 | 2 | REM | — |
| Machaon | 607 | 1 | WB | Myrmidon Core; counts as Myrmidon |
| Makhai | 1593 | 3 | MI | Steel Phalanx Duo/Haris; Thorakitai Core |
| Myrmidon Officer | 601 | 3 | WB | Myrmidon Core; counts as Myrmidon |
| Myrmidons | 588 | 6 | WB | Myrmidon Core |
| Nesaie Alkê | 604 | 1 | MI | Wildcard; counts as Thorakites |
| Netrods | 595 | 2 | LI | — |
| Penthesilea | 611 | 1 | WB | — |
| Phoenix | 608 | 1 | WB | Myrmidon Core; counts as Myrmidon |
| Probots | 596 | 1 | REM | — |
| Sāchā, Xenotech Hunters | 1874 | 1 | LI | — |
| Samekh Rebots | 592 | 1 | REM | — |
| Scylla | 721 | 1 | MI | Steel Phalanx Duo/Haris, **Scylla FTO / Charybdis FTO only** |
| Thamyris | 612 | 1 | LI | Wildcard |
| Thorakitai | 600 | 6 | MI | Thorakitai Core |
| Thyreos | 1592 | 2 | LI | — |
| Warcors | 50 | 1 | LI | — |
| Yudbots | 192 | 4 | REM | — |
| Zayin Rebots | 591 | 1 | REM | — |

### Optional-mode entries

| Unit | Army ID | Mode | Fireteam hook |
|---|---:|---|---|
| Chandra Spec-Ops | 1922 | Infinity Spec-Ops | Up to 1 in Myrmidon Core or Thorakitai Core |
| ALEPH Team-Ops | 1936 | Infinity Team-Ops | Optional-mode only; not part of the normal roster chart |

## Unit details

Notation: stats are `MOV CC BS PH WIP ARM BTS VITA S`. `STR` is called out where the source models Structure rather than normal Vitality. Costs are `pts / SWC`.

### Acmon, Sergeant of Dactyls — `acmon-sergeant-of-dactyls`

- **Stats:** `10-10 20 13 11 14 2 3 2 2`; AVA 1, MI.
- **Rules/equipment:** Courage, Engineer, Tactical Awareness; Deactivator, GizmoKit.
- **Option 1 — ACMON:** **31 / 0** — Combi Rifle, Panzerfaust, D-Charges, Breaker Pistol, CC Weapon; Regular + Tactical Awareness.

### Agamemnon the Atreides — `agamemnon-the-atreides`

- **Stats:** `15-10 20 14 15 14 6 6 3 6`; AVA 1, TAG, STR.
- **Rules/equipment:** Remote Presence, CC Attack (-3), Dodge (PH=11), GizmoKit (PH=11), Natural Born Warrior, Tactical Awareness, Religious Troop; ECM Guided (-6), ECM Hacker (-3).
- **Option 1:** **65 / 1.5** — AP HMG, Heavy Flamethrower, AP+DA CC Weapon; includes Karkata; Regular + Tactical Awareness.
- **Option 2:** **63 / 1.5** — AP Spitfire, Heavy Flamethrower, AP+DA CC Weapon; includes Karkata; Regular + Tactical Awareness.
- **Option 3:** **65 / 1.5** — as option 1, **Lieutenant**; includes Karkata; Regular + Tactical Awareness + Lieutenant order.
- **Karkata included profile:** `15-10 — — 10 12 0 3 1 1`, REM/STR; Courage, Dodge (+3), Mimetism (-3), Specialist Operative, Peripheral (Ancillary). Internal source cost 3; not independently selectable here.

### Agêma Marksmen — `agema-marksmen`

- **Stats:** `10-10 15 13 11 13 2 3 1 2`; AVA 2, MI.
- **Rules/equipment:** Courage, MSV2.
- **Option 1:** **27 / 1.5** — MULTI Sniper Rifle, Breaker Pistol, CC Weapon; Surprise Attack (-3), Hidden Deployment.
- **Option 3:** **27 / 1.5** — Missile Launcher, Pulzar, Breaker Pistol, CC Weapon; Camouflage (1 Use), Decoy (1).

### Ajax the Great, Myrmidon Officer — `ajax-the-great-myrmidon-officer`

- **Stats:** `10-10 24 13 16 12 5 6 2 5`; AVA 1, HI.
- **Rules:** Martial Arts L3, Natural Born Warrior, Berserk, Courage, Dodge (+5), Mimetism (-3), Stealth, No Wound Incapacitation, Impetuous, Limited Cover; source also carries BS Attack modifiers (+1B and SR-1).
- **Option 1 — AJAX FTO:** **39 / 0** — MULTI Rifle, Nanopulser, Smoke Grenades, AP Heavy Pistol, EXP CC Weapon. **Only this profile may use Myrmidon Fireteam access.**
- **Option 2 — AJAX:** **45 / 0** — same weapons plus Forward Deployment (+20); not FTO.

### Andromeda — `andromeda`

- **Stats:** `15-5 21 12 12 13 2 3 1 4`; AVA 1, MI.
- **Rules:** Martial Arts L3, Courage, Dodge (+5), Guard, Immunity (Shock), Mimetism (-3), Specialist Operative, Stealth, NWI, Infiltration (PH=15).
- **Option 5:** **30 / 0** — Submachine Gun, Zapper, Flash Pulse, D-Charges, Breaker Pistol, DA CC Weapon.
- **Option 6:** **33 / 0** — Boarding Shotgun, Zapper, Flash Pulse, D-Charges, Breaker Pistol, DA CC Weapon.

### Arjuna Unit — `arjuna-unit`

- **Stats:** `15-5 17 13 11 14 3 3 1 2`; AVA 1, MI.
- **Rules:** Immunity (Shock), Mimetism (-3), Specialist Operative, Dodge (+5), Tactical Awareness, Religious Troop. Non-FTO profiles below add Forward Deployment (+20).
- **FTO option 1:** **21 / 0** — Boarding Shotgun, Flash Pulse, D-Charges, Breaker Pistol, CC Weapon.
- **Option 2:** **32 / 0** — option-1 weapons + Forward Deployment; includes **KiranBot 1**.
- **Option 3:** **25 / 0** — option-1 weapons + Forward Deployment; no peripheral.
- **FTO option 7:** **30 / 1.5** — Spitfire, D-Charges, Breaker Pistol, CC Weapon; TinBot Firewall (-3).
- **Option 8:** **42 / 1.5** — option-7 weapons + Forward Deployment; includes KiranBot 1.
- **Option 9:** **35 / 1.5** — option-7 weapons + Forward Deployment; no peripheral.
- **FTO option 10:** **23 / 0** — AP Submachine Gun, E/Mitter, D-Charges, Breaker Pistol, CC Weapon; TinBot Firewall (-3).
- **Option 11:** **33 / 0** — option-10 weapons + Forward Deployment; includes KiranBot 1.
- **Option 12:** **26 / 0** — option-10 weapons + Forward Deployment; no peripheral.
- **Option 13:** **32 / 0** — option-1 weapons + Forward Deployment; includes **KiranBot 2**.
- **Option 14:** **33 / 0** — option-10 weapons + Forward Deployment; includes KiranBot 2.
- **Option 15:** **42 / 1.5** — option-7 weapons + Forward Deployment; includes KiranBot 2.
- **KiranBots:** `15-5 13 11 11 11 1 3 1 2`, REM/Peripheral; ECM Hacker (-3), Peripheral (Synchronized), Courage, Forward Deployment (+20), Dodge (+2.5), Mimetism (-6). KiranBot 1: Deployable Repeater, E/Marat, AP Heavy Pistol, PARA CC Weapon. KiranBot 2: Pulzar, Repeater, AP Heavy Pistol, PARA CC Weapon. Each is internal 7 points.

### Atalanta, Agêma's NCO — `atalanta-agema-s-nco`

- **Stats:** `10-10 15 15 11 14 2 3 1 2`; AVA 1, MI.
- **Rules/equipment:** MSV2, BS Attack (Shock), Courage, Immunity (Shock), Marksmanship; TinBot Discover (ReRoll).
- **Option 1:** **38 / 1.5** — MULTI Sniper Rifle, Pistol, CC Weapon; Surprise Attack (-3), Hidden Deployment.
- **Option 2:** **41 / 1.5** — MULTI Sniper Rifle, Pistol, CC Weapon; Total Reaction.

### Chandra Sergeant Thrasymedes — `chandra-sergeant-thrasymedes`

- **Stats:** `10-10 19 12 13 13 3 0 1 2`; AVA 1, MI.
- **Rules:** Frenzy, Courage, Dodge (+2.5), Mimetism (-6), Forward Observer, Stealth.
- **Option 1 — THRASYMEDES:** **28 / 0** — Light Shotgun, E/Mitter, Flash Pulse, Boarding Pistol, Shock CC Weapon; Infiltration, Decoy (1). Not FTO.
- **Option 2 — THRASYMEDES FTO:** **28 / 0** — AP Submachine Gun, E/Mitter, Light Rocket Launcher, Boarding Pistol, Shock CC Weapon; X-Visor. Wildcard; counts as Thorakites.

### Dactyls — `dactyls`

- **Stats:** `10-10 19 12 11 13 2 3 1 2`; AVA 2, MI.
- **Rules:** Courage, Dogged.
- **Option 1 Engineer:** **20 / 0** — Combi Rifle, Adhesive Launcher Rifle, D-Charges, Breaker Pistol, CC Weapon; Deactivator, GizmoKit.
- **Option 2 Engineer:** **19 / 0** — Combi Rifle, Flammenspeer, D-Charges, Breaker Pistol, CC Weapon; Deactivator, GizmoKit.
- **Option 3 Engineer:** **20 / 0** — option 2 + Deployable Cover.
- **Option 4 Engineer:** **23 / 0** — Combi Rifle, Flammenspeer, D-Charges, Armed Turret (Marksman Rifle), Breaker Pistol, CC Weapon; Deactivator, GizmoKit.
- **Option 5 Doctor:** **20 / 0** — Combi Rifle, Adhesive Launcher Rifle, Breaker Pistol, CC Weapon; MediKit.

### Daleth Rebots — `daleth-rebots`

- **Stats:** `15-10 13 11 10 13 0 3 1 3`; AVA 2, REM/STR.
- **Rules/equipment:** Remote Presence, Courage, Triangulated Fire, Forward Observer, Sensor, Climbing Plus; Deactivator, Repeater.
- **Option 1:** **15 / 0** — Combi Rifle, Flash Pulse, PARA CC Weapon.
- **Option 2:** **18 / 0** — same weapons, Tactical Awareness; Regular + Tactical Awareness.

### Ekdromoi — `ekdromoi`

- **Stats:** `10-10 22 12 13 14 2 0 1 2`; AVA 4, MI.
- **Rules:** Martial Arts L3, Courage, Parachutist, Combat Jump, Stealth, Dodge (+2.5), Super-Jump (Jet Propulsion).
- **Option 3:** **32 / 1.5** — Spitfire, Nanopulser, AP Heavy Pistol, DA CC Weapon.
- **Option 4:** **18 / 0** — Chain Rifle, AP Heavy Pistol, DA CC Weapon.
- **Option 6 Hacker:** **23 / 0.5** — Chain Rifle, AP Heavy Pistol, DA CC Weapon; Hacking Device.
- **Option 7 Hacker:** **25 / 0** — Submachine Gun, Flash Pulse, AP Heavy Pistol, DA CC Weapon, D-Charges; Killer Hacking Device.

### Eudoros, Myrmidon Officer — `eudoros-myrmidon-officer`

- **Stats:** `15-5 23 13 13 14 3 6 2 2`; AVA 1, HI.
- **Rules:** Martial Arts L4, Courage, Dodge (+2.5), Mimetism (-6), Number 2, Specialist Operative, Stealth, Impetuous, NCO, Limited Cover.
- **Option 1:** **36 / 0** — Mk12, Nanopulser, Heavy Pistol, DA CC Weapon; Regular + Impetuous.

### Hector, Homeridae's Champion — `hector-homerid-champion`

- **Stats:** `10-10 24 13 14 15 5 6 2 2`; AVA 1, HI.
- **Rules/equipment:** Martial Arts L4, Courage, Dodge (+5), Stealth, NWI, Strategos L1, X-Visor; TinBot Firewall (-3).
- **Option 1:** **61 / 0** — Plasma Rifle, Nanopulser, E/M Grenades, Heavy Pistol, EXP CC Weapon.
- **Option 2:** **60 / 1.5** — Spitfire, Nanopulser, E/M Grenades, Heavy Pistol, EXP CC Weapon.
- **Option 3 Lieutenant:** **65 / 0** — option 1 weapons; Lieutenant (+1 Order), generating 2 Lieutenant orders.
- **Option 4 Lieutenant:** **64 / 0.5** — option 2 weapons; Lieutenant (+1 Order), generating 2 Lieutenant orders.

### Hippolyta, Amazon Officer — `hippolyta-amazon-officer`

- **Stats:** `15-5 24 13 14 14 3 3 2 2`; AVA 1, WB.
- **Rules:** Impetuous, Martial Arts L3, Berserk, Courage, Dodge (+2.5), Mimetism (-6), Stealth, Super-Jump, Limited Cover.
- **Option 1:** **37 / 0** — Breaker Combi Rifle, Nanopulser, Flash Pulse, Smoke Grenades, Pistol, EXP CC Weapon; Regular + Impetuous.

### Hoplites Heavy Regiment — `hoplites`

- **Stats:** `15-5 20 13 13 13 3 6 2 2`; AVA 3, HI.
- **Rules:** CC Attack (-3), Dodge (+2.5), Natural Born Warrior, Immunity (Enhanced), Combat Instinct, Religious Troop.
- **Option 1:** **40 / 1.5** — HMG, Pulzar, AP Heavy Pistol, E/M CC Weapon.
- **Option 2:** **37 / 1** — Red Fury, Pulzar, AP Heavy Pistol, E/M CC Weapon.
- **Option 3 Specialist:** **36 / 0** — MULTI Rifle, Pulzar, Drop Bears, AP Heavy Pistol, E/M CC Weapon; Specialist Operative.
- **Option 4 Engineer:** **39 / 0** — option-3 weapons; GizmoKit, Engineer.
- **Option 5 Engineer:** **42 / 0** — option-3 weapons + Armed Turret (Combi Rifle); GizmoKit, Engineer.
- **Option 6 Lieutenant:** **40 / 1** — HMG, Pulzar, AP Heavy Pistol, E/M CC Weapon; Lieutenant.

### K2 Auxiliars — `k2-auxiliars`

- **Stats:** `10-10 18 11 12 13 2 3 1 2`; AVA 2, HI/STR.
- **Rules:** Courage, NWI, Remote Presence.
- **Option 1 — K2 AUXILIAR FTO:** **11 / 0** — E/Marat, Flash Pulse, Breaker Pistol, PARA CC Weapon.
- **Option 2 — K2 AUXILIAR FTO:** **12 / 0** — Flash Pulse, Mine Dispenser, Breaker Pistol, PARA CC Weapon.
- **Option 3 — K2 AUXILIAR FTO:** **12 / 0** — source duplicate of option 2; retained as a distinct Army option ID.
- **Option 4 — K2 AUXILIAR:** **18 / 0** — E/Marat, Flash Pulse, Breaker Pistol, PARA CC Weapon; GizmoKit, Parachutist, Super-Jump (Jet Propulsion), Specialist Operative. Not FTO.

### Lamedh Rebots — `lamedh-rebots`

- **Stats:** `15-15 13 8 11 13 0 3 1 3`; AVA 2, REM/STR.
- **Rules/equipment:** Remote Presence, Courage, Mimetism (-3), Repeater.
- **Option 1:** **7 / 0** — Flash Pulse, PARA CC Weapon.

### Machaon, Myrmidon Doctor-Officer — `machaon`

- **Stats:** `10-10 22 12 13 15 2 3 1 2`; AVA 1, WB.
- **Rules/equipment:** Martial Arts L3, Courage, Dodge (+2.5), Frenzy, Immunity (Shock), Doctor, Mimetism (-6), Stealth, NWI; MediKit.
- **Option 1:** **37 / 0.5** — Combi Rifle, Nanopulser, Smoke Grenades, Pistol, DA CC Weapon.
- **Option 2 Lieutenant:** **37 / 0.5** — same weapons; Lieutenant.

### Makhai — `makhai`

- **Stats:** `10-10 18 13 11 13 3 6 1 2`; AVA 3, MI.
- **Rules/equipment:** MSV1, Courage, Mimetism (-3), Stealth, Tactical Awareness; every profile generates Regular + Tactical Awareness orders.
- **Option 1:** **30 / 0** — MULTI Marksman Rifle, Zapper, Breaker Pistol, CC Weapon.
- **Option 2:** **31 / 1.5** — Missile Launcher, Zapper, Breaker Pistol, CC Weapon.
- **Option 3:** **31 / 1** — Red Fury, Zapper, Breaker Pistol, CC Weapon.
- **Option 4 FO:** **29 / 0** — K1 Combi Rifle, Zapper, Flash Pulse, D-Charges, Breaker Pistol, CC Weapon; Forward Observer.

### Myrmidon Officer — `myrmidon-officer`

- **Stats:** `10-10 23 12 13 14 2 3 1 2`; AVA 3, WB.
- **Rules:** Frenzy, Martial Arts L3, Courage, Dodge (+2.5), Mimetism (-6), Stealth, NWI, Immunity (Shock).
- **Option 1 CoC:** **31 / 0.5** — Boarding Shotgun, Nanopulser, Eclipse Grenades, Pistol, DA CC Weapon; Chain of Command.
- **Option 2 CoC:** **30 / 0.5** — AP Submachine Gun, Nanopulser, Eclipse Grenades, Pistol, DA CC Weapon; Chain of Command.
- **Option 3 Lieutenant:** **26 / 0** — option-1 weapons; Lieutenant.
- **Option 4 Lieutenant:** **25 / 0** — option-2 weapons; Lieutenant.

### Myrmidons — `myrmidons`

- **Stats:** `10-10 21 12 13 13 2 0 1 2`; AVA 6, WB.
- **Rules:** Frenzy, Martial Arts L3, Courage, Dodge (+5), Mimetism (-6), Stealth.
- **Option 1:** **23 / 0** — Combi Rifle, Nanopulser, Smoke Grenades, Pistol, AP CC Weapon.
- **Option 2:** **24 / 0** — Combi Rifle, Nanopulser, Smoke Grenades, Pistol, DA CC Weapon.
- **Option 3:** **30 / 1** — Spitfire, Nanopulser, Smoke Grenades, Pistol, DA CC Weapon.
- **Option 4:** **16 / 0** — Chain Rifle, Nanopulser, Smoke Grenades, Pistol, DA CC Weapon.
- **Option 5:** **21 / 0** — Boarding Shotgun, Smoke Grenades, Pistol, DA CC Weapon.
- **Option 6 Hacker:** **29 / 0.5** — Combi Rifle, Nanopulser, Smoke Grenades, Pistol, DA CC Weapon; Hacking Device.

### Nesaie Alkê, Thorakitai Warrant Officer — `nesaie-alke`

- **Stats:** `10-10 17 13 11 14 3 3 1 2`; AVA 1, MI.
- **Rules/equipment:** Dodge (+2.5), Combat Instinct, Immunity (Shock), Specialist Operative, Religious Troop; Deactivator, X-Visor.
- **Option 1:** **27 / 0** — MULTI Rifle, Pulzar, Disco Baller, Pistol, CC Weapon; NCO.
- **Option 2:** **31 / 1.5** — AP Spitfire, Pulzar, Disco Baller, Pistol, CC Weapon; NCO.
- **Option 3 Lieutenant:** **29 / 1** — AP Spitfire, Pulzar, Disco Baller, Pistol, CC Weapon; Lieutenant.

### Netrods — `netrods`

- **Stats:** `— — — — — 0 3 1 2`; AVA 2, LI/STR.
- **Rules:** Warhorse, Combat Jump (PH=12), Religious Troop. **Must be deployed by Combat Jump during the Deployment Phase.**
- **Option 1:** **6 / 0** — no weapons; Regular order.

### Penthesilea, Amazon Warrioress — `penthesilea`

- **Stats:** `20-15 23 13 11 13 2 3 2 4`; AVA 1, WB; Motorcycle.
- **Rules:** Impetuous, CC Attack (-6), Courage, Dodge (+5), Mimetism (-3), Specialist Operative, Limited Cover, Immunity (ARM).
- **Option 2145:** **28 / 0** — AP Submachine Gun, Zapper, Smoke Grenade Launcher, Pistol, Monofilament CC Weapon; Regular + Impetuous.

### Phoenix, Veteran Myrmidon Officer — `phoenix-veteran-myrmidon-officer`

- **Stats:** `10-10 23 13 13 14 2 3 1 2`; AVA 1, WB.
- **Rules:** Martial Arts L3, Courage, Dodge (+2.5), Immunity (Shock), Mimetism (-6), Stealth, NWI, Warhorse.
- **Option 1:** **32 / 1.5** — Heavy Rocket Launcher, Nanopulser, Heavy Pistol, DA CC Weapon.
- **Option 2 Lieutenant:** **32 / 1.5** — same weapons; Lieutenant.

### Probots — `probots`

- **Stats:** `10-10 13 11 10 13 2 3 1 4`; AVA 1, REM/STR.
- **Rules/equipment:** Remote Presence, Courage; Baggage.
- **Option 1:** **8 / 0** — PARA CC Weapon; Deactivator, Repeater.
- **Option 2 EVO Hacker:** **14 / 0.5** — PARA CC Weapon; EVO Hacking Device; Hacker.
- **Option 3 TR:** **17 / 0** — Combi Rifle, PARA CC Weapon; Repeater, Total Reaction.

### Sāchā, Xenotech Hunters — `sacha-xenotech-hunters`

- **Stats:** `10-10 17 11 12 13 0 3 1 2`; AVA 1, LI, Irregular.
- **Rules:** Forward Deployment (Army source modifier ID 26), Booty, Terrain (Army source modifier ID 33), Climbing Plus, Specialist Operative.
- **Option 1:** **6 / 0** — Flash Pulse, E/M Grenades, Stun Pistol, CC Weapon; Irregular order.

### Samekh Rebots — `samekh-rebots`

- **Stats:** `15-10 13 12 10 13 0 3 1 3`; AVA 1, REM/STR.
- **Rules:** Remote Presence, Courage; Army also applies the missile-system BS Attack modifier encoded as source extra ID 31.
- **Option 1:** **16 / 1.5** — Missile Launcher, PARA CC Weapon.

### Scylla, Steel Phalanx's Sergeant — `scylla`

- **Stats:** `10-10 20 12 11 13 2 6 1 2`; AVA 1, MI.
- **Rules/equipment:** Courage, Immunity (Shock), Terrain (source modifier 37); ECM Hacker (-3).
- **Option 1 — SCYLLA:** **32 / 0.5** — E/Mitter, Light Shotgun, Pitcher, Pistol, Shock CC Weapon; Hacking Device with Army upgrade 352 (Trinity SR-2); includes Devabot Charybdis.
- **Option 3 — SCYLLA:** **32 / 0.5** — same weapons; EVO Hacking Device with Army upgrade 352; includes Devabot Charybdis.
- **Option 7 — SCYLLA FTO:** **25 / 0.5** — E/Mitter, Light Shotgun, Pitcher, Pistol, Shock CC Weapon; Hacking Device with Army upgrade 352; **no peripheral**.
- **Devabot Charybdis:** `15-10 15 11 10 11 0 3 1 2`, REM/Peripheral; ECM Hacker (-3), Repeater, Courage, Peripheral (Synchronized), Terrain (source modifier 37); Heavy Flamethrower, PARA CC Weapon; internal 7 points.
- **Charybdis FTO:** `15-10 15 11 10 11 0 3 1 2`, AVA 1 REM/STR; Remote Presence, Courage, Terrain (source modifier 37), ECM Hacker (-3), Repeater; Heavy Flamethrower, Heavy Pistol, PARA CC Weapon; internal 12 points.
- **Combined Army option:** **Scylla FTO + Charybdis FTO = 37 / 0.5**, 2 Regular orders. Both profiles are legal Steel Phalanx-Fireteam entries as specified by the chart.

### Thamyris the Aoidos — `thamyris-the-aoidos`

- **Stats:** `10-10 17 12 12 14 1 3 1 2`; AVA 1, LI.
- **Rules:** Dodge (-3), NWI, Journalist; Hacking Device with source upgrades encoded as IDs 25 and 12.
- **Option 1:** **27 / 0.5** — E/Mitter, Pitcher, Pulzar, Assault Pistol, CC Weapon; Hacker.
- **Option 2:** **28 / 0.5** — option 1 + Cybermine; Hacker.
- **Option 3:** **21 / 0.5** — Pitcher, Pulzar, Flash Pulse, Cybermine, Assault Pistol, CC Weapon; Hacker, Minelayer.

### Thorakitai — `thorakitai`

- **Stats:** `10-10 16 12 11 13 3 0 1 2`; AVA 6, MI.
- **Option 1:** **12 / 0** — Submachine Gun, E/Mitter, Pulzar, Pistol, CC Weapon.
- **Option 2:** **14 / 0** — Combi Rifle, Nanopulser, Pistol, CC Weapon.
- **Option 3:** **17 / 0** — Submachine Gun, Light Rocket Launcher, Pistol, CC Weapon.
- **Option 4:** **22 / 1.5** — HMG, Nanopulser, Pistol, CC Weapon.
- **Option 6 FO:** **13 / 0** — Submachine Gun, E/Mitter, Pulzar, Flash Pulse, Pistol, CC Weapon; Forward Observer.
- **Option 7 Paramedic:** **14 / 0** — Submachine Gun, E/Mitter, Pulzar, Pistol, CC Weapon; MediKit, Paramedic.
- **Option 9:** **23 / 1.5** — Feuerbach, Nanopulser, Pistol, CC Weapon.
- **Option 12 Hacker:** **19 / 0.5** — Combi Rifle, Nanopulser, Pistol, CC Weapon; Hacking Device.
- **Option 13 Specialist:** **16 / 0** — Combi Rifle, Nanopulser, Pistol, CC Weapon; Commlink, Specialist Operative.

### Thyreos, Thyreophoroi Mobile Regiment — `thyreos`

- **Stats:** `15-5 21 12 10 13 2 3 1 2`; AVA 2, LI.
- **Rules:** CC Attack (-6), Forward Deployment (+20), Dodge (+5), Natural Born Warrior, Mimetism (-3), Stealth, Religious Troop, Surprise Attack (-3), Camouflage (1 Use).
- **Option 1:** **22 / 0** — Boarding Shotgun, D-Charges, Shock Mine, Pistol, Monofilament CC Weapon.
- **Option 2:** **21 / 0** — Submachine Gun, D-Charges, Shock Mine, Pistol, Monofilament CC Weapon.
- **Option 3 Minelayer:** **22 / 0.5** — option-2 weapons; Minelayer.
- **Option 4 FO:** **22 / 0** — option-2 weapons + Flash Pulse; Forward Observer.
- **Option 5 Hacker:** **26 / 0.5** — Submachine Gun, D-Charges, E/M Mine, Pistol, Monofilament CC Weapon; Hacking Device.
- **Option 6 KHD:** **25 / 0** — Boarding Shotgun, D-Charges, E/M Mine, Pistol, Monofilament CC Weapon; Killer Hacking Device.

### Warcors, War Correspondents — `warcors-war-correspondents`

- **Stats:** `10-10 11 9 11 13 0 0 1 2`; AVA 1, LI, Irregular.
- **Rules:** Journalist.
- **Option 1:** **3 / 0** — Flash Pulse, Stun Pistol, PARA CC Weapon; 360º Visor.
- **Option 2:** **3 / 0** — same weapons; Sixth Sense instead of 360º Visor.

### Yudbots — `yudbots`

- **Stats:** `15-10 11 8 10 13 0 3 1 1`; AVA 4, REM/Peripheral/STR.
- **Rules:** Peripheral (Servant), Courage, Mimetism (-3).
- **Option 1:** **3 / 0** — PARA CC Weapon; no independent order (`minis: 0` in Army option data).

### Zayin Rebots — `zayin-rebots`

- **Stats:** `15-10 13 11 10 13 0 3 1 3`; AVA 1, REM/STR.
- **Rules/equipment:** Remote Presence, Courage, Total Reaction, Climbing Plus; 360º Visor.
- **Option 1:** **24 / 1** — HMG, PARA CC Weapon.
- **Option 2:** **19 / 0** — Thunderbolt, PARA CC Weapon.

## Canonical Fireteam chart

This section is authoritative for Steel Phalanx Fireteam membership. The source chart is the `fireteamChart` object in Army version `7.26246.159`.

### Myrmidons Fireteams — Core

**Allowed type:** Core. **Sectorial Core cap:** 4 models.

| Entry | Min | Max | Required-source | Count-as / restriction |
|---|---:|---:|---|---|
| Myrmidon Officer | 0 | 3 | yes | Myrmidon |
| Machaon | 0 | 1 | yes | Myrmidon |
| Eudoros | 0 | 1 | yes | Myrmidon |
| Phoenix | 0 | 1 | yes | Myrmidon |
| Ajax FTO | 0 | 1 | yes | Myrmidon; **FTO profile only** |
| Myrmidon | 0 | 4 | no | Native Myrmidon |
| Acmon | 0 | 1 | no | — |
| Dactyl | 0 | 1 | no | — |
| Chandra Spec-Ops | 0 | 1 | no | Optional Spec-Ops mode only |

At least one member must come from the chart's required Myrmidon-source set. Wildcards may join subject to normal Fireteam legality and the four-model Core cap.

### Dactyls Fireteams — Duo / Haris

| Entry | Min | Max | Count-as / restriction |
|---|---:|---:|---|
| Dactyl | 1 | 2 | Native Dactyl |
| Acmon | 0 | 1 | Dactyl |
| K2 Auxiliar FTO | 0 | 1 | Dactyl; **FTO profile only** |

### Steel Phalanx Fireteams — Duo / Haris

| Entry | Min | Max | Required-source | Count-as / restriction |
|---|---:|---:|---|---|
| Makhe | 0 | 3 | yes | Steel Phalanx |
| Hoplite | 0 | 2 | yes | Steel Phalanx |
| Scylla FTO | 0 | 1 | no | Steel Phalanx; **FTO profile only** |
| Charybdis FTO | 0 | 1 | no | Steel Phalanx; source entry under Scylla |
| K2 Auxiliar FTO | 0 | 1 | no | **FTO profile only** |
| Dactyl | 0 | 1 | no | — |

At least one member must come from the required Steel-Phalanx-source set: Makhe or Hoplite.

### Thorakitai Fireteams — Core

**Allowed type:** Core. **Sectorial Core cap:** 4 models.

| Entry | Min | Max | Count-as / restriction |
|---|---:|---:|---|
| Thorakites | 1 | 4 | Native Thorakites |
| Dactyl | 0 | 2 | — |
| Makhe | 0 | 1 | — |
| K2 Auxiliar FTO | 0 | 1 | **FTO profile only** |
| Acmon | 0 | 1 | — |
| Chandra Spec-Ops | 0 | 1 | Optional Spec-Ops mode only |

Wildcards may join subject to normal legality and the four-model Core cap.

### Heavy Fireteams — Duo

| Entry | Min | Max | Required-source | Restriction |
|---|---:|---:|---|---|
| Agamemnon | 0 | 1 | yes | — |
| Hoplite | 0 | 1 | yes | — |
| Dactyl | 0 | 1 | no | — |

At least one member must come from the required Heavy-source set: Agamemnon or Hoplite.

### Wildcards

| Wildcard | Max | Count-as / restriction |
|---|---:|---|
| Hector | 1 | — |
| Hippolyta | 1 | Myrmidon |
| Thrasymedes FTO | 1 | Thorakites; **FTO profile only** |
| Alkê | 1 | Thorakites |
| Thamyris | 1 | — |
| Arjuna FTO | 1 | **FTO profiles only** |

Wildcard status does not erase profile restrictions or satisfy a family-specific required-source condition unless the Army chart explicitly supplies the appropriate count-as/source relationship.

## Reverse index — unit → Fireteam access

| Unit | Fireteam access |
|---|---|
| Acmon | Myrmidon Core (max 1); Dactyl Duo/Haris (max 1, counts as Dactyl); Thorakitai Core (max 1) |
| Agamemnon | Heavy Duo (max 1; required-source candidate) |
| Agêma | None |
| Ajax | Myrmidon Core, **FTO only**, max 1; required-source candidate; counts as Myrmidon |
| Andromeda | None |
| Arjuna | Wildcard, **FTO options only** |
| Atalanta | None |
| Thrasymedes | Wildcard, **FTO option only**; counts as Thorakites |
| Dactyl | Myrmidon Core max 1; Dactyl Duo/Haris min 1 / max 2 as native source; Steel Phalanx Duo/Haris max 1; Thorakitai Core max 2; Heavy Duo max 1 |
| Daleth | None |
| Ekdromoi | None |
| Eudoros | Myrmidon Core max 1; required-source candidate; counts as Myrmidon |
| Hector | Wildcard max 1 |
| Hippolyta | Wildcard max 1; counts as Myrmidon |
| Hoplite | Steel Phalanx Duo/Haris max 2, required-source candidate; Heavy Duo max 1, required-source candidate |
| K2 Auxiliar | Dactyl Duo/Haris max 1, **FTO only**, counts as Dactyl; Steel Phalanx Duo/Haris max 1, **FTO only**; Thorakitai Core max 1, **FTO only** |
| Lamedh | None |
| Machaon | Myrmidon Core max 1; required-source candidate; counts as Myrmidon |
| Makhe | Steel Phalanx Duo/Haris max 3, required-source candidate; Thorakitai Core max 1 |
| Myrmidon Officer | Myrmidon Core max 3; required-source candidate; counts as Myrmidon |
| Myrmidon | Myrmidon Core max 4 |
| Alkê | Wildcard max 1; counts as Thorakites |
| Netrod | None |
| Penthesilea | None |
| Phoenix | Myrmidon Core max 1; required-source candidate; counts as Myrmidon |
| Probot | None |
| Sāchā | None |
| Samekh | None |
| Scylla | Steel Phalanx Duo/Haris: Scylla FTO max 1 and/or Charybdis FTO max 1 as separate chart entries |
| Thamyris | Wildcard max 1 |
| Thorakites | Thorakitai Core min 1, max 4 |
| Thyreos | None |
| Warcor | None |
| Yudbot | None |
| Zayin | None |
| Chandra Spec-Ops | Optional-mode only: Myrmidon Core max 1; Thorakitai Core max 1 |

## Reinforcements boundary

Army version `7.26246.159` points Steel Phalanx to **Reinforcements list ID 799**. Reinforcement entries and any Reinforcement-specific Fireteams are not merged into the standard roster or standard Fireteam chart above. When analyzing a Reinforcements game, load the Reinforcements list as a separate force component and apply its own availability/chart rather than treating its units as normal Steel Phalanx AVA.

## Tactical tags

These tags are analytical conveniences, not rules text.

- **Vision control:** Myrmidons, Myrmidon Officer, Machaon, Ajax, Hippolyta, Penthesilea; Eclipse specifically on Myrmidon Officers.
- **Long-range / ARO:** Atalanta, Agêma, Phoenix, Makhai ML, Thorakitai Feuerbach/HMG, Zayin, Samekh.
- **Close assault:** Ajax, Hippolyta, Myrmidons, Eudoros, Machaon, Phoenix, Penthesilea, Thyreos, Andromeda.
- **Airborne / vertical attack:** Ekdromoi; K2 non-FTO specialist profile; Netrods are deployment-only Combat Jump order pieces.
- **Hacking / network:** Myrmidon Hacker, Ekdromoi HD/KHD, Scylla, Thamyris, Thorakitai Hacker, Thyreos HD/KHD, Probot EVO; Lamedh/Daleth/Probots and KiranBots contribute Repeaters or deployable network tools.
- **Engineers:** Dactyls, Acmon, Hoplites Engineer profiles; Yudbots extend support reach.
- **Doctors/medical:** Machaon, Dactyl Doctor, Thorakitai Paramedic; Yudbots extend support reach.
- **Orders/economy:** Netrods, Hector Lieutenant (+1 Order), Makhai Tactical Awareness, Arjuna Tactical Awareness, Acmon Tactical Awareness, Daleth Tactical Awareness, Agamemnon Tactical Awareness, NCO Eudoros/Alkê, Baggage Probot.
- **Midfield:** Andromeda, Thyreos, non-FTO Arjuna, Sāchā.

## Validation notes

- Standard roster count checked against the Steel Phalanx Army aggregate: **35** entries assigned to faction `702`, plus optional Spec-Ops/Team-Ops hooks.
- All selectable standard profiles above preserve current Army points and SWC from source version **7.26246.159**.
- FTO-only Fireteam access is explicitly retained for Ajax, Arjuna, Thrasymedes, K2 Auxiliars, Scylla, and Charybdis where the chart/profile requires it.
- Steel Phalanx's sectorial-specific **Core maximum of 4** is applied to both Myrmidon and Thorakitai Core construction.
- Generic catalog mercenaries that merely appear in the aggregate Army payload without Steel Phalanx faction availability are intentionally excluded.
- Source oddities that could matter to audits are preserved rather than silently normalized: K2 FTO options 2/3 are duplicate Army entries; Sāchā/Thamyris/Scylla retain raw source modifier IDs where the mirrored payload does not provide a sufficiently unambiguous human-readable label in the unit record itself.

## Expanded faction tactical guide

For comprehensive hero/utility choices, Myrmidon and Thorakitai architecture, Officer Eclipse, Agamemnon and alternative attacks, see the [Steel Phalanx tactical/list-building guide](../../notes/factions/steel-phalanx.md). **Read the current Fireteam chart here first:** Scylla FTO requires a legal Steel Phalanx Duo/Haris foundation, and cannot join a Thorakitai Core; Ajax requires the FTO profile for Myrmidon Core.

## Command-unit apex/value cross-reference (2026-10-23)

**Hector LT(+1) 64–65** makes both personal Lieutenant Orders **Regular** through Strategos L1, improving a hero-focused force's cross-unit order flexibility. **Myrmidon Officer CoC 30–31/0.5** contributes Eclipse, Mimetism(-6) and close-range utility as an actual backup, but loses insurance value if sent into the same deadly assault as Hector. Compare **Alkê/Eudoros NCO and Makhai/Arjuna/Acmon Tactical Awareness** based on which teams really receive useful activations; L1 does not grant the L2 free group transfer.

See [cross-game Lieutenant, CoC and Order-economy tiers](../../notes/list-building/command-units-apex-and-value.md). **Current pinned profiles and Fireteam chart above govern legality.**

## TAG tactical cross-reference (2026-10-23)

**Agamemnon (63–65)** is one of the strongest pure **points-value** TAGs: AP HMG, TacAware, useful CC deterrence, and enough budget left for independent Steel Phalanx pressure. It is not an Avatar-style unkillable solo plan (ARM6 and hacking vulnerability). The 2025 tier-list hosts debate high-A versus S **peak** ranking; practical points efficiency is much less disputed.

Across all factions, compare **apex power** separately from **points value**, counterplay and mission fit: [N5.3 TAG guide](../../notes/list-building/tags.md). The current unit profiles and canonical Fireteam chart above take precedence over tactical opinions.

## Hacker and KHD tactical cross-reference (2026-10-23)

**Scylla HD + Trinity (32/0.5 with Charybdis Devabot)** pairs Pitcher/anti-Hacker attacks with a **Synchronized Repeater + flamethrower** fork; **25/0.5 FTO** drops the peripheral and relies on the canonical team chart. **Ekdromoi HD 23/0.5 or KHD 25/0** is a parachute/Combat Jump specialist, especially valuable when target consoles are far beyond the initial network. **Myrmidon HD 29/0.5** combines smoke/Mimetism(-6) and scoring in a fast assault group. Scylla's **EVO variant** is for supportware, not a replacement for HD or KHD. **Why:** Steel Phalanx spends heavily on Myrmidon combat and smoke; take a linked network when it improves their approach, but avoid paying twice for hackers who cannot project beyond the team.

See the [cross-game apex/value Hacker/KHD tier guide](../../notes/list-building/hackers-and-killer-hackers.md). **The sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative; device upgrades are profile-specific.**


## Cheerleader / Order-generation tactical cross-reference (2026-10-23)

For cross-faction **apex** and **points-value** rankings, the Order types, situational counterexamples and transcript-backed disagreements, see [Cheerleaders and Order Generators — N5.3](../../notes/list-building/cheerleaders-and-order-generators.md). Roster profiles/AVA/Fireteam legality above take precedence.

- **6pt Netrod**: cheapest Regular pool Order where roster-legal, but its mandatory deployment and stationary non-combat body are a risk

**List-building test:** count *transferable* Regular Orders by Combat Group after deployment; include required link members/command enablers, physical DZ footprint, and the unit's actual ARO/mission contribution. Do not treat Irregular, Tactical, Lieutenant or Peripheral activations as interchangeable generic Orders.


## ARO apex/value cross-reference (2026-10-23)

See [ARO units: N5.3 apex/value tiers, hidden-versus-visible and deployment/matchups](../../notes/list-building/aro-units-apex-and-value.md). The **current profile details here** control exact cost/SWC, Training and Fireteam eligibility; do not import another faction's link or specialist upgrades.

- **Zayin Thunderbolt TR** — 19pt/0SWC reactive volume and regular Order; protected Engineer/Yudbot route makes defeating it a repeat job
- **Samekh FTO ML** — linked launcher only when the canonical chart permits this precise profile; Guided version is not automatically a linked ARO
- **Lamedh Flash/Repeater** — cheap order/secondary ARO; better as first/last gate than primary exposed hard gun
- **Myrmidon smoke / concealed flank** — smoke/Close Assault complicates gun lanes; guard objective approaches rather than depend only on sniper
- **Thorakite link/short guard** — cheap defensive body; pair with active high-Burst shooter rather than overbuild all-static fireteams

**Choose by circumstance:** a hard long gun matters only when the opponent must cross its arc; cheaper mines, Camo markers, templates, Flash, DTWs and hacking force movement or risk without committing an entire attack plan. Budget a second layer and preserved counterattack, check pie-slicing, hidden Order cost, anti-visual bypass and repair routes.
