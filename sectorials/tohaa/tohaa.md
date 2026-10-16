---
schema_version: 1
reference_type: faction
status: current
faction_id: 801
faction_slug: tohaa
faction_name: Tohaa
rules_baseline: N5.3
army_source_version: "7.26246.159"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-15
coverage: "Standard Vanilla Tohaa roster, profile/loadout costs and AVA, Symbiont active/inactive profile groups, peripherals/composite entries, current Duo/Haris/Triad Fireteam chart and reverse access index, Lieutenant/order-control and hacking/network hooks, optional-mode content, and Reinforcements boundary."
---

# Tohaa — N5.3 faction reference

## Overview and provenance

Repository-native reference for **Tohaa** (Army faction ID `801`). Although Tohaa is a generic faction rather than a sectorial, current Army data gives it a faction-specific Fireteam chart; this file therefore uses the faction metadata convention established by the Vanilla ALEPH reference while preserving the same canonical Fireteam sections used by sectorial references.

Sources used:

- Army-derived Tohaa source revision `7.26246.159` from `massayoshi/infinity-army-backup` commit `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b` (`army: N5.3 + ITS18`, 2026-09-03).
- Aggregate dataset: `n5/tohaa/tohaa.json`; versioned snapshot: `n5/tohaa/7.26246.159.json`.
- InfinityDB normalization/semantics at commit `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: N5.3 + N5 FAQ v0.1.

Coverage notes:

- Covers the **40 standard Tohaa roster entries** in the current Army snapshot.
- `Hatail Spec-Ops` (ID `1908`) and `Tohaa Team-Ops` (ID `1909`) are optional-mode hooks and are listed separately.
- Generic Soldier-of-Fortune / mercenary-catalog objects with an empty `factions` array are excluded. Named mercenary entries explicitly assigned to faction `801` by Army are retained.
- Linked Reinforcement army ID: **899**. Reinforcement profiles are not merged into this base roster.
- Army encodes **AVA Total** as raw value `255`; this file renders it as `Total`.
- Symbiont-equipped units preserve their distinct active and inactive statlines. The active/inactive profiles are one logical trooper, not separate roster selections.
- **Jaan Staar and Kiiutan Imposters share AVA 1:** Army explicitly prohibits taking both in the same Army List.

## Faction summary

| Field | Value |
|---|---|
| Faction | Tohaa |
| Army ID | 801 |
| Rules baseline | N5.3 + FAQ v0.1 |
| Standard roster entries | 40 |
| Optional-mode entries | Hatail Spec-Ops; Tohaa Team-Ops |
| Reinforcement roster | Army ID `899` |
| Core Fireteams | 0 |
| Haris / Triad Fireteams | Unlimited; Army raw sentinel `256` |
| Duo Fireteams | Up to 2 |
| Fireteam families | Triad; Reex Escorts; Chaksa |

## Fireteam chart limits and faction-level restrictions

| Constraint | Current source value / normalized meaning |
|---|---|
| Core | `0` — no Core Fireteams |
| Haris | raw `256` — Army's special/unlimited value for Tohaa's Triad/Haris access |
| Duo | `2` |
| Main/Reinforcement mixing | Reinforcement roster ID `899` remains separate; do not merge charts unless a source exception says otherwise |
| Wildcards | No separate Wildcard list is exposed by the current Tohaa chart |
| Optional Spec-Ops | Hatail may appear in the general Triad chart only when Spec-Ops mode is enabled |

Current Army models the historical Tohaa **Triad** concept through chart entries whose allowed types are `DUO` and `HARIS`. Preserve those exact types when checking legality; do not import older-edition Triad composition rules over the N5.3 chart.

## Standard roster index

| Unit | Unit ID | AVA | Type | Regularity | Primary hooks |
|---|---:|---:|---|---|---|
| Kamael Light Infantry | 646 | Total | LI | Regular | cheap orders, Lt, Hacker, FO, Commlink, Triad |
| Wardrivers | 265 | 1 | LI | Regular | Hacker, Cybermine, Disco Baller |
| Makaul Troops | 653 | 6 | WB | Regular + Impetuous | Eclipse, CC, templates, Triad |
| Gao-Tarsos Unit | 649 | 3 | MI | Regular | Combat Jump/Parachutist, attack, Paramedic |
| Jaan Staar | 1554 | 1* | SK | Regular | Impersonation, enemy-DZ attack; shared AVA with Kiiutan |
| Sakiel Regiment | 647 | 6 | LI | Regular | Symbiont, Lt, FO, Paramedic, Triad |
| Greif Operators | 1298 | 1 | SK | Regular | infiltration/IMP-2 options, Mimetism, MSV1 |
| Kaeltar Specialists | 719 | 2 | LI | Regular | SymbioMate/Bomb, Chain of Command, Triad |
| Igao Unit | 707 | 2 | SK | Regular + Frenzy | Camo/Infiltration CC attacker |
| Cube Jäger | 956 | 1 | LI | Irregular | Parachutist/Paramedic, Monofilament |
| Kiel-Saan | 1305 | 2 | HI | Regular | heavy CC/attack; Reex + Chaksa teams |
| Reex Escorts | 1308 | 2 | LI | Regular | cheap gunfighters; Reex team anchor |
| Gorgos Squad | 1559 | 1 | TAG | Regular | Tactical Awareness TAG, optional Chaksa peripheral |
| Sukeul Commandos | 790 | 4 | LI | Regular | Mimetism, heavy weapons, FO/Lt, Triad |
| Rasail Boarding Team | 1552 | 4 | MI | Regular | 3W active profile, Nanoscreen, Chaksa peripheral, Lt |
| Chaksa Servants | 656 | 4 | LI Peripheral | — | Servant support |
| Motorized Bounty Hunters | 1565 | 1 | LI | Irregular + Impetuous | very fast disposable attack |
| Kotail Mobile Unit | 661 | 4 | LI | Regular | Holomask/Projector, Super-Jump, FO |
| Kerail Preceptors | 1553 | 2 | LI | Regular | Smoke, fast SymbioBeasts |
| Gao-Rael Unit | 648 | 4 | MI | Regular | MSV2 sniper/Spitfire, Triad |
| Kiiutan Imposters | 1309 | 1* | SK | Regular | IMP-2, attack; shared AVA with Jaan Staar |
| Nikoul Ambush Unit | 660 | 2 | LI | Regular | Sapper, MSV1, Viral Sniper, Minelayer |
| Chaksa Auxiliars | 655 | 4 | LI | Regular | HMG/HRL ARO; FTO Baggage/Sensor |
| Freelance Operator Samsa | 1683 | 1 | MI | Regular | Infiltration, Mimetism, Decoy, specialist |
| Chaksa Longarms | 1310 | 4 | MI | Regular | Autocannon/ML/Mk12, Chaksa team anchor |
| Clipsos Infiltrators | 652 | 3 | SK | Regular | Hidden Deployment, Mimetism -6, FO/Minelayer |
| Hatail Aelis Keesan | 659 | 1 | MI | Regular | KHD, Sensor, Triangulated Fire, Triad |
| Kosuil Assault Pioneers | 746 | 2 | MI | Regular | Engineer, mines, K1, Triad |
| Taagma Schemers | 1304 | 1 | LI | Regular | Holomask, Counterintelligence, MSV2 sniper, Triad |
| Kriigel Agents | 1307 | 2 | LI | Regular | Pheroware, Mirrorball, Triad/Reex |
| Ectros Regiment | 650 | 4 | HI | Regular | Symbiont HI, Lt/NCO, Triad |
| Ioann Bann | 1940 | 1 | WB | Irregular | Dog-Warrior, Smoke, close assault, Triad |
| Kumotail Bioengineers | 654 | 2 | LI | Regular | Doctor + Engineer, Triad |
| Kaauri Sentinels | 791 | 4 | LI | Regular | MSV1, Sixth Sense, mines/Mirrorball |
| Libertos Freedom Fighters | 1275 | 1 | LI | Irregular | Camo, Dogged, FD, Minelayer option |
| Draal Saboteurs | 1306 | 2 | SK | Regular | Mimetism -6, FD, Dazer/mines, specialist, Triad |
| Tohaa Diplomatic Delegates | 658 | 1 | LI | Irregular | 5-point specialist/Journalist |
| Neema Saatar | 657 | 1 | HI | Regular + Frenzy | elite Lt, +1 Order/Command Token options, Triad |
| Taqeul Officers | 801 | 2 | MI | Regular | CoC or premium Lt, Pheroware, Triad |
| Armand “Le Muet” | 680 | 1 | MI | Regular | Mimetism -6 sniper, Minelayer/MSV1 |

`1*` = Jaan Staar and Kiiutan share one combined AVA slot; they cannot coexist in the same Army List.

## Unit details

### Kamael Light Infantry

**ID 646 · AVA Total · LI** — `MOV 10-10 | CC 13 | BS 11 | PH 11 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 12 | 0 | Combi Rifle, Pistol, CCW |
| 2 | 18 | 1 | Spitfire, Pistol, CCW |
| 4 | 16 | 0.5 | Sniper Rifle, Pistol, CCW |
| 5 | 17 | 0.5 | Combi Rifle; **Hacking Device** |
| 6 | 13 | 0 | Combi Rifle, Flash Pulse; **Forward Observer**, Deployable Repeater |
| 7 | 14 | 0 | Combi Rifle; **Paramedic**, MediKit |
| 8 | 12 | 0 | Combi Rifle; **Lieutenant** |
| 10 | 14 | 0 | Combi Rifle; **Commlink**, Specialist Operative |

Fireteam: general Triad family, max 3.

### Wardrivers, Mercenary Hackers

**ID 265 · AVA 1 · LI** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 2`. Sixth Sense.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 14 | 1 | Boarding Shotgun, Flash Pulse, Cybermine, Pistol, CCW; **Hacking Device** with source upgrade package |
| 2 | 16 | 1 | As above + **Disco Baller** |

### Makaul Troops

**ID 653 · AVA 6 · WB** — `MOV 10-10 | CC 23 | BS 11 | PH 13 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Martial Arts L2, CC Attack modifier, Courage, Dodge bonus, Impetuous, No Cover.

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 14 | 0 | Heavy Flamethrower, Contender, Eclipse Grenades, Pistol, Viral CCW |
| 2 | 14 | 0 | Heavy Flamethrower, Contender, Eclipse Grenades, Pistol, DA CCW |
| 3 | 15 | 0 | Vulkan Shotgun, Pulzar, Eclipse Grenades, Pistol, Viral CCW |
| 4 | 15 | 0 | Combi Rifle, Eclipse Grenades, Pistol, Viral CCW |

Fireteam: general Triad family, max 3.

### Gao-Tarsos Unit

**ID 649 · AVA 3 · MI** — active `MOV 10-10 | CC 17 | BS 12 | PH 12 | WIP 13 | ARM 3 | BTS 0 | W 2 | S 2`; inactive Symbiont profile lowers PH/ARM while retaining the source's two-wound profile. Parachutist, Combat Jump, Super-Jump/jet-propulsion package, Transmutation.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 31 | 1.5 | Spitfire |
| 2 | 22 | 0 | Boarding Shotgun, D-Charges |
| 3 | 24 | 0 | Boarding Shotgun, D-Charges; **Paramedic** |

### Jaan Staar, Kiiutan Imposter

**ID 1554 · AVA 1 shared · SK** — active `MOV 10-10 | CC 22 | BS 12 | PH 11 | WIP 13 | ARM 2 | BTS 6 | W 2 | S 2`. Impersonation (IMP-2) package and close-range assassination tools.

| Pts | SWC | Loadout |
|---:|---:|---|
| 30 | 1 | Light Shotgun, Shock Mine, Viral Pistol (+1B), Viral CCW |

**Roster relation:** cannot be selected in the same Army List as a Kiiutan Imposter.

### Sakiel Regiment

**ID 647 · AVA 6 · LI** — active `MOV 10-10 | CC 18 | BS 12 | PH 11 | WIP 13 | ARM 2 | BTS 0 | W 2 | S 2`. Courage, Frenzy, Transmutation/Symbiont profile.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 19 | 0 | Viral Combi Rifle, E/M Grenades |
| 2 | 22 | 1.5 | Spitfire |
| 3 | 21 | 0 | Viral Combi Rifle, E/M Grenades; **Paramedic** |
| 4 | 19 | 0 | Viral Combi Rifle, E/M Grenades; **Lieutenant** |
| 5 | 20 | 0 | Viral Combi Rifle, E/M Grenades, Flash Pulse, D-Charges; **Forward Observer** |

Fireteam: general Triad family, max 3.

### Greif Operators

**ID 1298 · AVA 1 · SK** — `MOV 10-10 | CC 17 | BS 11 | PH 11 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. MSV1, Courage, Stealth; profile-specific infiltration/impersonation package.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 23 | 0 | Combi Rifle, D-Charges, Breaker Pistol, Viral Mine; FD +20, Mimetism -6 |
| 2 | 25 | 0 | Shock Marksman Rifle, D-Charges, Breaker Pistol; FD +20, Mimetism -6 |
| 3 | 21 | 0.5 | Breaker Combi Rifle, D-Charges, Silenced Pistol, CCW; Surprise Attack, IMP-2 |

### Kaeltar Specialists

**ID 719 · AVA 2 · LI** — `MOV 10-10 | CC 14 | BS 11 | PH 11 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 15 | 0 | Light Shotgun, Flash Pulse, SymbioBomb, Pistol, PARA CCW; **1 SymbioMate** |
| 3 | 21 | 0.5 | Same base package; **Chain of Command**, 1 SymbioMate |
| 4 | 28 | 0.5 | Combi Rifle, Flash Pulse, Pistol, PARA CCW; **Chain of Command, 2 SymbioMates** |

Fireteam: general Triad family, max 2.

### Igao Unit

**ID 707 · AVA 2 · SK** — `MOV 10-10 | CC 23 | BS 11 | PH 13 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 2`. Martial Arts L3, Camouflage, Infiltration, Mimetism -3, Stealth, Terrain (Total), Frenzy.

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 23 | 0 | Vulkan Shotgun, Nanopulser, Pistol, DA CCW |
| 2 | 25 | 0 | Combi Rifle, Nanopulser, Pistol, DA CCW |
| 3 | 26 | 0.5 | Combi Rifle, Nanopulser, **Pheroware Tactic: Mirrorball**, Pistol, DA CCW |

### Cube Jäger

**ID 956 · AVA 1 · LI · Irregular** — airborne specialist/medic with Parachutist and Monofilament CCW.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 15 | 0 | Boarding Shotgun, Pistol, Monofilament CCW; **Paramedic** |
| 2 | 18 | 0 | SMG, E/Mitter, Pistol, Monofilament CCW; **Paramedic** |

### Kiel-Saan Covert Assault Unit

**ID 1305 · AVA 2 · HI** — active `MOV 15-5 | CC 21 | BS 13 | PH 14 | WIP 12 | ARM 4 | BTS 6 | W 3 | S 5`; separate inactive Symbiont profile. Martial Arts L2, Berserk, Natural Born Warrior, MetaChemistry, Stealth, Transmutation, Warhorse.

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 49 | 1.5 | Red Fury, E/M Carbine, Heavy Pistol, DA CCW |
| 2 | 49 | 0 | Mk12, E/M Carbine, Heavy Pistol, DA CCW |

Fireteams: Reex Escorts 0–1; Chaksa 0–1.

### Reex Escorts

**ID 1308 · AVA 2 · LI** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | STR 1 | S 1`.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 12 | 0 | Boarding Shotgun, Contender, Pistol, PARA CCW |
| 2 | 12 | 0 | Thunderbolt (+1B), Pistol, PARA CCW |
| 3 | 16 | 0 | K1 Marksman Rifle, Pistol, PARA CCW; BS Attack (Shock) |

Fireteam: Reex Escorts; **1–2 Reex are required/source anchors**.

### Gorgos Squad

**ID 1559 · AVA 1 · TAG** — active `MOV 15-10 | CC 19 | BS 14 | PH 16 | WIP 13 | ARM 7 | BTS 9 | W 4 | S 7`, with inactive Symbiont profile. ECM: Guided, Tactical Awareness and source TAG/Symbiont package.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 63 | 1.5 | AP HMG, Flammenspeer, Pulzar, Heavy Pistol, Viral CCW |
| 2 | 70 | 1.5 | Same Gorgos + Chaksa peripheral with Light Shotgun/E/M Grenades |
| 3 | 67 | 1.5 | Same Gorgos + cheaper Chaksa peripheral with Pulzar/E/M Grenades |

Bundled Chaksa profiles are peripherals and are not independent roster entries.

### Sukeul Commandos

**ID 790 · AVA 4 · LI** — active `MOV 10-10 | CC 17 | BS 13 | PH 11 | WIP 13 | ARM 2 | BTS 3 | W 2 | S 2`. Mimetism -3, Stealth, Terrain (Total), Warhorse, Transmutation/Symbiont profile.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 29 | 0 | K1 Combi Rifle, Flash Pulse, D-Charges; **Forward Observer**, Deployable Repeater |
| 2 | 33 | 1.5 | HMG |
| 3 | 28 | 1 | K1 Sniper Rifle |
| 4 | 34 | 1.5 | Missile Launcher, Light Shotgun |
| 5 | 29 | 0 | K1 Combi/FO package; **Lieutenant** |

Fireteam: general Triad family, max 3.

### Rasail Boarding Team

**ID 1552 · AVA 4 · MI** — active `MOV 10-10 | CC 17 | BS 12 | PH 11 | WIP 13 | ARM 1 | BTS 3 | W 3 | S 2`; inactive Symbiont profile. Nanoscreen/No Cover package. Each selectable profile includes its source Chaksa peripheral.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 31 | 0 | Viral Combi Rifle |
| 2 | 27 | 0 | Boarding Shotgun, Shock Mine |
| 3 | 29 | 0 | Light Shotgun, Contender |
| 4 | 34 | 1.5 | Spitfire |
| 5 | 31 | 0 | Viral Combi Rifle; **Lieutenant** |
| 6 | 34 | 1.5 | Spitfire; **Lieutenant** |

### Chaksa Servants

**ID 656 · AVA 4 · LI Peripheral** — Servant support trooper.

| Pts | SWC | Loadout |
|---:|---:|---|
| 3 | 0 | PARA CCW; Peripheral (Servant) |

### Motorized Bounty Hunters

**ID 1565 · AVA 1 · LI · Irregular + Impetuous** — `MOV 20-15 | CC 17 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 4`. Motorcycle, Booty, Limited Cover, Mimetism -3.

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 8 | 0 | Boarding Shotgun, Heavy Riotstopper, Pistol, PARA CCW |
| 2 | 9 | 0 | SMG, Chain-colt, Pistol, PARA CCW |
| 3 | 16 | 0.5 | Red Fury, Breaker Pistol, PARA CCW |

### Kotail Mobile Unit

**ID 661 · AVA 4 · LI** — active `MOV 15-10 | CC 18 | BS 12 | PH 12 | WIP 13 | ARM 2 | BTS 3 | W 2 | S 2`. Holomask, Holoprojector, Surprise Attack, Super-Jump and Transmutation.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 30 | 0 | Combi Rifle, E/M Grenades |
| 2 | 31 | 0 | Combi Rifle (+1B) |
| 3 | 35 | 1 | Spitfire |
| 4 | 32 | 0 | Combi Rifle, E/M Grenades, Flash Pulse; **Forward Observer**, Deployable Repeater |

### Kerail Preceptors

**ID 1553 · AVA 2 · LI** — fast Symbiont trooper with Smoke and bundled SymbioBeast choices.

| Profile ID | Pts | SWC | Loadout / composition |
|---:|---:|---:|---|
| 1 | 25 | 0 | SMG, Smoke Grenades, Kobra Pistol, CCW + **1 Surda SymbioBeast** |
| 2 | 33 | 0 | Same controller + **2 Surda SymbioBeasts** |
| 3 | 30 | 0 | Same controller + **1 Mutan SymbioBeast** |

Surda/Mutan are bundled peripherals; their disabled standalone source rows do not create independent roster options.

### Gao-Rael Unit

**ID 648 · AVA 4 · MI** — active `MOV 10-10 | CC 19 | BS 12 | PH 12 | WIP 14 | ARM 2 | BTS 3 | W 2 | S 2`. **MSV2** and Symbiont/Transmutation profile.

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 29 | 1 | Sniper Rifle, Shock Mine |
| 2 | 30 | 1.5 | Spitfire |

Fireteam: general Triad family, max 3.

### Kiiutan Imposters

**ID 1309 · AVA 1 shared · SK** — active `MOV 10-10 | CC 17 | BS 12 | PH 11 | WIP 13 | ARM 2 | BTS 6 | W 2 | S 2`; inactive Symbiont profile `ARM 0/BTS 0/PH 10`. Surprise Attack, Stealth, IMP-2 source package.

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 4862 | 29 | 0.5 | Combi Rifle, Zapper, Viral Pistol, CCW |
| 5100 | 27 | 0.5 | SMG, E/Mitter, Viral Pistol, CCW |

**Roster relation:** AVA 1 is shared with Jaan Staar; the two cannot coexist.

### Nikoul Ambush Unit

**ID 660 · AVA 2 · LI** — active Symbiont profile with **MSV1, Sapper** and long-range Viral weaponry.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 25 | 1.5 | Viral Sniper Rifle |
| 2 | 27 | 1.5 | Viral Sniper Rifle, Shock Mine; **Minelayer** |

### Chaksa Auxiliars

**ID 655 · AVA 4 · LI** — `MOV 10-10 | CC 19 | BS 11 | PH 12 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 24 | 1 | HMG; 360º Visor, Neurocinetics |
| 2 | 15 | 1 | Heavy Rocket Launcher, Light Shotgun; source Guided BS Attack package |
| 3 | 10 | 0 | **FTO** Heavy Flamethrower; **Baggage, Sensor** |

Only the FTO profile is eligible for the Chaksa Fireteam row; max 2.

### Freelance Operator Samsa

**ID 1683 · AVA 1 · MI** — `MOV 15-5 | CC 15 | BS 13 | PH 11 | WIP 13 | ARM 3 | BTS 0 | W 1 | S 2`. Infiltration, Mimetism -3, Decoy, Specialist Operative, Super-Jump and source Exrah package.

| Pts | SWC | Loadout |
|---:|---:|---|
| 26 | 0 | Plasma Rifle, D-Charges, Pistol, CCW |

### Chaksa Longarms

**ID 1310 · AVA 4 · MI** — `MOV 10-10 | CC 17 | BS 12 | PH 12 | WIP 12 | ARM 3 | BTS 3 | W 1 | S 2`. Sixth Sense/Religious/Terrain and source defensive modifiers.

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 21 | 0 | Combi Rifle, Pulzar (+1B), E/M Grenades |
| 2 | 29 | 1.5 | Portable Autocannon, Pulzar |
| 3 | 24 | 1.5 | Missile Launcher, Pulzar |
| 4 | 25 | 0 | Mk12, Pulzar, AP Mine |

Fireteam: Chaksa family; **1–3 Longarms are the source anchor**.

### Clipsos Infiltrators

**ID 652 · AVA 3 · SK** — `MOV 10-10 | CC 14 | BS 12 | PH 12 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 2`. Camouflage, Hidden Deployment, Infiltration, Mimetism -6, Stealth.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 25 | 0 | Combi Rifle, Shock Mine |
| 2 | 22 | 0 | Boarding Shotgun, Shock Mine |
| 3 | 24 | 1 | Sniper Rifle |
| 4 | 23 | 0.5 | Boarding Shotgun, Shock Mine; **Minelayer** |
| 5 | 26 | 0 | Combi Rifle, Flash Pulse, Shock Mine; **Forward Observer** |

### Hatail Aelis Keesan

**ID 659 · AVA 1 · MI** — `MOV 10-10 | CC 15 | BS 12 | PH 12 | WIP 14 | ARM 2 | BTS 3 | W 1 | S 2`. Killer Hacking Device, Sensor, Triangulated Fire, Regeneration.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 25 | 0 | AP Rifle, E/M Carbine, Nanopulser, Flash Pulse, D-Charges; **KHD** |
| 2 | 25 | 0 | K1 Combi Rifle, Nanopulser, Flash Pulse, D-Charges; **KHD** |

Fireteam: general Triad family, max 1.

### Kosuil Assault Pioneers

**ID 746 · AVA 2 · MI** — active Symbiont profile; Engineer-capable combat specialist with K1 weapons, mines and D-Charges.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 25 | 0 | K1 Combi Rifle, D-Charges, AP Mine; **Engineer**, GizmoKit |
| 2 | 20 | 0 | Boarding Shotgun, Panzerfaust, D-Charges; **Engineer**, GizmoKit |
| 3 | 22 | 0 | K1 Combi Rifle, D-Charges, Shock Mine; **Minelayer** |

Fireteam: general Triad family, max 2.

### Taagma Schemers

**ID 1304 · AVA 1 · LI** — `MOV 10-10 | CC 15 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Holomask, Counterintelligence, Immunity (Shock), Stealth.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 15 | 0 | Breaker Combi Rifle, Nanopulser, Pistol, CCW |
| 2 | 22 | 1.5 | Viral Sniper Rifle, Pistol, CCW; **MSV2** |

Fireteam: general Triad family, max 1.

### Kriigel Agents

**ID 1307 · AVA 2 · LI** — `MOV 10-10 | CC 14 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Courage, Sixth Sense.

| Pts | SWC | Loadout |
|---:|---:|---|
| 21 | 0.5 | Breaker Combi Rifle, Grenade Launcher, **Pheroware Tactic: Eraser**, **Pheroware Tactic: Mirrorball**, Viral Pistol, CCW |

Fireteams: general Triad max 1; Reex Escorts max 1 and counts as the chart's `(Reex)` entry.

### Ectros Regiment

**ID 650 · AVA 4 · HI** — active `MOV 15-5 | CC 19 | BS 13 | PH 14 | WIP 13 | ARM 3 | BTS 6 | W 3 | S 2`; inactive Symbiont profile. Courage, Dodge bonus, Transmutation.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 33 | 0 | Viral Combi Rifle, Pulzar, Pistol, Shock CCW |
| 2 | 39 | 1.5 | HMG, Pulzar, Pistol, Shock CCW |
| 3 | 32 | 0 | Vulkan Shotgun (+1B), Pulzar, Pistol, Shock CCW |
| 4 | 33 | 0 | Viral Combi Rifle package; **Lieutenant** |
| 5 | 41 | 1.5 | HMG package; **NCO** |

Fireteam: general Triad family, max 3.

### Ioann Bann, Varangian Dog-Warrior

**ID 1940 · AVA 1 · WB · Irregular** — Dogface `MOV 15-10 | CC 22 | BS 11 | PH 14 | WIP 13 | ARM 2 | BTS 3 | W 3`; Dog-Warrior `MOV 15-10 | CC 23 | PH 16 | ARM 4 | BTS 6 | W 3`. Transforms under the source Dog-Warrior package.

| Pts | SWC | Loadout |
|---:|---:|---|
| 32 | 0 | Chain Rifle (+1B), Viral Tactical Bow (+1SD), Smoke Grenades, AP Heavy Pistol (+1B), AP+T2 CCW |

Fireteam: general Triad family, max 1.

### Kumotail Bioengineers

**ID 654 · AVA 2 · LI** — `MOV 10-10 | CC 14 | BS 11 | PH 11 | WIP 14 | ARM 1 | BTS 0 | W 1 | S 2`. **Doctor + Engineer**, MediKit/GizmoKit support.

| Pts | SWC | Loadout |
|---:|---:|---|
| 21 | 0 | Combi Rifle, D-Charges, Pistol, CCW |

Fireteam: general Triad family, max 2.

### Kaauri Sentinels

**ID 791 · AVA 4 · LI** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | STR 1 | S 1`. Biometric Visor, MSV1, Sixth Sense, Discover bonus.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 11 | 0 | SMG, Nanopulser (+1B), E/M Mine; **Minelayer** |
| 2 | 11 | 0 | Vulkan Shotgun, E/M Mine |
| 3 | 17 | 0.5 | Sniper Rifle, E/M Mine |
| 4 | 14 | 0.5 | Combi Rifle, E/M Mine, **Pheroware Tactic: Mirrorball** |

### Libertos Freedom Fighters

**ID 1275 · AVA 1 · LI · Irregular** — `MOV 10-10 | CC 16 | BS 11 | PH 11 | WIP 12 | ARM 0 | BTS 0 | W 1 | S 2`. Camouflage (limited), Courage, Forward Deployment +20, Dogged, Frenzy, aquatic Terrain.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 8 | 0 | SMG, Chain-colt, Pistol, CCW |
| 4 | 8 | 1 | Light Shotgun, Shock Mine, Pistol, CCW; **Minelayer** |

### Draal Saboteurs

**ID 1306 · AVA 2 · SK** — active `MOV 15-5 | CC 16 | BS 13 | PH 12 | WIP 13 | ARM 2 | BTS 6 | W 2 | S 2`. Forward Deployment +20, Mimetism -6, Specialist Operative, Stealth, Transmutation.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 32 | 0 | SMG, Pulzar, D-Charges, Viral Pistol, CCW; **Dazer** |
| 2 | 33 | 0 | SMG, Pulzar, D-Charges, Viral Pistol, Viral Mine |
| 3 | 33 | 1 | SMG, Pulzar, D-Charges, Viral Pistol, Shock Mine; **Minelayer** |
| 4 | 38 | 1 | AP Marksman Rifle, D-Charges, Viral Pistol, Shock Mine; **Minelayer** |

Fireteam: general Triad family, max 1.

### Tohaa Diplomatic Delegates

**ID 658 · AVA 1 · LI · Irregular** — `MOV 10-10 | CC 12 | BS 10 | PH 10 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. CC Attack modifier.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 2 | 5 | 0 | Nanopulser, Flash Pulse, Pheroware Tactic: Eraser, Pistol, CCW; **Specialist Operative** |
| 3 | 5 | 0 | Same weapons; **Journalist (+3)** |

### Neema Saatar

**ID 657 · AVA 1 · HI** — active `MOV 15-5 | CC 22 | BS 13 | PH 14 | WIP 15 | ARM 3 | BTS 9 | W 3 | S 2`. Martial Arts L2, Courage, Dodge bonus, Frenzy, Stealth; inactive Symbiont profile retained by source.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 32 | 0 | Breaker Combi Rifle, Panzerfaust, Nanopulser, Viral Pistol, Viral CCW |
| 2 | 37 | 1.5 | AP Spitfire, Nanopulser, Viral Pistol, Shock CCW |
| 3 | 36 | **+1** | Breaker/Panzerfaust package; **Lieutenant (+1 Order)** |
| 4 | 41 | 0.5 | AP Spitfire package; **Lieutenant (+1 Command Token)** |

Fireteam: general Triad family, max 1.

### Taqeul Officers

**ID 801 · AVA 2 · MI** — active `MOV 10-10 | CC 14 | BS 13 | PH 11 | WIP 14 | ARM 3 | BTS 6 | W 2 | S 2`. Courage, Regeneration, Symbiont/Transmutation profile.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 36 | 0 | Viral Combi Rifle, Nanopulser, Pheroware Tactic: Endgame, Pheroware Tactic: Mirrorball, Pistol, CCW; **Chain of Command** |
| 2 | 35 | 0 | Same package; **Lieutenant (+1 Order)** |
| 3 | 35 | 0 | Same package; **Lieutenant (+1 Command Token)** |

Fireteam: general Triad family, max 2.

### Armand “Le Muet”, Freelance Killer

**ID 680 · AVA 1 · MI** — active `MOV 10-10 | CC 21 | BS 13 | PH 12 | WIP 13 | ARM 2 | BTS 3 | W 2 | S 2`; inactive Symbiont profile. Forward Deployment, Natural Born Warrior, Mimetism -6, Stealth.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 33 | 1.5 | MULTI Sniper Rifle, Nanopulser, Shock Mine, Breaker Pistol, Viral CCW; **Minelayer** |
| 2 | 34 | 1.5 | MULTI Sniper Rifle, Nanopulser, Breaker Pistol, Viral CCW; **MSV1** |

## Lieutenant and order-control index

| Unit/profile | Function |
|---|---|
| Kamael | cheap Lieutenant, 12/0 |
| Sakiel | Lieutenant, 19/0 |
| Sukeul | Lieutenant on K1 Combi/FO chassis, 29/0 |
| Rasail | Lieutenant on Viral Combi 31/0 or Spitfire 34/1.5 |
| Ectros | Lieutenant 33/0; HMG **NCO** 41/1.5 |
| Neema Saatar | Lieutenant +1 Order with **+1 SWC**, or Lieutenant +1 Command Token at 0.5 SWC |
| Taqeul | Lieutenant +1 Order or Lieutenant +1 Command Token, both 35/0 |
| Kaeltar | Chain of Command profiles at 21/0.5 and 28/0.5 |
| Taqeul | Chain of Command profile 36/0 |
| Taagma | Counterintelligence on the unit chassis |

## Hacking and network index

### Hackers

- **Kamael:** Hacking Device, 17/0.5.
- **Wardriver:** Hacking Device with its source upgrade package, 14/1 or 16/1 with Disco Baller.
- **Aelis Keesan:** Killer Hacking Device on both current profiles.

### Repeater / projection pieces

- Kamael Forward Observer: Deployable Repeater.
- Sukeul Forward Observer: Deployable Repeater.
- Wardriver: Cybermine; one option adds Disco Baller.
- Aelis: Sensor + KHD gives a capable anti-hacker/tech-counter node once projected coverage exists.

Tohaa's network is substantially smaller than REM-heavy factions; do not assume generic Repeater bots that are not present in the faction roster.

## Deployment / marker-state index

- **Impersonation / enemy-DZ pressure:** Jaan Staar; Kiiutan; one Greif option.
- **Combat Jump / Parachutist:** Gao-Tarsos; Cube Jäger uses airborne deployment appropriate to its source profile.
- **Hidden Deployment:** Clipsos.
- **Camouflage / midfield:** Clipsos, Igao, Libertos; Draal/Greif use their respective source marker/deployment packages.
- **Forward Deployment / infiltration:** Greif, Igao, Samsa, Draal, Libertos, Armand and other profile-specific entries above.
- **Holomask / Holoprojector:** Kotail; Taagma has Holomask.

## Vision-control index

- **Eclipse:** Makaul.
- **Smoke:** Kerail Preceptors; Ioann Bann.
- **Pheroware Tactic: Mirrorball:** Kriigel; Taqeul; Kaauri profile; Igao profile.
- **MSV2:** Gao-Rael; Taagma Viral Sniper.
- **MSV1:** Greif; Nikoul; Kaauri; Armand MSV profile.

## Canonical Fireteam definitions

The current Tohaa chart exposes **no Core**, **unlimited Haris/Triad access** (raw source value `256`) and **up to two Duos**. The following member tables are authoritative for this file.

### FT-01 — Triad Fireteams

**Types:** Duo, Haris  
**Wildcard team:** no separate Wildcard model  
**Observation:** current Army labels this family `Triad Fireteams`. None of the rows carries a `required: true` flag; legal team size/type still applies.

| Member | Unit ID | Required | Min | Max | Counts as / source comment | Profile restriction |
|---|---:|---|---:|---:|---|---|
| Kamael | 646 | no | 0 | 3 | Triad | all |
| Sakiel | 647 | no | 0 | 3 | Triad | all |
| Gao-Rael | 648 | no | 0 | 3 | Triad | all |
| Ectros | 650 | no | 0 | 3 | Triad | all |
| Makaul | 653 | no | 0 | 3 | Triad | all |
| Kumotail | 654 | no | 0 | 2 | Triad | all |
| Neema Saatar | 657 | no | 0 | 1 | Triad | all |
| Aelis Keesan | 659 | no | 0 | 1 | Triad | all |
| Kaeltar | 719 | no | 0 | 2 | Triad | all |
| Kosuil | 746 | no | 0 | 2 | Triad | all |
| Sukeul | 790 | no | 0 | 3 | Triad | all |
| Taqeul | 801 | no | 0 | 2 | Triad | all |
| Taagma | 1304 | no | 0 | 1 | — | all |
| Draal | 1306 | no | 0 | 1 | — | all |
| Kriigel | 1307 | no | 0 | 1 | Triad | all |
| Hatail Spec-Ops | 1908 | no | 0 | 1 | Spec-Ops | optional mode only |
| Ioann Bann | 1940 | no | 0 | 1 | Triad | all |

### FT-02 — Reex Escorts Fireteams

**Types:** Duo, Haris  
**Wildcard team:** no

| Member | Unit ID | Required | Min | Max | Counts as / source comment | Profile restriction |
|---|---:|---|---:|---:|---|---|
| Reex Escorts | 1308 | **yes by min** | **1** | 2 | Reex | all |
| Kriigel Agent | 1307 | no | 0 | 1 | Reex | all |
| Kiel-Saan | 1305 | no | 0 | 1 | — | all |

### FT-03 — Chaksa Fireteams

**Types:** Duo, Haris  
**Wildcard team:** no

| Member | Unit ID | Required | Min | Max | Counts as / source comment | Profile restriction |
|---|---:|---|---:|---:|---|---|
| Chaksa Longarms | 1310 | **yes by min** | **1** | 3 | Chaksa | all |
| Chaksa Auxiliar | 655 | no | 0 | 2 | Chaksa | **FTO profile only** |
| Kiel-Saan | 1305 | no | 0 | 1 | — | all |

### Wildcards

The current source does **not** expose a separate Tohaa Wildcard list. Do not infer Wildcard access from older Tohaa/Spiral charts.

## Unit → Fireteam access index

| Unit | Fireteam | Type | Access | Profile restriction | Min–max | Notes |
|---|---|---|---|---|---|---|
| Kamael | FT-01 Triad | Duo/Haris | native | all | 0–3 | Triad |
| Sakiel | FT-01 Triad | Duo/Haris | native | all | 0–3 | Triad |
| Gao-Rael | FT-01 Triad | Duo/Haris | native | all | 0–3 | Triad |
| Ectros | FT-01 Triad | Duo/Haris | native | all | 0–3 | Triad |
| Makaul | FT-01 Triad | Duo/Haris | native | all | 0–3 | Triad |
| Kumotail | FT-01 Triad | Duo/Haris | native | all | 0–2 | Triad |
| Neema | FT-01 Triad | Duo/Haris | native | all | 0–1 | Triad |
| Aelis | FT-01 Triad | Duo/Haris | native | all | 0–1 | Triad |
| Kaeltar | FT-01 Triad | Duo/Haris | native | all | 0–2 | Triad |
| Kosuil | FT-01 Triad | Duo/Haris | native | all | 0–2 | Triad |
| Sukeul | FT-01 Triad | Duo/Haris | native | all | 0–3 | Triad |
| Taqeul | FT-01 Triad | Duo/Haris | native | all | 0–2 | Triad |
| Taagma | FT-01 Triad | Duo/Haris | native | all | 0–1 | — |
| Draal | FT-01 Triad | Duo/Haris | native | all | 0–1 | — |
| Kriigel | FT-01 Triad | Duo/Haris | native | all | 0–1 | also Reex access |
| Hatail Spec-Ops | FT-01 Triad | Duo/Haris | special | optional mode | 0–1 | Spec-Ops only |
| Ioann Bann | FT-01 Triad | Duo/Haris | native | all | 0–1 | Triad |
| Reex | FT-02 Reex | Duo/Haris | required | all | 1–2 | source anchor |
| Kriigel | FT-02 Reex | Duo/Haris | counts-as | all | 0–1 | source `(Reex)` comment |
| Kiel-Saan | FT-02 Reex | Duo/Haris | native | all | 0–1 | — |
| Chaksa Longarm | FT-03 Chaksa | Duo/Haris | required | all | 1–3 | source anchor |
| Chaksa Auxiliar | FT-03 Chaksa | Duo/Haris | native | FTO only | 0–2 | source `(Chaksa)` comment |
| Kiel-Saan | FT-03 Chaksa | Duo/Haris | native | all | 0–1 | — |

If this reverse index ever conflicts with the canonical tables above, the canonical Fireteam definitions win.

## Optional-mode units

| Unit | ID | Mode | Normal Tohaa status |
|---|---:|---|---|
| Hatail Spec-Ops | 1908 | Spec-Ops | Optional mode only; may join FT-01 when enabled |
| Tohaa Team-Ops | 1909 | Team-Ops | Optional mode only |

Do not count these as ordinary matched-play roster entries unless the corresponding optional mode is explicitly enabled.

## Reinforcements boundary

Army links Tohaa to Reinforcement roster ID **899**. Reinforcement-only profiles and any Reinforcement Fireteam data remain separate from this base-faction reference. Do not infer Main/Reinforcement mixing.

## Derived tactical index

This section is analytical and non-authoritative; source profile data and Fireteam tables above take precedence.

| Block / tag | Strong Tohaa candidates |
|---|---|
| Long-range attack | Gorgos; Sukeul HMG/ML; Ectros HMG; Neema AP Spitfire; Gao-Rael Spitfire; Chaksa Longarm Autocannon |
| Long-range ARO | Gao-Rael Sniper; Nikoul Viral Sniper; Sukeul K1 Sniper/ML; Taagma Viral Sniper; Chaksa Longarm Autocannon/ML; Chaksa Aux HRL/HMG; Armand |
| Mid-range attack | Sukeul; Ectros; Neema; Kotail; Draal AP Marksman; Reex K1 Marksman |
| Close assault | Makaul; Igao; Kiel-Saan; Ioann Bann; Kerail/SymbioBeasts; Jaan Staar; Kiiutan |
| Specialist | Kamael FO/Paramedic/Commlink; Sakiel FO/Paramedic; Sukeul FO; Kumotail; Kosuil; Clipsos FO; Draal; Samsa; Diplomatic Delegate |
| DZ defense | Kaauri; Chaksa Auxiliars; Nikoul; Libertos; Taagma sniper |
| Midfield defense | Clipsos; Draal; Libertos; Igao; Kaauri; Greif |
| Midfield specialist | Clipsos FO; Draal; Samsa; Sukeul FO; Kotail FO |
| Warband / order-efficient assault | Makaul; Ioann Bann; Motorized Bounty Hunter |
| Airborne | Gao-Tarsos; Cube Jäger |
| Enemy-DZ attacker | Jaan Staar; Kiiutan; Greif IMP-2; Gao-Tarsos |
| Network projection | Kamael FO Deployable Repeater; Sukeul FO Deployable Repeater; Wardriver tools |
| Vision control | Makaul Eclipse; Kerail Smoke; Ioann Smoke; Kriigel/Taqeul/Kaauri/Igao Mirrorball |
| Hacker | Wardriver; Kamael |
| KHD | Aelis Keesan |
| Tech-counter | Aelis Sensor/KHD; Kosuil Engineer; Kumotail Doctor/Engineer; Kaauri MSV1/Sixth Sense |
| TAG support | Kumotail; Chaksa Servant support chain; Kaeltar defensive Symbio tools do not directly repair the TAG |

## Source-normalization and validation notes

- `AVA 255` on Kamael is rendered as **AVA Total**.
- Fireteam chart raw `HARIS: 256` is preserved semantically as Tohaa's **unlimited Haris/Triad allowance**, not a literal count of 256 teams.
- The chart itself labels its broad family `Triad Fireteams` but exposes the allowed types `DUO` and `HARIS`; this file keeps both facts.
- Jaan Staar and Kiiutan's source note is enforced as a shared AVA-one relationship.
- FTO is preserved where it affects chart legality: the **Chaksa Auxiliar FTO** profile is the eligible Chaksa-team entry.
- No Wildcard list is synthesized because none is exposed by the current Tohaa chart.
- Symbiont active/inactive source statlines are retained as profile groups under one logical roster entry.
- Disabled subordinate profiles (Chaksa peripherals, SymbioBeasts, inactive forms) are documented with their parent rather than counted as independent roster units.
- Generic `merc-*` catalogue objects with empty faction lists are excluded. Named entries explicitly listing faction `801` remain part of the standard roster.
- Standard-roster count excludes Hatail Spec-Ops and Tohaa Team-Ops: **40 ordinary entries + 2 optional-mode entries**.

## Provenance

- Corvus Belli Army-derived source revision: `7.26246.159`
- Source commit: `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b` (`army: N5.3 + ITS18`)
- Army data changed on: 2026-09-03
- Source dataset: `n5/tohaa/tohaa.json` / `n5/tohaa/7.26246.159.json`
- InfinityDB commit: `4e2662be3f43387fbae42b3790a711b3e98570c4`
- Rules baseline: N5.3 + N5 FAQ v0.1
- Generated / verified: 2026-10-15
