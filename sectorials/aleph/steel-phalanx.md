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

## Mission specialist / button-pusher choices (N5.3)

**Dactyl Engineer19–20 + Yudbot3**, or **Daleth FO15/TA18**, gives cheap tech/FO Classifieds beside expensive Myrmidon assault. **Myrmidon Officer CoC30–31/.5** is both Eclipse lane-opener and Specialist where the mission permits, but must survive if acting as LT backup. **Acmon/Artalis or legal Dactyl** lets combat links heal/repair and score as allowed; **Agamemnon Karkata** is a bundled ancillary specialist with strict activation/Order restrictions. Hector LT Strategos doesn't itself make every nearby hero a Specialist.

[Cross-game apex and value specialist tier guide](../../notes/list-building/mission-specialists-and-button-pushers-apex-value.md). The unit profiles/Fireteams above control exact legality.

## Airborne and enemy-DZ attack choices — N5.3 (2026-10-23)

**Ekdromoi Chain Rifle18/0, HD23/.5, KHD25/0 and Spitfire32/1.5** are actual Combat Jump/ordinary Parachutist profiles: ideal to hit soft support or score behind the main Myrmidon/Agamemnon lane, and they add MA3/CC22 if close. Without legal Parachutist(DZ), a safe side entry may need more movement. **Hector LT64–65 Strategos** is an *on-table* hero commander; **Myrmidon Officer CoC30–31** protects succession while opening Eclipse route but should not be the disposable backline diver. **Agamemnon TAG TacAware** is ground fire support, not Combat Jump.

See [current cross-game apex/value, landing odds and expected-trade tiers](../../notes/list-building/airborne-and-enemy-dz-attackers-apex-value.md). **This roster and Fireteam chart control exact loadout/availability.**

## Active-turn gunfighter cross-reference (2026-10-23)

**Active-turn shooting choices:** **Agamemnon AP HMG65/1.5** is a lower-cost **TAG** BS14/3STR/TacAware long-range armor-killer, but has no built-in MSV/Mimetism for unfair openings. **Achilles** is the elite **non-TAG** close/medium breakthrough and exploitation piece; it wins more useful attacks when a separate gun first eliminates strong Mimetism/long-range AROs. A legal Fireteam moves specialists up behind the attacker in the same Orders, but its required bodies add genuine cost. [Separate non-TAG and TAG attack rankings](../../notes/list-building/active-turn-gunfighters-apex-and-value.md).

## Warbands and cheap high-upside trading — N5.3

**Myrmidon Chain Rifle16/0** is a Regular/Mimetism(-6)/MA3 **Smoke+template trade** and legal team scaffolding; **current basic Myrmidon/Machaon normal Smoke is NOT Eclipse**. **Myrmidon Officer CoC30–31/.5** *does* bring **Eclipse+NWI** and command continuity; **Officer LT25–26/0** is a **different variant**. **Ajax39 FTO/45 FD+20, Machaon LT37/.5, Phoenix LT32/1.5** are premium fighting heroes, not 5pt disposable trades. Prefer a 16pt warband delivering a hero safely over throwing 37pt Doctor-LT into a speculative melee exchange.

[Current cross-game warband apex/value, target counters and LT/CoC tiers](../../notes/list-building/warbands-and-cheap-trading-units-apex-value.md). Pinned profile choices and canonical Fireteam chart in this roster remain authoritative.

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

## Doctor / Engineer / Recovery cross-reference (2026-10-23)

**Recovery:** For expensive VITA assault troops, a roster-legal **Doctor(2W)** can restore useful durability in one roll; **Sophotect** is a flexible high-WIP Doctor/Engineer if available. For the **Agamemnon TAG** or STR support, stage an eligible **Engineer/Yudbot** along the *return* route. A fast Achilles/Myrmidon assault that leaves the network cannot be counted as cheaply recoverable. [Doctor/Engineer apex and recovery odds](../../notes/list-building/doctors-engineers-and-recovery-apex-value.md).

## Close-combat assassins and counter-CC — N5.3 (2026-10-23)

**Ajax39 FTO vs 45 FD+20** is different legal delivery with MA3, NBW, Berserk, EXP and 2W/NWI; **Eudoros36** is MA4/Mimetism−6 Mk12 assault, **Hippolyta37** brings Super-Jump/Smoke/Berserk/EXP. **Andromeda30 Guard** covers LoF+ZoC around midfield corners; **Myrmidon16** is often the best *supporting* CC value by providing Regular Smoke/Mimetism−6. Opposing view: don't throw a premium melee character into enemy NBW/guard just because it has MA4; shooting the counter-piece first may be cheaper. [Cross-game CC assassin apex/value, Guard and delivery disputes](../../notes/list-building/dedicated-close-combat-assassins-apex-value.md).

## N5.3 network projection — Pitchers, Repeaters, TinBots and disposable delivery

**Scylla Hacking Device with Trinity upgrade, Pitcher and Charybdis32/.5** is a strong multi-vector package: Pitcher plus synchronized close **Repeater + flamethrower**; **FTO Scylla25/.5** has no Charybdis and team legality must be verified. **Thamyris Pitcher/Minelayer/Cybermine21/.5** combines cheap ranged projection and prepaid mine (the **27/.5** option is a distinct profile). **Arjuna KiranBots** provide selected native/Deployable Repeaters behind fast synchronized pressure. **Dispute:** building an expensive hacking network is unnecessary if Phalanx wins through Eclipse/CC and specialists; buy projection only when opponent Hackable/visors make a real program outcome likely.

[Cross-game apex/value guide, exact delivery cost and transcript disagreements](../../notes/list-building/network-projection-repeaters-pitchers-apex-value.md). Profile and Fireteam tables above remain authoritative.

## N5.3 rare abilities & unusual combinations — tactical synthesis

**Eclipse is not interchangeable with ordinary Smoke**: **Myrmidon Officer CoC+Eclipse30–31/.5** moves and insures Lieutenant; **Scylla32/.5 + synchronized Charybdis** doubles threat origins (Pitcher + Repeater/template) for one controller; **Arjuna+KiranBot** similarly gives a rare synchronized body that may have native/Deployable Repeater. **Andromeda Guard+Infiltration30/0** makes CC threat inside legal LoF+ZoC without base contact, unlike mere Martial Arts 4. **Opposing choice:** ordinary Myrmidons16/0 and a gun/mission specialist are more points efficient if neither Eclipse-assisted push nor peripheral activation is planned. Steel Phalanx **does not have OSS G:Jumper Proxies by implication**.

[Cross-faction rare abilities apex/value, mechanics, and MCP source debates](../../notes/list-building/rare-capabilities-and-unique-combinations-apex-value.md). Current roster/Fireteam profile tables above are authoritative.

## Anti-TAG / Anti-HI without hacking — N5.3 (2026-10-23)

**K2 Auxiliary11 E/Marat** and **Thorakitai12 E/Mitter** are inexpensive hard-target *state* threats; **Thyreos21 SMG/Monofilament** is a mid-priced assassin, and **Penthesilea28 Monofilament on fast motorcycle** is a high-mobility but exposed can-opener. **Myrmidon Smoke, Myrmidon Officer Eclipse** create safe approach only when the extra Orders and ammo are accounted for. **Agamemnon TAG AP HMG** and other premium assault units should not be scored as better points value than a genuinely deliverable 11pt E/Marat. [Non-hacking anti-TAG/HI apex/value and target matchups](../../notes/list-building/anti-tag-anti-heavy-infantry-non-hacking-apex-value.md).

## N5.3 objective holding, zone domination & carried-objective choices

**Eclipse-supported durable carrier** rather than raw STR: **Myrmidon Officer CoC/Eclipse30–31/.5** (eligible CoC Specialist) or other current Specialist with Myrmidon Smoke/Eclipse cover can retreat from dangerous objective lane. **Andromeda30/0 Guard/MA/Infiltration** can prevent enemy close reclaim but Guard does not mean she is automatically a normal box-carrier; check current Specialist Operative and scenario rules. **Achilles62/1.5 or Ajax39/0** are excellent **zone VP combat guards** (when non-Null) but don't silently claim Specialist where absent. **Contrary view:** compared with a 42pt Shikami elsewhere, Steel's best objective-holder is often a **separate cheap specialist** behind two complimentary Eclipse/CC bodies, not a single pricey duel hero.

[Cross-game zone-holder and carrier apex/value guide, rules, and transcript disagreements](../../notes/list-building/objective-holding-zone-domination-and-carriers-apex-value.md). Source roster/FT chart above wins over tactical comparisons.

## Anti-Tech — enemy visors, Mimetism, markers and Impersonation (2026-10-23)

**Daleth/rostered Sensor FO REM** is the low-cost **Camo/Hidden ZoC** sweep; **Agêma MSV2** and other rostered visor guns can actually threaten revealed Mimetism/Smoke targets, while **Myrmidon Smoke** provides the classic MSV firing opportunity. **Myrmidon Officer Eclipse** / rostered **Disco Baller** profiles bypass a *hostile MSV/Marksmanship* ARO rather than trying to beat it in a straight contest. **Counter:** Smoke does not deny LoF to MSV2, and enemy White Noise shuts down your MSV gun; keep an ordinary gun and a mission-focused path. Not all ALEPH/OSS Satrah/Asura profiles are legal in Steel Phalanx.

[Non-hacking & tech-specific counter-selection, N5.3 anti-tech apex/value and opposing MCP transcripts](../../notes/list-building/anti-tech-msv-mimetism-camo-impersonation-apex-value.md).

## N5.3 peripheral / synchronized / multi-body apex-value update

**Steel Phalanx multi-body** role comes primarily from **Servant recovery** rather than importing OSS Posthuman G:Jumper or Tunguska Puppetactica. Pair source-legal **Doctor (such as Machaon) or source-legal Engineer with cheap Servants**, allowing a safe support controller to affect casualty contact elsewhere; **one target per Doctor/Engineer Order, only one Servant active**. **Fireteam + support** gives multi-model coverage but is NOT Peripheral-Synchronized, nor a single controller creating two attacks on one Order. **Opposing choice:** spend ~3–6pt on two far-flank Servants when recovering Achilles/other elite is core plan; otherwise buy an independent guard or second mission specialist over unused healbots.

[Whole-game N5.3 Peripheral & Multi-Body Apex/Value guide](../../notes/list-building/peripheral-synchronized-multibody-apex-value.md). Source profiles, dependency and Fireteam tables above remain authoritative; media are opinions.

## Mission performance — battle-report evidence (2026-11-01)

| Mission(s) | Tested composition / scoring mechanism | Evidence |
|---|---|---|
| **Double Bind / anti-materiel** | Andromeda + Hoplite/Myrmidon assault and multiple real D-Charge/anti-materiel options completed objectives for 8–6 over TAK. | [#190](../../notes/battle-reports/181-190-n5-battle-report-tactical-analysis.md) |
| **Area of Interest / room entry** | Phoenix/Myrmidon smoke/Mimetism and resilient close fighters pressure access and can challenge a Cutter-style gun, but this is matchup/table-dependent. | [#092](../../notes/battle-reports/091-100-n5-battle-report-tactical-analysis.md) |
| **Critical Intervention / vulnerability** | Expensive Ajax/Phoenix/Eudoros attackers can lose their mission package if an early ARO removes a key hero. | [#225](../../notes/battle-reports/221-230-n5-battle-report-tactical-analysis.md) |

**Limits:** Do not extrapolate a generalized Steel Phalanx win rate from these single matches. Game-era qualitative evidence, not a win-rate or current Fireteam claim. [Full mission evidence audit](../../notes/battle-reports/cross-report-mission-performance-by-sectorial.md).

## Counterplay — observed N5 battle-report responses (2026-11-02)

| Threat / target | Observed response and limitation | Battle reports |
|---|---|---|
| **Against hidden gun and zone ARO** | Andromeda flanking and Myrmidon/Hoplite fast close action carried anti-materiel D-Charges through TAK Vystrel/Tankhunter denial in Double Bind 8–6. | [#190](../../notes/battle-reports/181-190-n5-battle-report-tactical-analysis.md) |
| **Counter-counterplay: hacking and E/M** | Tunguska Interventor/Heckler/Hollow Man bricked Phalanx heroes in Hardlock 5–0; Combined hidden Puzzler E/M isolated Eudoros and Vector sniper removed Ajax. | [#151](../../notes/battle-reports/151-160-n5-battle-report-tactical-analysis.md), [#225](../../notes/battle-reports/221-230-n5-battle-report-tactical-analysis.md) |
| **Defensive link protection** | Avoid clustering Phoenix/Myrmidon/Ajax in one accessible vector and preserve Dactyl/independent Specialist; Converted Steel bodies from Charontid Sepsitor became AROs against their own troops. | [#225](../../notes/battle-reports/221-230-n5-battle-report-tactical-analysis.md) |

**Limit:** #225 depends on exceptionally bad early dice and historical Sepsitor rules; check current N5.3 availability/target legality. These are historical qualitative interactions, not present N5.3 unit, Fireteam, or win-rate claims. [Full cross-report counterplay analysis](../../notes/battle-reports/n5-cross-report-counterplay-tags-hi-hacking-camo-impersonators-fireteams.md).

---

## Must-have / Go-to / Avoid — source-backed recommendations (2026)

Dated media-backed tactical judgments and miniature purchasing advice. These are qualitative opinions, **not roster/profile/Fireteam authority**; use the canonical N5.3 data above for legality.

**Original audit title:** ALEPH N5.3 — Must-have / Go-to / Avoid (YouTube and podcast evidence)

**Audit:** 23 October 2026. **Armies:** [Vanilla ALEPH](aleph.md), [Operations Subsection (OSS)](operations-subsection.md), and [Steel Phalanx](steel-phalanx.md). Current legality, profile, points, SWC, and Fireteams come from pinned **N5.3 / Army 7.26246.159 (3 September 2026)**, not video captions. Cross-check the detailed [Vanilla guide](../../notes/factions/vanilla-aleph.md), [OSS guide](../../notes/factions/operations-subsection.md), and [Steel guide](../../notes/factions/steel-phalanx.md). Podcast and YouTube statements are **players' assessments**, not measured inclusion rates.

**Method:** Independently retrieved via MCP the [June 2026 Robert Shepherd/Jordan faction-tier transcript](https://www.youtube.com/watch?v=1dW3i9dpI34), [Tactical Awareness S3 E44 OSS YouTube](https://www.youtube.com/watch?v=Jh4jVsFoHN4) and [podcast transcript](https://open.spotify.com/episode/3E6Og0ydRErBokXHYOG6PG), [Tactical Awareness Owen's Adepticon Vanilla ALEPH interview](https://open.spotify.com/episode/0YhA9K7K2xJkiCzqI7PcbV), [MetaChemistry OSS first impressions](https://open.spotify.com/episode/5ynZcV8kOHiVfemyiaOLak), [WIP12 OrderMonkey OSS](https://open.spotify.com/episode/1lx8buKkqrLgCwZB6CaSLZ), [CNN Steel Phalanx N5 deep dive](https://www.youtube.com/watch?v=6RBi4U3t-WQ), and [Robert Shepherd Steel Phalanx N4 focus](https://www.youtube.com/watch?v=764JXbnQ3jQ). The [Yellow Snake/RXron Oct 2025 Steel episode](https://www.youtube.com/watch?v=DcCXt508-CU) **failed direct YouTube transcript retrieval in this audit**; its published example lists and prior guide's notes can corroborate, but are *not* independently transcript-confirmed here. Earlier N4 material describes enduring play patterns only.

**Labels:** **Must / near-must** means a speaker calls it almost automatic or it recurs as a backbone across distinct builds; a strategically coherent omission is still possible. **Go-to** means widely useful, not “take every row.” **Avoid** means a *particular build, profile, or use* is directly criticized by a presenter or defeated by a current rules/profile check. **No confirmed never-take** is better than inventing a dominated whole unit. All three armies need Orders, meaningful attacks, and specialists; not necessarily the same named purchase.

### At a glance

| Roster | Most defensible near-must | General go-to purchases | Source-supported avoidance |
|---|---|---|---|
| **Vanilla ALEPH** | **Posthumans Mk1 Engineer13 + Mk4 HMG30**; 6pt Netrod / 7pt Lamedh cheap-order base; **Apsaras LT20** *when not using a premium LT architecture* | Pilot-X23 + RacerBots8, Tarkshya34/41, Myrmidon Smoke16, Penthesilea28, Marut86/90, Danavas22, Naga FO25, Zayin19 | No universally condemned current unit. Do not pay for vanilla **FTO** solely expecting a Fireteam. Old Dakini recommendations are illegal. |
| **OSS / OperationS** | **Posthumans Mk1 + Mk4**; **Pilot-X + RacerBots** is the clearest *explicit “auto-include” opinion*; cheap Lamedh/Netrod infrastructure | Sharvara15, Dikpala13, Apsaras LT20/TAGCom18, Tarkshya34/41, Asura HD+63/67, Zayin19/24, Riksha20/24, Artalis23, Naga25–29 | **Naga MULTI Sniper29** is *criticized* against Dasyu34 in the May 2026 podcast but **not strictly dominated** after checking full N5.3 profiles; **Samekh FTO** is **not Guided**. No defensible blanket never-take. |
| **Steel Phalanx** | **Netrods6 / Lamedh7** cheap-order shell; **Myrmidon Officer** near-default *when Eclipse/CoC is needed*. **No individual hero** qualifies as universal. | Ajax FTO39, Phoenix, Machaon, Agamemnon63/65, Thorakitai FO13, Dactyl19–20/Acmon, Agêma ML/Atalanta, Scylla32, Eudoros | Avoid **redundant expensive hero bricks** or an unsupported **Scylla FTO** profile taken for its link label; no verified current universally bad whole unit. |

### 3. Steel Phalanx

#### Must / near-must

| Choice | Why; exception | Direct recording |
|---|---|---|
| **6pt Netrods and 7pt Lamedh** | **Closest true repeating near-must.** Two Netrods + two Lamedh occur in all three example lists documented in the Oct 2025 [Yellow Snake/RXron review](https://www.youtube.com/watch?v=DcCXt508-CU), and the independent [CNN N5 list](https://www.youtube.com/watch?v=6RBi4U3t-WQ) uses two Lamedh. High-cost Greeks need a cheap Regular order floor; first models also supply Repeater/Flash Pulse. **Do not call the exact 2+2 split compulsory**: special orders, Thorakitai, specialists and board space can justify a different shell. | [CNN N5 transcript](https://www.youtube.com/watch?v=6RBi4U3t-WQ); [Steel guide source/list reconciliation](../../notes/factions/steel-phalanx.md) — Yellow Snake *transcript failed* this audit |
| **Myrmidon Officer — conditional near-default** | When LT is a fighting Machaon/Hector/Agamemnon or Eclipse is important, Officer **CoC + Eclipse** creates strong command/approach insurance. **Not automatic** when a protected LT or different visual plan makes an extra ~30pt officer poorer than another scoring body. N5 Smoke/Eclipse allocation is not the old N4 Machaon package. | [CNN N5 deep dive](https://www.youtube.com/watch?v=6RBi4U3t-WQ); [Shepherd N4 tactical explanation, corrected for current Army](https://www.youtube.com/watch?v=764JXbnQ3jQ) |

**No individual premium hero meets “in almost any Steel Phalanx list.”** Different credible builds center Ajax/Phoenix/Machaon, Agamemnon, Hector command, or Thorakitai/Scylla/Hoplite combined arms.

#### Go-to

| Unit/profile | Why / when | Evidence |
|---|---|---|
| **Ajax FTO39** | Compact Myrmidon Core assault/CC/short-middle-range battering ram; exceptionally hard to punish if paired with Smoke/Eclipse and protection. **Only Ajax FTO** joins this Core; the separate forward-deployed profile is a different deployment choice. Not compulsory if TAG/Thorakitai is main combat engine. | [CNN N5](https://www.youtube.com/watch?v=6RBi4U3t-WQ); [Yellow Snake listed builds](https://www.youtube.com/watch?v=DcCXt508-CU); [Steel guide](../../notes/factions/steel-phalanx.md) |
| **Phoenix** | Long-range heavy rocket/ARO threat in difficult-to-engage Myrmidon team; extraordinarily credible against ordinary guns, but not an auto-include once Agamemnon/Hoplite/Agêma already anchors ranged play. | [Shepherd Steel Phalanx focus (N4)](https://www.youtube.com/watch?v=764JXbnQ3jQ), *N5.3 access verified separately*; [Steel guide](../../notes/factions/steel-phalanx.md) |
| **Machaon** | WIP15 Doctor and resilient close specialist/possible LT; supports aggressive Myrmidon pieces. **Do not assume old N4 personal Eclipse access**. Skip in favor of cheaper Doctor/engineer and other LT structure if primarily buying him for an obsolete trick. | [CNN N5](https://www.youtube.com/watch?v=6RBi4U3t-WQ); [Steel guide](../../notes/factions/steel-phalanx.md) |
| **Agamemnon63–65/1.5** | Remote Presence, Tactical Awareness and AP weaponry: serious independently funded TAG that opens long/midrange lanes while infantry scores. Shepherd/Jordan (June 2026) explicitly call it one of the best TAGs. Dactyl/Yudbot repair support strongly improves its value. Obvious hackable large investment; can forgo if hero/Thorakitai attack structure has enough range. | [Shepherd/Jordan 2026, Steel segment](https://www.youtube.com/watch?v=1dW3i9dpI34); [CNN N5](https://www.youtube.com/watch?v=6RBi4U3t-WQ) |
| **Thorakitai FO13, other 12–17pt Thorakitai; Alkê NCO** | ARM3 efficient Regular mission/utility bodies, E/M, smoke-alternative, varied Thorakitai Core; Alkê converts LT orders and supports a combined-arms Core. CNN explicitly builds around this route. | [CNN N5](https://www.youtube.com/watch?v=6RBi4U3t-WQ) |
| **Agêma Missile27/1.5, Atalanta; Zayin19/24** | Anti-Mimetism/sniper/ARO lane, cheap recoverable TR backup. June 2026 reviewers specifically praise **Agêma ML Camo+Decoy** while **sniper retains Hidden Deployment**; avoid mixing versions. | [Shepherd/Jordan 2026](https://www.youtube.com/watch?v=1dW3i9dpI34) |
| **Dactyl19–20 / Acmon, Scylla32 with Charybdis** | Engineer repairs Agamemnon and Zayin; Scylla projects hacking/Pitcher plus flamethrower Repeater peripheral; supports diversified plans without another expensive CC hero. **Scylla FTO25 lacks synchronized Charybdis** unless taking the explicit independent FTO pair (37/.5). | [CNN N5](https://www.youtube.com/watch?v=6RBi4U3t-WQ); [TA Steel guide (N4 conceptual)](https://open.spotify.com/episode/4z0CSbXz8AwSubquKnZuPC) |
| **Eudoros, Hector, Thyreos/Arjuna FTO** | Distinct purpose: mobile NCO/flank; LT/Strategos command economy; early mission reach or a more economical combined-arms link. Good *when relevant*; none is a universal buy. | [CNN N5](https://www.youtube.com/watch?v=6RBi4U3t-WQ); [Steel guide](../../notes/factions/steel-phalanx.md) |

#### “Never take” audit

- **No source-backed absolute veto against any whole currently legal Steel Phalanx unit.** This army has mutually exclusive good archetypes; calling Phoenix, Eudoros, Machaon or Agamemnon “must” makes the other credible builds impossible.
- **Avoid buying two costly, redundant Greek hero Fireteams** with no Orders, independent attack vector, or objective pieces left. Shepherd's older focus and the N5 CNN sample illustrate different viable architectures. It is a **list-construction trap**, not an intrinsically weak named unit.
- **Avoid Scylla FTO25 solely because the label looks linkable** if the chosen team does not qualify. It sacrifices the synchronized Charybdis compared with **non-FTO Scylla32**. Valid FTO teams and the **Scylla FTO + independent Charybdis FTO37** are legitimate separate choices; current canonical [Steel Phalanx Fireteam chart](steel-phalanx.md#canonical-fireteam-chart) takes precedence.
- **Avoid old assumptions** that Achilles is in current Steel Phalanx, that Machaon personally gives the old Eclipse package, that a five-person Core is legal, or that non-FTO Ajax can join a Myrmidon Core. These are **legality/edition errors**, not current 'bad units'.

### Cross-army takeaways

1. **The least debatable generic ALEPH value is Posthumans where available, cheap Regular Order infrastructure, and a repair/network plan.** Steel Phalanx substitutes its compact, complementary Myrmidon/Thorakitai architecture for the OSS/Vanilla Posthuman engine.
2. **Most credible explicit “auto-include” claims in retrieved *modern* media:** Pilot-X in the May 2026 [Tactical Awareness OSS episode](https://open.spotify.com/episode/3E6Og0ydRErBokXHYOG6PG); **15pt Sharvara** is emphatically favored around 75m; the June [Shepherd/Jordan](https://www.youtube.com/watch?v=1dW3i9dpI34) review calls Posthumans extraordinary but *does not establish literal 100% tournament usage*.
3. **Profile-specific versus unit-level “never”:** A bad support purchase (EVO without targets, FTO without a legal/useful link, expensive hacker redundant with an Asura, Guided missile without Spotlight), or a duplicate gun, **does not prove the parent unit is universally bad**. Preserve disagreement, especially the Naga sniper/Dasyu sniper comparison.
4. **Current rules beat old voices on legality:** No Dakini in September ALEPH/OSS; Mk4 HMG and Mk5 FO; OSS Asura HD+ LT exists whereas **Vanilla's Asura LT is AP Spitfire**, not HD+; Steel's Agamemnon is its sole standard TAG; current Core member cap and FTO restrictions apply.

### Whole-unit purchasing audit — entire model, not single profile (2026-10-30)

**Result: no defensible all-profile, current-roster whole-unit avoid** in Vanilla ALEPH, Operations Subsection or Steel Phalanx based on the sources above. That is a positive outcome of checking the actual alternatives, **not** a missing category.

| Army | Full-model purchasing decision | Why the apparent “avoid” is not a model ban |
|---|---|---|
| **Vanilla ALEPH** | **No unit to blacklist** | FTO Maximus/Rudra cannot gain a non-existent Vanilla team bonus, but may still have a viable standalone profile. Post-update Maximus has real improved combat options; old Dakini is **unavailable** rather than an avoidable *current* model. |
| **OSS** | **No unit to blacklist** | Naga sniper versus Dasyu is disputed (+1SD versus Hidden/BS); Samekh **FTO** lacks Guided while normal Samekh **has Guided**. Yaksha's cost is contested, not all-profile dominated. |
| **Steel Phalanx** | **No unit to blacklist** | Scylla FTO sacrifices Charybdis, but standard Scylla + Charybdis and supported FTO configurations remain useful. Expensive duplicate hero teams are a **shopping/list architecture** problem, not proof an individual hero sculpt is bad. |

**Practical collection advice:** defer a pricey hero or TAG when you already own another **for the same battlefield job**, but label that as **redundancy**, not “never take” evidence. [Cross-faction buying shortlist](../../notes/factions/model-purchase-avoid-summary-2026.md).

### Worst-value, rarely needed and proxy-first miniature purchases by army (2026-10-30)

This section answers a **miniature-buying** question separately from Army list selection: which **complete units** are low-priority purchases, which **specific profiles** are weak without making their parent unit bad, which **legitimate but mission-dependent models** merit a proxy before buying, and which **extra copies** are not worth purchasing merely because AVA allows them? Cover all three N5.3 armies: **Vanilla ALEPH, Operations Subsection (OSS), Steel Phalanx**. *Rare* means situational or not needed for the source-backed standard list structures—not a measured frequency or tournament pick-rate claim. **No unit in the checked evidence is conclusively worthless across all current profiles**.

**Confidence labels:** **Strong profile avoid** is a direct negative reviewer comparison or a demonstrated profile/Fireteam mismatch; **Defer whole miniature** means its usual niche is less important to an initial collection, not mathematical domination; **Proxy first** is a **reasoned collection recommendation**, not a claimed literal podcast quote; **Contested** explicitly preserves contrary opinion or a post-review update; **Extra-copy defer** means the first model may be excellent. Roster, profile, availability and Fireteam facts use the [September 2026 Vanilla](aleph.md), [OSS](operations-subsection.md) and [Steel](steel-phalanx.md) references; dated commentators provide preferences. The linked [whole-model purchase audit](#whole-unit-purchasing-audit--entire-model-not-single-profile-2026-10-30) continues to apply.

#### 3. Steel Phalanx — expensive hero overlap, rare support bodies and known collection

For Steel Phalanx there **is** an actual checked-in [owned miniature inventory](../../inventory/steel-phalanx.md), dated **2026-10-30**. Recommendations here distinguish a model that is **bad to buy** from one that is already owned and worth *proxying in a different role*, and do not count the same shared PanO miniature twice.

| Unit / profile / buying proposal | Specific value concern or real alternative | Purchase versus proxy — **your current inventory** |
|---|---|---|
| **A second complete premium Greek hero Fireteam** (Ajax/Phoenix/Machaon/Eudoros/Hector/Officer) | **Direct architecture warning** from [CNN N5 Steel deep dive](https://www.youtube.com/watch?v=6RBi4U3t-WQ), [Steel guide](../../notes/factions/steel-phalanx.md) and older [Shepherd Steel](https://www.youtube.com/watch?v=764JXbnQ3jQ): two expensive formations compete for the same Orders and leave too few cheap scorers, even though **each hero is strong**. | **Buy none of these characters again as alternatives**: inventory already has **Ajax1, Phoenix1, Machaon1, Eudoros1, Hector1, Myrmidon Officer1, Thrasymedes1, Alkê1 and Acmon1**. Build/declare the chosen team and **proxy extra generic Myrmidon/Officer profiles only if simultaneous body count demands it**. |
| **Myrmidon and Thorakitai to AVA solely to fill a 'full Core'** | **Source Fireteam cap:** current Steel **Core max four**, even though **Myrmidon AVA6** and **Thorakitai AVA6**. Need actual required team members/missing support, not an AVA completion exercise. | **Extra-copy defer:** you own **4 Myrmidons**, **3 Thorakitai**, **1 Officer**, **2 Dactyls**, plus other eligible named models. **No automatic reason to buy Myrmidons5–6, Thorakitai4–6, Officers2–3**. Proxy the precise extra simultaneous profile when a specific legal four-body build needs it. |
| **A second Agêma or extra Atalanta/Phoenix/Ajax ranged sculpt** | **Role overlap:** **Agêma MSV2** sniper vs hidden missile, **Atalanta** high-precision long lane, **Phoenix** HRL/ARO, **Agamemnon** independent main gun; all useful but multiple costly exposed/reactive guns don't always add value. [Shepherd/Jordan 2026](https://www.youtube.com/watch?v=1dW3i9dpI34), [Steel guide](../../notes/factions/steel-phalanx.md). | **Proxy extra Agêma** rather than purchase now: you own **Agêma1/AVA2, Atalanta1, Phoenix1 and Agamemnon1**. A possible spare OSS Agêma proxy is **unconfirmed**, not counted as owned. Buy second Agêma only for a proven **two-Agêma simultaneous list**. |
| **Agamemnon TAG without Karkata / engineer or an additional TAG** | **Agamemnon is highly praised**, not a weak purchase; but the selected ancillary **Karkata**, repair plan and distinct TAG body matter. Steel's only standard TAG is **Agamemnon**, not Vanilla Marut or OSS Maximus. | **No Agamemnon purchase needed: owned1/AVA1.** Inventory reports **Karkata0** and suggests your **existing PanO Crabbot1** as a proxy; check silhouette/acceptance. **Dactyl2 + Acmon1 + Yudbots2** cover repair concepts. Do **not** buy a second/illegal Steel TAG. |
| **Unplanned extra Ekdromoi, Makhai, Hoplites or Thyreos to AVA** | **Reasoned role distinctions:** Ekdromoi flanking/Combat Jump, Makhai specialist team support, Hoplite resilient HI fighting, Thyreos camo midfield — all useful but their second/third copies cannot automatically share the attacking Order budget. | **Proxy extras first.** Owned **Ekdromos1/AVA4, Makhai2/3, Hoplite1/3, Thyreos1/2**. These gaps alone are **not a shopping list**. Buy only when a **specific simultaneous second body/Fireteam** is recurring. |
| **Scylla FTO25 purchased for automatic Charybdis + link** | **Strong loadout/legality trap:** current [Steel roster](steel-phalanx.md) distinguishes **Scylla FTO25 with NO synchronized Charybdis**, **ordinary Scylla32 with Charybdis**, and **Scylla FTO + independent Charybdis FTO37/.5** where legal. A suffix doesn't give the cheaper version all the partner's effects. | **Avoid mistaken FTO *profile* assumption; buy no duplicates.** You already own **Scylla1 and Charybdis1**, each physically distinct. Choose one **legal configuration**, and deploy Charybdis only with a profile that fields it. |
| **Arjuna as a generic extra linked gun** | **Niche but useful:** optional FTO Wildcard and unique KiranBot perimeter/specialist packages; a standalone Arjuna without a plan may be less urgent than a cheap Thorakitai/K2 or a known hero. **A selected KiranBot needs its own physical figure**. | **Proxy first, don't buy blind:** inventory has **Arjuna0 and KiranBot0**. If the list needs Arjuna **and** a bot, represent **both separately** before committing to sculpts. |
| **K2 Auxiliary FTO / ordinary K2 model missing** | **Positive role, not 'worst':** cheap E/M/mine/Fireteam support can protect Greek heroes and contest hard attack targets at lower cost than another 30–40pt character. **FTO-only** team legality must be observed. | **Best modest missing-model test:** inventory **K2 Auxiliars0/AVA2**, with a proposed **generic bot proxy**, not yet counted as owned. **Proxy suitable K2 body first**; buy a dedicated model if it routinely solves your *actual* team/defense gap. |
| **Hippolyta as extra expensive Myrmidon-style close-combat hero** | **Inferred:** powerful Mimetism(-6)/Smoke/CC and Wildcard/Counts-as roles, but your **Ajax/Eudoros/Penthesilea/Myrmidon** collection already offers a lot of fast close pressure. She could become worthwhile for a very specific Smoke/CC/legality interaction. | **Low-priority dedicate purchase; proxy first.** Inventory has **Hippolyta0/AVA1**; suggested **spare OSS model** is **unconfirmed physically**, so do not count a spare copy as guaranteed. |
| **Sāchā Xenotech Hunters for an ordinary all-comers Steel list** | **Unranked mission-specific option:** current **Steel roster explicitly includes Sāchā AVA1**, but neither the Steel recordings nor normal attacking cores establish a required model. “Rare purchase” ≠ unit is bad or illegal. | **Skip buying by default / proxy if mission needs it.** Inventory records **Sāchā0**, no concrete proxy designated. Borrow/choose a distinct appropriate body if testing. |
| **Probot Baggage/EVO as a special-purpose additional REM** | **Conditional:** cheap Baggage/Repeater is good but full **EVO** should support actual remotes/airborne units; an unused support REM can crowd an army's small deployment zone and score fewer objectives than cheap infantry. | **No dedicated Probot; proxy first.** Inventory has **Probot0/AVA1** but **2 shared PanO Mulebots** proposed as proxies. They are **the same models already counted under PanO**; verify silhouette and avoid simultaneously assigning one to two roles. |
| **A second Daleth, Lamedh, Samekh or Zayin miniature / 'all four complete Rebot lines'** | **Cheap/strong or situational:** **Lamedh7** often a best buy; **Daleth Sensor/FO**, **Zayin TR19/24** and **Samekh Guided** have distinct jobs. **Guided** needs real Targeted/Orders; don't buy separate launchers or EVO just for the possibility of using them once. | **Existing shared pool**: **2 ALEPH Rebot chassis plus 4 PanO Dronbots** potentially cover distinct Rebots **in simultaneous lists** if silhouettes/proxy rules fit. **Buy no additional Rebot as a default**. Don't count “2 ALEPH Rebots” as two *of each* family; assign a different physical chassis for each concurrently fielded REM. |
| **More Netrods, Yudbots, Dactyls or additional peripherals bought to hit AVA** | **All useful in real support context**; four Yudbots, a full Dactyl set or multiple Servants are not compulsory for every list. **Netrod cheap Orders are unusually strong** but your max count is already supplied. | Inventory: **Netrods2/AVA2, Yudbots2/AVA4, Dactyls2/AVA2**. **No Netrod/Dactyl purchases needed**; proxy a third/fourth Yudbot if a particular Doctor/Engineer plan actually needs multiple independent Servant bodies. |
| **Extra named character Thamyris, Penthesilea, Andromeda, Acmon, Atalanta etc. only to own alternate loadouts** | **Source-based shopping inference:** a single character miniature can represent different *non-simultaneous* legal loadouts; these are credible unique tools and do not need second named sculpts for normal AVA1 play. **Thamyris** provides an alternate support/Fireteam angle, not universal must or hard avoid. | **Already owned: Thamyris1, Penthesilea1, Andromeda1, Acmon1, Atalanta1**, plus named heroes above. **Use existing sculpts, proxy weapon/card variation**, and do not buy duplicates to fill imaginary profile variants. |

**Steel Phalanx purchasing priority for your *reported* collection** ([inventory, 2026-10-30](../../inventory/steel-phalanx.md)):

| Priority | What to do | Why |
|---|---|---|
| **Do not buy now** | Additional **Phoenix/Ajax/Machaon/Hector/Eudoros**, **Agamemnon**, two more **Myrmidons**, extra **Thorakitai/Officers**, extra **Agêma**, duplicate **Dactyls/Netrods** | Most needed major heroes and supporting bodies are already owned. A roster gap to **AVA** is *not* evidence of needing more models. |
| **Use already-owned shared proxies** | **PanO Crabbot → Karkata**, **PanO Mulebot → Probot**, **PanO Dronbots → suitable Rebots**; **2 owned ALEPH Rebots** assigned between actual selected types | Reuses physical models rather than buying redundant support. Check correct silhouette, base size and table-by-table collision with PanO inventory. |
| **Try by proxy if a *specific* list needs them** | **K2 Auxiliary**, **Hippolyta**, **Arjuna + KiranBot**, **Sāchā**, second **Agêma**, more **Ekdromoi/Makhai/Hoplites/Thyreos** | These are genuine missing minis/duplicate-unit possibilities, *not* guaranteed best buys. The K2 support role is particularly worth testing; Arjuna+KiranBot needs **two separate represented bodies** for that loadout. |
| **Buy after repeated play** | The **one** missing unit or peripheral whose distinct role wins missions and cannot be represented by an accepted, correctly based proxy | Avoids buying every named unit simply because the army's roster contains it. |

**High-confidence existing Steel assets not to downgrade:** **Ajax, Phoenix, Machaon, Officer, the real Myrmidon squad, Dactyl/Acmon, two Netrods, Lamedh-capable Rebots, Agamemnon, a credible Agêma/Atalanta ranged plan, Scylla with optional Charybdis**. [CNN current-version deep dive](https://www.youtube.com/watch?v=6RBi4U3t-WQ), [2026 broader ALEPH review](https://www.youtube.com/watch?v=1dW3i9dpI34), [full Steel guide](../../notes/factions/steel-phalanx.md).

#### Cross-ALEPH — good units, rare loadouts and economical proxy substitutions

**Owned-model coverage:** Steel Phalanx counts above come from the checked-in [actual inventory](../../inventory/steel-phalanx.md). No equally authoritative current **Vanilla ALEPH or OSS inventory** was found at the expected paths; thus no ALEPH/OSS owned unit counts are inferred. A suggested **“spare OSS model”** for Hippolyta does **not establish** which OSS models are physically owned.

| Buying opportunity | Better initial proxy or reuse | When a separate miniature becomes sensible |
|---|---|---|
| **Posthuman Mk1/Mk2/Mk4/Mk5 / extra Proxy sculpts** | Use distinct appropriately sized *G:Jumper body* stand-ins, each declared as Mk1 Engineer, Mk2 specialist, Mk4 HMG or Mk5 FO. Their exact silhouettes may differ and are **not one freely interchangeable physical base**. | Buy the exact Proxy Mk bodies that appear **together** in the 2–3-body combination you routinely field; **one proxy selection doesn't make 3 independent Regular Orders**. |
| **Named S2-scale heroes and support characters** (Apsaras, Sophotect, Danavas, Parvati, Claire, Shukra, Thamyris, Hippolyta, Atalanta, Ajax, Phoenix, Machaon, etc.) | Use a *distinct*, correctly based/silhouetted legal Corvus Belli miniature from the same collection, with named identity and profile stated. Check especially **large HI** and any non-S2 Silhouettes rather than assuming all heroes are S2. | When using multiple named characters **simultaneously**, the proxy isn't visually distinct, event demands closer match, or the character becomes a regular purchased favourite. |
| **Common Fireteam gun/scoring variants** (Myrmidon, Officer, Thorakitai, Yadu, Deva, Makhai, Hoplite, Posthuman Mk) | Declare the equipped profile clearly and reuse a correct-size mini **of the same troop family** for an alternate rifle/HMG/Doctor/FO/FTO card where allowed. **Only use troop families actually available in the selected ALEPH roster**; never treat a proxy as granting faction access. | Only buy another exact weapon sculpt when the chosen team needs **different bodies simultaneously**, or the organizer requires greater WYSIWYG clarity. |
| **REM chassis** (Lamedh, Daleth, Zayin, Samekh, Probot, Riksha, Dikpala, Rudra) | Test with spare compatible-size bots: **Steel has two ALEPH Rebots plus four shared PanO Dronbots, and two PanO Mulebots as potential Probot stand-ins**. Specialized support bots **may differ in size** from large combat REMs and tiny RacerBots. | Buy a distinct chassis if its **silhouette/base or simultaneous count** cannot be met, or you play REM-skew lists often. Do not assume every REM uses the same base. |
| **Multi-body teams and peripherals**: Scylla + Charybdis, Pilot-X + RacerBot(s), Arjuna + KiranBot(s), Dart + Sharvara K-9, Agamemnon + Karkata, Engineer/Doctor + Yudbot | Declare/physically represent **each fielded model and its controller**; the main figure cannot “stand for” all extras at once. **RacerBot additional Regular Orders differ from ordinary Servant/KiranBot/Charybdis order accounting**; consult exact current options. | Buy complete partners once you regularly field the combination and lack enough correctly based stand-ins. **Steel Charybdis1 and Yudbots2 already exist; Karkata0 has Crabbot proxy; Arjuna0/KiranBots0**. |
| **Heavy/TAG models**: Marut, Maximus TAG, Agamemnon; **Tarkshya Vehicle** | Proxy/borrow **correct silhouette and base** models to test a TAG-heavy list. **Steel already has Agamemnon1**; it is **not a Marut/Maximus TAG legal listing** and one large model cannot be two separate TAGs simultaneously. Tarkshya is a **Vehicle**, not a TAG. | Buy a new large model when its **specific legal roster, physical size and attack role** recur. A large TAG model with the wrong silhouette isn't a drop-in substitute at an organized event. |
| **Scylla variants / Agent Maximus vs TAG Maximus / Apsaras options / Samekh FTO vs Guided** | Most are **profile choices**, not simultaneously fielded separate named models. **Scylla FTO without Charybdis** is not the same as the **paired** option; **Agent/TAG Maximus** cannot both be selected; **Samekh FTO does not become Guided**. | Buy alternate sculpts only if a second separate legal body is needed concurrently and current event proxy rules require it. Models cannot create missing traits or legal permissions. |
| **Retired Dakini miniatures, extraneous FTO sculpts, Spec-Ops/Team-Ops** | Reuse Dakini **only as a clearly declared legal trooper proxy** with suitable Silhouette/base; optional game modes require explicit event permission. FTO status requires current roster profile and a real **sectorial Fireteam**. | No reason to buy **illegal old Dakini or optional-mode-only minis for current standard ALEPH/OSS**. |
| **Sculpt quantity to AVA** (Steel Myrmidon6, Ekdromoi4, Thorakitai6, etc.) | Start from your **actual 300pt list** and physical **simultaneous model count**. One real Myrmidon Officer represents one trooper; it cannot physically represent two different units deployed simultaneously. | Buy duplicates when proven necessary in repeated, legal list builds, not because a spreadsheet has “missing to AVA.” |

**Proxy safety and legal limits:** announce all substitutes before play; verify selected N5.3 **unit access, exact Fireteam option, Silhouette, base, physically represented secondary figures and troop count**. Check current tournament/ITS/organizer proxy conditions for organized play rather than claiming any old season's blanket rule. A model can be a proxy for another unit when legally represented and accepted; **it cannot lend weapons/skills, faction access, an unavailable Fireteam, extra Orders or missing extra bodies**.

**Bottom line for purchases:** There are **no transcript-proven universal ALEPH whole-model “never buys.”** Best direct **profile-only** skips are **OSS Samekh FTO *if the objective is Guided***, **Steel Scylla FTO *if the expectation is included Charybdis*** and **Vanilla/OSS imaginary FTO Fireteams**; the **Naga sniper vs Dasyu** is *contested*, not a settled Naga verdict. Best **whole-model deferral / proxy-first tests** are **OSS Yaksha when a cheap infiltrator suffices**, **Tarkshya when bought only as an early ARO breaker**, **additional expensive Asura/TAG/hero alternatives**, and **Steel Hippolyta/Arjuna+KiranBot/Sāchā / surplus AVA copies** given the actual inventory. Do **not** convert a weak loadout into advice to skip **Posthumans, Myrmidons, Deva/Yadu, Scylla, Agamemnon or ordinary ALEPH scoring/support REMs**.
