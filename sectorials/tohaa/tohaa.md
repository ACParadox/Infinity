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

**Tactical companion:** [Tohaa — N5.3 list-building, video/podcast transcript analysis and TAG/Chaksa/Kaauri/Reex roles](../../notes/factions/tohaa.md). This is community-derived analysis; the structured roster and Fireteam charts here remain authoritative.

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

## Command-unit apex/value cross-reference (2026-10-23)

**Kaeltar CoC 21/0.5 with one SymbioMate or 28/0.5 with two** has outstanding marginal command value because it buys *both* protected succession and meaningful protection of key fighters. **Taqeul LT(+1) 35/0** provides two personal LT Orders/mission control; **Neema LT(+1) 36/+1 SWC** unlocks SWC-heavy attack options. Choose **Taqeul36/0 CoC** only when its Pheroware/weapon role justifies extra cost over Kaeltar. Do not treat the two SymbioMates as free on a cheaper loadout.

See [cross-game Lieutenant, Chain of Command and Order-package tiers](../../notes/list-building/command-units-apex-and-value.md). **Use this roster/Fireteam chart above for exact legality.**

## Mission specialist / button-pusher selections (N5.3)

**Sukeul FO29/0** is 2W Symbiont, K1 gun, Warhorse and Deployable Repeater in legal Triad; excellent durable late carrier versus a **Clipsos FO26/0** Hidden/Infiltrating opener. **Kaeltar CoC21/.5 (1 SymbioMate) or 28/.5 (2)** compresses succession + protection of another scorer; **Taqeul CoC36** Pheroware is stronger as a combat/support operator but worse pure cheap insurance. Lt Sukeul FO29 is an exposed command risk, not automatic best button.

[Cross-faction apex and points-value guide](../../notes/list-building/mission-specialists-and-button-pushers-apex-value.md). Use **this roster and Fireteam chart** for exact availability.

## N5.3 airborne / backline-strike archetypes and trades (2026-10-23)

**Jaan Staar IMP-2**, **Kiiutan Imposters** and **Gao-Tarsos Combat Jump/Parachutist** are legitimate alternate DZ-assault vectors, but **Jaan Staar/Kiiutan share AVA in pinned Tohaa** (don't purchase independent maximums). **Cube Jäger Irregular Parachutist** trades cheap disruption/Paramedic role for lower pool value. **Clipsos Hidden/Infiltration** starts near side objective but does not directly deploy into enemy DZ. **Kaeltar CoC21/.5 with SymbioMate** protects a separate active fighter or important mission scorer; it is not an off-table assault profile. Assess arrival risk and actual scored mission benefit before buying multiple assassins.

[Full N5.3 apex/value and delivery-probability tier guide](../../notes/list-building/airborne-and-enemy-dz-attackers-apex-value.md). Current roster/profile restrictions and canonical Fireteam chart above govern legal choices.

## Active-turn gunfighter cross-reference (2026-10-23)

**Active-turn shooting choices:** **Sukeul HMG33/1.5** is a **non-TAG** BS13/Mimetism(-3)/active 2W Symbiont shooter in a useful Triad; **Sukeul FO K1 Combi29/0** trades range for armor removal and mission access. **Gao-Rael MSV2 Spitfire30/1.5** is the anti-Mimetism/smoke alternate, with shorter bands. **Gorgos AP HMG63/1.5** belongs to the separate **TAG** ranking, paying more for ARM7, TacAware, and possible Chaksa support; Fireteam mobility and objective role are the reason cheaper infantry guns compete. [Separate TAG/non-TAG ceiling and points value](../../notes/list-building/active-turn-gunfighters-apex-and-value.md).

## Warbands and cheap high-upside trading — N5.3

**Makaul HFT+Eclipse+Viral/DA CC14/0** is S-tier **team enabler** in a legal Triad: **Eclipse blocks MSV**, Heavy Flamethrower threatens W1 infantry, CC23/MA2 and specialty CC ammo deter Hackable/elite units. **Mirrorball/Kriigel competing view**: repeated no-LoF Pheroware vision denial often replaces Makaul as *pure smoke delivery*, but Makaul retains cheap HFT/melee+Triad role. **Ioann Bann32/0** is a multi-Wound aggressive dog-warrior, not 14pt disposable smoke. **Kaeltar CoC21/.5** with SymbioMate supports survival of scorer/command; do not throw the protected CoC first.

[Current cross-game warband apex/value, target counters and LT/CoC tiers](../../notes/list-building/warbands-and-cheap-trading-units-apex-value.md). Pinned profile choices and canonical Fireteam chart in this roster remain authoritative.

## TAG tactical cross-reference (2026-10-23)

**Gorgos (63)** has AP HMG, Flammenspeer, Pulzar and multiple wounds/states; for **67–70** the added Chaksa peripheral buys close-range/utility screening, not simply more TAG gun Burst. It is often the most efficient way for Tohaa to add an armored attack axis if existing Eclipse/K1/mission tools can clear approach threats. The 2025 podcast hosts disagreed partly because of limited personal experience versus actual frequent Gorgos use.

For the two-tier **apex/points-value** comparison, TAG counterplay, matchup matrix and direct transcript sources: [N5.3 TAG field guide](../../notes/list-building/tags.md). Treat current profiles, points/SWC and canonical Fireteam data above as authoritative.

## Hacker and KHD tactical cross-reference (2026-10-23)

**Aelis Keesan KHD 25/0 WIP14** brings **Sensor, Triangulated Fire, Regeneration and a useful combat gun** to a legal Tohaa Triad: Trinity/Cybermask are valuable secondary roles on a mission specialist. **Kamael HD17/0.5** offers much cheaper ordinary **Carbonite/Oblivion/Spotlight**, and **Wardriver HD14/1** adds otherwise scarce cyber utility at high SWC cost. **Why:** Tohaa's strengths are generally Triads, Eclipse and resilient objective carriers rather than a Nomad-style Repeater lattice. Field Aelis for *combined combat/specialist/anti-Hacker duties*, not because the KHD alone dominates an absent network; don't pay Wardriver SWC if Tohaa gun/mission resources are more urgently needed.

See the [cross-game apex/value Hacker/KHD tier guide](../../notes/list-building/hackers-and-killer-hackers.md). **The sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative; device upgrades are profile-specific.**


## Cheerleader / Order-generation tactical cross-reference (2026-10-23)

See [Cheerleaders and Order Generators — N5.3 apex, points-value and matchup guide](../../notes/list-building/cheerleaders-and-order-generators.md) for complete comparative tables and verified transcript disagreements. The **current roster above controls** legality, AVA, Training and Fireteams.

- Kamael — S2 Regular line/triad material; price its fireteam/mission role rather than chasing pure Orders-per-point.
- Kaeltar — supporting SymbioMate/Triad capability adds utility but no separate Order for attached equipment.
- Wardriver — useful only for its hacking/Specialist role; high SWC for a generic cheerleader is inefficient.

**Order audit:** add up only deployed eligible **Regular** Orders in each Combat Group; special LT/Tactical, Irregular and Peripheral activations are not transferable pool Orders. Buy the cheapest protected body that supplies the *second function the list truly needs*; consider large-base DZ crowding, expensive mandatory Fireteam slots, and whether another scoring specialist beats one more cheap Order.


## ARO apex/value cross-reference (2026-10-23)

[Best ARO units across N5.3 — absolute apex vs points-value](../../notes/list-building/aro-units-apex-and-value.md) compares hidden reactive fire, TR/Neurocinetics, Flash/DTW/expendable defenders and why competing creators disagree. The **roster here** is authoritative for actual costs, Training, AVA and Fireteam construction.

- **Nikoul Viral sniper** — 25pt Sapper and Viral long-lane attrition with Symbiont; needs real range and vision match
- **Taagma MSV2 Viral sniper** — 22pt visor, Holomask and Counterintelligence role compression vs camo/smoke
- **Kaauri E/M Minelayer** — 11pt S1 Sixth Sense/Biometric/MSV1 rear-zone assassin trap and cheap Regular Order
- **Gao-Rael sniper** — MSV2/2W Symbiont support for visible long-lane presence; more expensive than Kaauri/Taagma

**Best circumstance:** long exposed lanes justify a real sniper/missile/linked gun; dense tables, DZ landings and mission rooms favor E/M, mine, Shotgun, Riotstopper and hidden traps. Cover the destination/approach, layer serial threats rather than two pie-sliceable visible guns, and preserve scoring units for the active turn.

## N5.3 midfield area denial / speed bumps (tactical synthesis)

**Zero-SWC rear guard:** **Kaauri E/M Minelayer 11/0** gives a small Sixth Sense/MSV1/Biometric anti-intrusion body and a deployment mine, not an infiltrator. **Hidden Clipsos Shock Minelayer 23/.5** is genuine midfield surprise but its **FO 26/0** is separate and Hidden orders are withheld; **Draal 33/1 Shock Minelayer** adds a robust 2W FD body. **Draal Dazer 32/0 is NOT Minelayer**; its Dazer placement later costs Orders. **Counterpoint:** a fast Kotail/Gao-Tarsos mission run or cheap Kaauri may be better than overbuying hidden mines.

[Cross-game apex/value, matchups, and transcript disagreements](../../notes/list-building/midfield-area-denial-and-speed-bumps-apex-value.md). Tactical evaluation, not a modification to Army profiles or Fireteam legality.

## Doctor / Engineer / Recovery cross-reference (2026-10-23)

**Kumotail21 WIP14 Doctor+Engineer + Chaksa Servant3** is an efficient one-slot dual network, able to work with legal Triad routes **or** remotely with Servants (respect Fireteam restriction). **Kosuil Engineer20–25** instead offers an assault-side K1/shotgun shooter and technical support inside a legal moving Triad; worth its points when it contributes attacks/objectives, not as a pure 20pt rear Engineer. Symbiont models use their relevant current attribute/state; inspect patient eligibility before Doctor versus Engineer choice. [Doctor/Engineer apex and recovery odds](../../notes/list-building/doctors-engineers-and-recovery-apex-value.md).

## N5.3 DZ defense / anti-alpha-strike tactical choices

**Kaauri E/M Minelayer 11/0** is an extraordinary **Regular** home guard against Impersonation: Biometric Visor, Sixth Sense, MSV1, strong Discover and Nanopulser(+1B) plus an already-laid E/M Mine. Put its mine on the intruder's **next corner/reveal square**, not adjacent to valuable cheerleaders. **Chaksa Auxiliar FTO 10/0** adds **HFT + Sensor + Baggage** and a Regular Order; not a REM or Biometric guard. **Opposing view (TA Tohaa):** multilayering with Draal mines/Nikoul/Kriigel is potent but can over-invest in static defense instead of scoring. Kaauri Mirrorball14/.5 is a different profile.

[DZ Defenders — whole-game apex/value, matchups, and MCP transcript debate](../../notes/list-building/dz-defenders-alpha-strike-and-impersonation-apex-value.md). Tactical commentary; the pinned profile/Fireteam tables above are authoritative.

## Close-combat assassins and counter-CC — N5.3 (2026-10-23)

**Makaul14/0** is the standout *value* **CC23 MA2 + Eclipse + HFT + Viral/DA**, opening a safe route for the whole Triad while threatening short-range attacks. **Igao Vulkan23/0** is **Infiltration/Camo/MA3/DA** better for a concealed opening strike; **Mirrorball26/.5** adds a different vision-control route. **Neema32** is durable forward CC22/MA2 with important ranged work, not a pure assassin. Transcript dissent: cheap Eclipse Makaul often contributes more than paying for niche 1W Igao. [Dedicated CC assassin apex/value, delivery and counter-CC](../../notes/list-building/dedicated-close-combat-assassins-apex-value.md).

## N5.3 network projection — Pitchers, Repeaters, TinBots and disposable delivery

**Kamael FO+Deployable Repeater13/0**, **Sukeul FO+Deployable Repeater29/0**, and **Kotail FO+Deployable Repeater32/0** provide physical node placement while doing mission work, but **without printed Minelayer these do not begin as extra Turn-0 Repeater tokens**. Standard Tohaa Pheroware is **not automatically the same as conventional Hacking Device programs routed through Repeaters**: verify chosen Wardriver/other actual Hacker and eligible target before investing in a network. **Counter:** Tohaa typically gains more from Kaauri mine/Biometric, Kriigel Mirrorball/Pheroware, and scoring Triads than from a conventional Pitcher/Guided network copied from Nomads.

[Whole-game apex/value network guide, current profiles, and opposing media views](../../notes/list-building/network-projection-repeaters-pitchers-apex-value.md).

## Tactical cross-reference — toolbox units (2026-10-23)

**Draal32/0 Dazer or33/0 mine** is an unusually competent forward Specialist/denial generalist (FD+20, Mimetism-6, 2W, fast movement); Dazer and viral mine are **separate profiles**, not cumulative equipment. **Kriigel21/.5** excels at Mirrorball/Eraser control, and Taqeul35–36 adds command—not the same gun or Dazer tool. Pairing multiple toolboxes in Triads creates redundancy but risks starving the Sukeul attack plan of points/Orders. [Cross-game apex/value tiers](../../notes/list-building/jack-of-all-trades-toolbox-units-apex-value.md).

## N5.3 rare abilities & unusual combinations — tactical synthesis

**Makaul HFT+Eclipse+Viral/DA CCW14/0** is extremely rare **Regular + Impetuous + Triad Eclipse** with a direct-template guard/trader in same package; **Chimera19/0** elsewhere buys a different peripheral swarm but not Tohaa Triad access. **Kriigel Mirrorball21/.5** repeats **Eclipse-like control through Pheroware** but is not a standard throwable Eclipse grenade; choose when the existing Triad also exploits its commands. **Kaauri11/0 Biometric+Sixth Sense+MSV1+E/M Minelayer** is another ultra-cheap anti-IMP role combination, particularly protecting high-value Triad orders. **Opposing:** several command/vision/defense layers together are strong in dense scenarios but can tax actual active Orders; a Makaul plus two useful objective members often wins more than expensive redundant rare abilities.

[Whole-game rare capability apex/value, rules, matchups and opposing MCP transcripts](../../notes/list-building/rare-capabilities-and-unique-combinations-apex-value.md). Use current profile and Fireteam chart above.

## Anti-TAG / Anti-HI without hacking — N5.3 (2026-10-23)

**Kaauri11 E/M Minelayer** is excellent static counter-TAG deterrence; **Reex16 K1 Marksman B3** is cheap repeatable **ARM=0** fire, **Kosuil Engineer20 Panzerfaust or 25 K1 Combi** is flexible close/mid can-opener, **Sukeul29 K1 Combi FO** more reliable BS13+mission worker. **Cube Jäger15 Mono /18 E/Mitter+Mono** offers flank assassination but is Irregular; **Kiiutan27 E/Mitter/Impersonation** breaks rear support/engineering. **Gorgos63 AP HMG TAG** is a separate budget; Eclipse+Viral Makaul14 is delivery, not guaranteed TAG kill. [Non-hacking anti-TAG/HI apex/value and target matchups](../../notes/list-building/anti-tag-anti-heavy-infantry-non-hacking-apex-value.md).

## N5.3 objective holding, zone domination & carried-objective choices

**Best Tohaa sustained scoring:** **Sakiel FO20/0** (initial W2 Symbiont, Viral/E/M, Triad) is exceptional value; **Sukeul FO29/0** (W2 Symbiont, Mimetism(-3), K1, Repeater) is durable anti-armor carrier; **Taqeul CoC36/0** (W2 Symbiont/Regeneration/Mirrorball) can protect an important zone and command; **Ectros Viral33/0** or **Vulkan32/0** supplies mobile heavy **W3 Symbiont VP** in a Triad but is **not FO merely by Ectros name**. **Makaul HFT+Eclipse14/0** shields the carrier from MSV/normal fire, while **Kaauri E/M Minelayer11/0** defends pickup squares. **Gorgos63/1.5** 4W/ARM7 Symbiont TAG shifts large zone differential but lacks ordinary box Specialist; peripherals add *distinct physically valuable* angles at 67/70pts. **Opposing TA Tohaa:** Triad with two specialists+Eclipse creates scoring resiliency that 63pt Gorgos by itself lacks; Gorgos better if already using it to fight and zone swing.

[Cross-game zone-holder and carrier apex/value, mission rules, and opposing transcripts](../../notes/list-building/objective-holding-zone-domination-and-carriers-apex-value.md). Current local roster/FT chart is authoritative.

## Anti-Tech — enemy visors, Mimetism, markers and Impersonation (2026-10-23)

**Kaauri E/M Minelayer11/0** is one of the game's best economical **Biometric+MSV1+Sixth Sense+Discover+mine** rear guards versus Fiday/Speculo and Camo, but 1STR and MSV1 only reduces Mimetism(-6) to -3. **Chaksa Auxiliar FTO Sensor10/0** is cheap ZoC/Hidden detection + HFT/Baggage; **Aelis Keesan25/0 Sensor+Triangulated Fire** is the specialist Triad solution. **Taagma22/1.5 MSV2 Viral Sniper** is the long anti-Mimetism shot. **Kriigel21/.5 Mirrorball vs Makaul14 Eclipse:** first wins repeated projected anti-MSV lanes, second a single linked HFT/CC assault. The Tohaa podcast strongly favors Mirrorball, but the actual Triad job and Orders decide.

[Full N5.3 anti-tech apex/value, rules, matchups and transcript disagreements](../../notes/list-building/anti-tech-msv-mimetism-camo-impersonation-apex-value.md).

## Force multipliers — N5.3 role/value cross-reference (2026-10-23)

**Taagma Holomask+Counterintelligence15/0** is among best cheap first-turn command buffs while remaining a legal Triad body; **22/1.5 MSV2 Viral Sniper** is the expensive combat option, not an improvement to Counterintel. **Chaksa Auxiliary FTO10/0 Baggage+Sensor** can support disposable ammunition and Camo detection in a legal team; it is *not* a standard EVO Repeater engine. **Samsa Decoy** is static deception, not an Order/independent ARO. Expensive Triads can still fail when all their buffs compete with one real Sukeul gun or objective scorer. [Whole-game guide](../../notes/list-building/force-multipliers-special-abilities-apex-value.md).

## N5.3 peripheral / synchronized / multi-body apex-value update

**Cheap durable synchronized fork:** **Rasail Boarding Team BSG+Shock Mine+Chaksa27/0** (W3 active Symbiont, Nanoscreen) offers controller gun and bundled Chaksa close threat with different legal targets; **Viral31/0** and **Spitfire34/1.5** change range, not 3 Regular Orders. **Kerail+Surda25/0**, **+two Surda33/0**, **+Mutan30/0** creates Smoke-assisted expendable SymbioBeast close threat with actual bundling and subtype restrictions, not independent free Regular troops. **Gorgos TAG63/1.5 without bot vs 67/1.5 Pulzar Chaksa /70/1.5 LSG Chaksa** is major cost/active-fork difference; a regular Gorgos profile has **no included Chaksa**. **Kumotail/Engineer/Doctor + 3pt Chaksa Servant** is long-distance healing/repair geometry (max one patient per Order), not new attack Order. **TA Tohaa counterviews:** synchronized Gorgos/Chaksa elite corner defense versus **25–33pt Kerail** whose smoke and cheap beasts can create more forks per point. Keep the expensive controller protected: lose parent and no free independent Chaksa gun.

[Cross-game multi-body apex/value and transcript disputes](../../notes/list-building/peripheral-synchronized-multibody-apex-value.md). Current sectorial roster and N5.3 rules decide actual type and access.

## Battle-report effectiveness and combinations (qualitative, 2026-11-01)

**Repeated synergy:** **Makaul Eclipse** supports a **Sukeul/Gao-Rael / Triad shooter or cargo specialist**; **Kriigel pheroware/E/M, Kaeltar Symbio support, Neema/Sakiel/Chaksa and Rasail** supply layered survivability, templates and denial. #189's winning Data Harvest Tohaa defense protected collector routes with multiple resilient bodies/short-range threats; the opposing Shasvastii lost Orders fighting a TR HMG instead of delivering collectors. [#189](../../notes/battle-reports/181-190-n5-battle-report-tactical-analysis.md).

**Tactical limits:** In #224 a Tohaa **Sukeul/Makaul/Kriigel** fortress lost its final cargo carrier to Hatamoto after first-turn activation failures. #217's player found **Makauls inefficient as stand-alone shooters**, even though **Eclipse** remained strategically useful; against Stigmata hackers, an otherwise resilient Gorgos/Clipsos plan lacked a secured physical server-destruction route. [#224](../../notes/battle-reports/221-230-n5-battle-report-tactical-analysis.md) · [#217](../../notes/battle-reports/211-220-n5-battle-report-tactical-analysis.md).

**Role-based pick:** Makaul for visual delivery/close deterrence, Kriigel for specific ZOC disruption, Sukeul for gun/FO scoring and cheap peripheral protection for corridors. Protect the actual console/carry operator; do not equate Triad survivability with automatic mission scoring.

[Cross-report synthesis and evidence cautions](../../notes/battle-reports/cross-report-unit-effectiveness-and-combinations.md).

## Mission performance — battle-report evidence (2026-11-01)

| Mission(s) | Tested composition / scoring mechanism | Evidence |
|---|---|---|
| **Data Harvest / carried-objective defense** | Neema Saatar/Sakiel/Chaksa, Rasail and Kaeltar with Sukeul gun denied collector delivery lanes, won 4–1 vs Shasvastii. | [#189](../../notes/battle-reports/181-190-n5-battle-report-tactical-analysis.md) |
| **Critical Intervention / room defense or assault** | Kriigel E/M pheroware + Makaul Eclipse + Sukeul/Libertos protected objective room, but Tohaa lost final data-pack carrier to Hatamoto after delayed first-turn progress. | [#224](../../notes/battle-reports/221-230-n5-battle-report-tactical-analysis.md) |
| **Mindwipe / sabotage vulnerability** | Gorgos/Clipsos/Makaul Eclipse approach could reach a console but failed to destroy enemy AI versus Stigmata hackers; Bakunin score provisional. | [#217](../../notes/battle-reports/211-220-n5-battle-report-tactical-analysis.md) |
| **Hardlock / resilient objective plan** | Makaul/Rasail/Kaeltar and durable Triad bodies provide escort/holding options; #093's opponent chose Dino zone-saturation specifically to contest Tohaa resilience. | [#093](../../notes/battle-reports/091-100-n5-battle-report-tactical-analysis.md) |

**Limits:** Do not confuse Makaul Eclipse movement value with being a reliable primary gun. Printed current anti-materiel and Specialist capability determine Mindwipe options. Game-era qualitative evidence, not a win-rate or current Fireteam claim. [Full mission evidence audit](../../notes/battle-reports/cross-report-mission-performance-by-sectorial.md).

## Counterplay — observed N5 battle-report responses (2026-11-02)

| Threat / target | Observed response and limitation | Battle reports |
|---|---|---|
| **Against elite HI / room** | Kriigel pheroware E/M and Makaul Eclipse deter Hatamoto approach, while Rasail/Chaksa templates and Kaeltar/Sakiel resilient bodies defend contested objective corridor. | [#224](../../notes/battle-reports/221-230-n5-battle-report-tactical-analysis.md), [#189](../../notes/battle-reports/181-190-n5-battle-report-tactical-analysis.md) |
| **Camo/Impersonation / scoring** | Makaul Eclipse and independent Sukeul/Libertos or hidden Specialist can travel around snipers, but #217 player found Makauls poor primary shooters. | [#217](../../notes/battle-reports/211-220-n5-battle-report-tactical-analysis.md), [#224](../../notes/battle-reports/221-230-n5-battle-report-tactical-analysis.md) |
| **Counterexample: breach** | Shinden Hatamoto/Shizoku/Yamabushi pressure removed the final data pack Paramedic; Tohaa Camo/room fortress failed when no protected carrier survived. | [#224](../../notes/battle-reports/221-230-n5-battle-report-tactical-analysis.md) |

**Limit:** Do not claim Tohaa automatically defeats defensive HI; #224 is a defender-successful counterexample in an asymmetric mission. These are historical qualitative interactions, not present N5.3 unit, Fireteam, or win-rate claims. [Full cross-report counterplay analysis](../../notes/battle-reports/n5-cross-report-counterplay-tags-hi-hacking-camo-impersonators-fireteams.md).

---

## Must-have / Go-to / Avoid — source-backed recommendations (2026)

The following dated assessment preserves source-backed tactical classifications, disagreements and miniature purchase guidance. It is **opinion and collection advice**, not a substitute for the roster, profiles or Fireteam chart above.

**Consolidated audit title:** Tohaa N5.3 — Must-have / Go-to / Avoid (YouTube and podcast evidence)

**Audit:** 25 October 2026. **Scope:** standard Tohaa (Army faction `801`), not former Spiral Corps or Reinforcements. **Current rules/profile baseline:** [Tohaa N5.3 roster and Fireteam reference](tohaa.md), Army `7.26246.159` (3 September 2026), verified 15 October 2026. **Companion tactical analysis:** [Tohaa list-building guide](../../notes/factions/tohaa.md). Recorded opinions are *qualitative recommendations*, not measured tournament inclusion rates. Costs and legality are checked against the current repository, not older captions.

**Evidence standard:** A *must-have / near-must* is described by a presenter as an auto-include or staple in almost all lists. *Go-to* is a generally safe role-efficient selection but never compulsory. *Avoid* is an identifiable bad-value profile or package that a named presenter criticizes; **“never” is not a claim of mathematical domination without a full current-profile comparison**. When speakers disagree, preserve the disagreement. Transcripts can misspell Tohaa, Kaeltar, Sukeul, Kriigel, Taqeul, Kiiutan, Chaksa, etc.; canonical names below follow the repository.

### Source key — actual recordings

| Key | Recording and evidence | Edition/limits |
|---|---|---|
| **RS26** | [Robert Shepherd — N5 Tohaa Faction Focus](https://www.youtube.com/watch?v=93L3POjJKkU), **full ~124-minute YouTube MCP transcript consulted**. Most direct modern individual-unit evaluation; notably Kaeltar/Sukeul/Delegate auto-includes, the value of Kriigel/Ioann Bann, and Ectros/Kiel-Saan/Chaksa avoidance. | Current-era N5 opinions; verify individual profiles against pinned N5.3 roster. One commentator, not usage statistics. |
| **TA25** | [Tactical Awareness — Zeroes & Heroes: Tohaa](https://www.youtube.com/watch?v=i1tcqWpV9jQ) / [podcast](https://open.spotify.com/episode/5zhPiR44EzbQ4GFKkICRvG), Oct 2025; both YouTube and podcast transcripts consulted. Multiple actual army builds, Taqeul/Kaeltar/Kriigel, Gorgos and objective trade-offs. | Earlier N5 roster and local player perspective. |
| **MX26** | [T1E8 — Entrevista Ejército Tohaa, Sectorial Regio](https://open.spotify.com/episode/1ryq6mbCHeSBdcfNIiiqpO), July 2026, Spanish; podcast transcript consulted. Two experienced players weigh mission-first construction and question expensive Reex/Kiel-Saan packages; one still enjoys Kiel-Saan. | Spanish automated transcript, approximate spellings/timing; pre-September roster. |
| **RS-tier26** | [Robert Shepherd/Jordan — July 2026 N5 faction tier list](https://www.youtube.com/watch?v=1dW3i9dpI34); Tohaa placed near top of C, arguing traditional multiwound/Fireteam/visibility edge is less distinctive in N5. | Faction-level comparative opinion, not a unit-pick survey; predates current Ioann Bann roster. |
| **LoL25** | [Loss of Lieutenant E142 — N5 TAG Tier List](https://open.spotify.com/episode/1h5CJfZC5zBPxdg66o7xIN), April 2025; transcript findings retained in [Tohaa guide](../../notes/factions/tohaa.md). Mixed/C-level views of Gorgos, including limited direct experience. | Early N5, historical comparison only. |
| **MC23** | [MetaChemistry E70 — Faction Takedown: Tohaa](https://open.spotify.com/episode/5jADKiplmnNSdZKBNCEPd7), July 2023; podcast transcript consulted. Opponent's perspective on Pheroware and vulnerability to STR targets. | N4: relevant to strategic roles, **not** N5 profile costs or current rule interpretations. |

[Historical Tohaa tournament interview, Loss of Lieutenant E87](https://open.spotify.com/episode/1IQ6KijBbjWYqIfSIIqTeG) was located but the podcast transcript was unavailable; **do not cite it as evidence of a specific unit judgment**.

### Quick verdict

| Category | Units/profiles | Overall confidence |
|---|---|---|
| **Must / near-must** | **Kaeltar Specialists** (often 1–2); **Sukeul Commandos** (especially HMG and/or K1 FO); **Tohaa Diplomatic Delegate 5pt Specialist** | High: explicitly near-auto or universal language in RS26 |
| **Go-to — core support/attack** | **Kriigel**, **Taqeul LT (+1 Order)**, **Kaauri 11pt E/M Minelayer**, **Chaksa Aux FTO 10pt**, **Makaul 14pt**, **Ioann Bann**, **Taagma 15pt or MSV2 sniper**, **Kosuil Engineer** | High-to-medium: strong general reasons, alternative architectures exist |
| **Go-to — mission or matchup** | **Samsa**, **Kiiutan Zapper**, **Greif IMP-2**, **Draal**, **Clipsos FO**, **Nikoul Viral Sniper**, **Gao-Tarsos Paramedic**, **Kamael FO/Hacker**, **Gorgos** in a dedicated TAG plan | Medium: specific role, budget, deployment, and scenario make the pick |
| **Generally avoid** | **Ectros NCO HMG41/1.5**, **Kiel-Saan49**, **Chaksa Aux Neurocinetics HMG24/1**, **Sakiel Spitfire22/1.5**, **Kamael Spitfire18/1**, **Gao-Rael Spitfire30/1.5**, **Sukeul ML34/1.5** in tight SWC lists | Primarily RS26; Kiel-Saan and ML disputed, **not universal unit bans** |

### 1. Must-have / nearest auto-includes

| Unit / profile | Why almost every list wants it | Evidence and qualification |
|---|---|---|
| **Kaeltar Specialists — 15/0; CoC21/.5; 2-Mate CoC28/.5** | SymbioMates materially increase the first-engagement survival of Symbiont gunfighters/ARO pieces; SymbioBombs lend single-use Mirrorball, Eraser or Endgame access. Linkable, WIP14, and optional Chain of Command support aggressive Lt choices. | **RS26 ~27–32m** explicitly presents Kaeltar as the closest thing to an auto-include and often takes two (15pt plus 21pt CoC or two 15pt). **TA25** army-building panel also treats Kaeltar as a recurrent backbone. **Do not assume 28pt CoC with two Mates is intrinsically cheaper than two Kaeltars:** it is a concentrated alternate loadout, 7pt more than the 21pt CoC. |
| **Sukeul Commandos — HMG33/1.5; K1 FO29/0; K1 Sniper28/1** | BS13 Mimetism(-3), Warhorse, Transmutation and legal Triads. HMG is the repeatable five-dice linked attacker, K1 FO can defeat armor while scoring, carrying D-Charges and placing a Repeater; K1 sniper provides lower-SWC long-range contesting. | **RS26 ~48–54m** says the regiment belongs in nearly every Tohaa list, and specifically recommends HMG and K1 combi. **TA25** and [existing guide](../../notes/factions/tohaa.md) independently build around Sukeul. The exact profile is a role choice; don't force an HMG alongside Gorgos if SWC and missions disagree. |
| **Tohaa Diplomatic Delegate — Specialist Operative5/0** | Very cheap Irregular objective button-pusher plus Nanopulser and reusable **Eraser** against Vitality-based targets; enormous value for a low-demand combat-group slot. | **RS26 ~88–90m** explicitly says to include the 5pt *Specialist Operative* in every list, calling it one of the strongest 5pt purchases. **Avoid substituting the identically priced Journalist(+3)** when the job is scoring; 5pt Specialist and Journalist are distinct loadouts. |

*No other Tohaa unit meets a strong evidence-based “every army list” test.* In particular, Mirrorball is usually desirable **as a capability**, but Kriigel and Taqeul are alternatives; likewise Eclipse can come from Makaul, Ioann Bann or Pheroware.

### 2. Go-to — generally high-return choices

| Unit/profile | Why and when it is better | Why it is not mandatory | Recording |
|---|---|---|---|
| **Kriigel Agent21/.5** | Linkable repeatable WIP13 **Mirrorball + Eraser**; reliable two-dice Mirrorball when appropriately linked, and offensive isolation/denial against **W/Vitality**, not STR. Defends a forward position or escorts a gun. | Costs 0.5 SWC and has limited direct shooting; Taqeul Lt and/or bomb carriers can supply some control. | **RS26 ~58–60m**, TA25 |
| **Taqeul Lt (+1 Order)35/0** | WIP14 linked Mirrorball + Endgame, good survivability, and Lt orders that can be spent on useful Pheroware setup rather than requiring exposed combat. CoC36/0 is an alternate non-Lt command option. | 35–36pts is expensive; without a plan to spend Lt orders or control the center, buy cheaper attack/scoring tools. | **RS26 ~60–63m**, TA25 |
| **Kaauri E/M Minelayer11/0** | Regular order, Sixth Sense, MSV1, Biometric Visor and E/M Mine cover the deployment zone against impersonation/AD/infiltration; cheap defense without an expensive ARO weapon. | May be redundant if a different mine screen already exists; do not assume its S1/STR makes it an ordinary combat REM. | **RS26 ~84–88m** |
| **Chaksa Auxiliary FTO HFT10/0** | Baggage, Sensor, Regular order and Heavy Flamethrower; inexpensive DZ guard and Baggage resupply where permitted, particularly for Endgame/Disposable equipment. | FTO profile is not an independent Chaksa link by itself; its named team needs a legal Longarm anchor. | **RS26 ~84–87m**, TA25 |
| **Makaul HFT + Eclipse + DA CCW14/0** | Reusable Eclipse blocks even MSV, cheap CC threat and template coverage in a Triad; gives close-assault utility Kriigel cannot match. | RS26 says its earlier almost-universal role has been eroded by Mirrorball/new options. Impetuous/No Cover makes a careless reactive deployment fragile. | **RS26 ~54–57m**, TA25 |
| **Ioann Bann32/0** | Irregular + Impetuous forward motion, fast Dog-Warrior/smoke/close assault, and **Triad-compatible** profile. Enables unusual attack sequences when combined with Lt activations and late team formation. | Costs a roster slot/Irregular order and requires careful formation timing; cannot be treated as generic Regular order fuel. | **RS26 ~62–69m** (specific N5 Tohaa new-role analysis) |
| **Taagma Counterintel15/0; MSV2 Viral Sniper22/1.5** | Cheap Holomask/Counterintelligence in a legal Triad; MSV2 sniper can shoot through **normal Smoke** projected by Ioann Bann, supplying a distinct range answer. | MSV2 sniper spends real SWC and is only BS12; Counterintel less important when order stripping is unlikely. | **RS26 ~69–73m**, TA25 |
| **Kosuil Engineer20/0 BSG+Panzerfaust; K1 25/0** | WIP14 utility/specialist in an advancing Triad, Deactivator/D-Charges, anti-armor option and SymbioBomb carrier. Mines on more expensive profile may help fortify forward ground. | Paying 5 extra for K1/AP-mining package can be inefficient; **Minelayer variant is not the Engineer** in the current roster. | **RS26 ~43–48m**, TA25 |
| **Samsa26/0** | Infiltration, Decoy, fast Super-Jump, Plasma Rifle, Mimetism and specialist status: high-impact independent first-order strike and Classified access. | A single-Wound Exrah can die to one mistake; do not leave it exposed just because of Decoy. | **RS26 ~91–94m** |
| **Kiiutan Imposter27–29/.5 (especially Zapper29/.5)** | IMP-2 deployment threatens immediate backfield attacks; Zapper gives a dangerous active/reactive fork against attempts to discover it. Saves SWC vs Jaan Staar. | Vulnerable to discover-shoot and layered DZ defense; **Jaan Staar and Kiiutan share AVA1, cannot both be taken.** | **RS26 ~93–98m** |
| **Greif IMP-2 21/.5** | Cheap independent backfield disruption, can force defensive movement even if it fails to kill a key unit; separately available alongside Kiiutan/Jaan. | W1, BS11 and risky aggressive deployment; choose the **IMP-2** profile, not presume that all Greif loadouts have impersonation. | **RS26 ~96–99m** |
| **Draal Dazer32/0 / Viral Mine33/0** | Forward Deployment +20, Mimetism(-6), specialist and area denial; strong when needing an objective-holding midfield specialist. | 32–38pts, considerable opportunity cost versus Sukeul and cheaper FO, transmutation loses much of its gunfighting edge. | **RS26 ~73–77m**, TA25 |
| **Clipsos FO26/0** | Hidden Deployment Mimetism(-6) Infiltrating scorer; threatens objective play without exposing the specialist early. | TA25 discusses lists without Clipsos; mobility/order demands can favor Kotail FO/Gao-Tarsos instead. | **TA25**, [guide synthesis](../../notes/factions/tohaa.md) |
| **Nikoul Viral Sniper25/1.5** | Sapper, MSV1, long range and Viral threaten flesh-based advancing units; Mate can force extra orders to remove. | Viral does not threaten STR targets the same way; fixed firing lane and 1.5 SWC are real constraints. | **RS26 ~108–111m**, TA25 |
| **Kamael FO13/0 + Hacker17/.5 (as a pair of tools)** | Very cheap linkable objective/deployable Repeater and basic hacking access; can create an extra anti-HI/TAG interaction otherwise missing in Tohaa. | Not a generally powerful hacker/network faction. Kamael BS11 baseline is poor; buy for the mission/network, not gunfighting. | **RS26 ~32–40m** |
| **Gao-Tarsos Paramedic24/0** | Cheapish AD mission/scoring fork, BSG + D-Charges on a resilient entering attacker. | Costs more than budget specialist and can exhaust valuable Regular orders trying to reach objectives. | **TA25**, [guide synthesis](../../notes/factions/tohaa.md) |
| **Gorgos63/1.5 or 67/1.5 with Pulzar Chaksa** | Tohaa's **only TAG**, AP HMG, BS14, ARM7/BTS9, Tactical Awareness, Chaksa Peripheral E/M pressure. Better when an actual durable STR/armor solution is required. | Expensive package, no strong visual modifier and needs a specialist/recovery plan. RS26 cannot fit it into his preferred lists; TA25/LoL25 are more sympathetic. **Not an unconditional avoid or “bad TAG.”** | **RS26 ~111–116m**, **TA25**, **LoL25** |

**Other credible role options, not default go-tos:** **Sakiel FO/Paramedic20–21** (durable linked button-pusher with Viral+E/M, compared with cheaper Kosuil/Kamael), **Jaan Staar30/1** (more direct CC assassination than Kiiutan but steeper SWC), **Igao23–26** (powerful Camouflaged melee assassin but can whiff or idle all game), **Kerail25–33** (fast SymbioBeast pressure, high setup/positioning cost), **Armand Le Muet** (superior independent long-range shot quality at a substantial premium), **Rasail** (multi-body wound economy but slow to make it count). These are **situational**, not evidence-backed never-takes. Sources: RS26 discussion ~40–45m, ~90–112m; TA25; [current guide](../../notes/factions/tohaa.md).

### 3. Generally avoid / “never take” audit

These are **presenter-backed negative picks**. Distinguish a unit-wide condemnation from one weak profile, and retain dissent.

| Unit/profile | Evidence-based criticism | Better use of the resources / caveat | Evidence strength |
|---|---|---|---|
| **Ectros HMG + NCO41/1.5** | **RS26 ~78–80m** explicitly calls the NCO a trap: 41pt hackable BS13 gun with no visual modifiers, paying a premium just to spend Lt orders. | **Sukeul HMG33/1.5** is cheaper and Mimetism(-3); **Taqeul Lt** itself can spend Lt orders productively on Mirrorball. [Older guide](../../notes/factions/tohaa.md) presents Ectros NCO as *possible* order conversion; **this ranking flags that meaningful dissent rather than silently deleting the prior idea**. | **High negative opinion; not strict stat dominance** |
| **Kiel-Saan Mk12 / Red Fury49** | **RS26 ~80m** describes it as meme/very bad in modern Tohaa: expensive, limited to **Reex/Chaksa** team families rather than normal versatile Triads with specialists, failing to convert the nominal combat package into efficient scoring. | **Sukeul**, **Ioann Bann** or **Samsa** fit the attack plan with better order/delivery opportunities. **MX26 disagrees in part:** one player runs Kiel-Saan by preference; another considers it too costly. | **Strong negative, explicitly disputed** |
| **Chaksa Auxiliary HMG with Neurocinetics24/1** | **RS26 ~83–86m** dismisses it as an inefficient static ARO purchase in an army short on points and SWC. | **10pt FTO HFT/Sensor/Baggage**, **11pt Kaauri Minelayer**, or a properly positioned **Nikoul/Taagma** for actual long-lane needs. | **High** |
| **Sakiel Spitfire22/1.5** | **RS26 ~37–42m** generally avoids basic gunfighter Sakiel: BS12, modest range/visual leverage for precious SWC. | **Sukeul HMG33/1.5** is better when buying a true attack gun; **Sakiel FO20/0** or Paramedic21/0 provides a distinctive specialist role. | **High for profile, not whole regiment** |
| **Kamael Spitfire18/1** | **RS26 ~32–37m** calls Kamael general fighting stats among the worst value, and sees merit in FO/Hacker/Paramedic instead. | **Kamael FO13/0**, or save for **Sukeul HMG** as the primary shooter. | **High for profile** |
| **Gao-Rael Spitfire30/1.5** | **RS26 ~80–82m** finds BS12, slow movement and costly linked MSV smoke shooting underwhelming. | **Taagma MSV2 Viral Sniper22/1.5** for the affordable smoke/ARO job, or **Sukeul** for superior general offense. **Not strictly dominated**: range, transmutation and weapon differ. | **Medium-high** |
| **Sukeul Missile Launcher34/1.5** | **RS26 ~51–53m** explicitly avoids its +6pt/+0.5 SWC premium over K1 Sniper; prefers the less costly sniper for comparable long-range defensive jobs. | **Sukeul K1 Sniper28/1** where SWC/points are tight. **Dissent explicitly noted by RS26:** other players favor ML's two-dice reactive, high-consequence EXP/template threat. | **Disputed profile avoidance** |
| **Kaeltar CoC + two Mates28/.5** | **RS26 ~28–31m** finds the extra 7pts over the 21pt CoC version hard to pay, generally favoring 15pt and 21pt Kaeltars. | Take **21pt CoC** unless the *specific* second Mate on one body is necessary; two separate Kaeltars cost **36pts**, so the comparison is about versatility/bombs/slots, **not cheaper total cost**. | **Medium: luxury loadout, never absolute** |
| **Greif non-IMP infiltrator variants23–25/0** | **RS26 ~96–98m** argues these Mimetism forward-deployed guns lack the high-quality attack/retaliation tools that make Greif worth taking. | **21pt IMP-2 Greif** for immediate backfield pressure; **Samsa** for infiltrating specialist firepower. | **Medium-high for these variants** |

#### Niche, not “never”

| Unit | Why usually cut | Why an honest audit cannot call it useless |
|---|---|---|
| **Hatail Aelis Keesan25/0** | **RS26 ~80m** says overcosted KHD/hard to get value in an army with weak hacking infrastructure. | WIP14, Sensor, D-Charges, K1/AP and varied Classified eligibility; scenario-specific utility is real. |
| **Kumotail21/0** | **RS26 ~80–82m** sees little reason for general lists outside specific Classifieds. | Combined Doctor+Engineer role and Chaksa Servant support can make excellent recovery infrastructure. |
| **Rasail27–34** | **RS26 ~104–108m** calls it too order-inefficient despite four-Wound body+Peripheral package. | Very durable LT/assault distraction, dangerous Chaksa HFT if protected; RS26 even reports a scenario win with a Rasail. |
| **Neema Saatar32–41** | **RS26 ~76–79m** finds many profiles vanity purchases versus cheaper Sukeul shooting and Taqeul Lt orders. | Three Wounds, mobility, WIP15, AP/CC and particular command plans are genuine differentiators. |
| **Kerail25–33** | **RS26 ~100–105m** considers it nerfed and tricky to use. | Presenter is actively experimenting with its fast one-Surda package and describes concrete group-two staging/CC success. |
| **Gorgos63–70** | **RS26** finds its points burden prohibitive in otherwise functioning lists. | **TA25** makes a positive case for the TAG, and RS26 acknowledges real AP-HMG/TacAware/Peripheral utility. |
| **Kiel-Saan49** | RS26's firm avoidance already listed. | MX26 reports a player who voluntarily uses it; at minimum label *highly inefficient in mainstream tournament builds*, not “never legal or never effective.” |

### 4. Concrete list-building implications

1. **First buy the essential capabilities:** one protected long gun (**Sukeul HMG**), one Pheroware/visibility plan (**Kriigel** or **Taqeul**), one SymbioMate/CoC plan (**Kaeltar**), a couple of actual objectives specialists, and one cheap rear screen (**Kaauri / Chaksa 10**). The **Delegate** is almost free but Irregular.
2. **Choose one attack architecture.** Traditional **Sukeul + Makaul/Ioann Bann + specialist** Triad advances with visibility control; newer **Samsa + Kiiutan/Greif + Ioann Bann** uses already-forward bodies for short, order-efficient strikes. **RS26** illustrates both.
3. **Do not neglect STR threats.** Eraser and Endgame are biological/Vitality threats; take real **K1/AP/E/M**, especially Sukeul K1, Kosuil K1 or Gorgos AP HMG. Use actual hacking only if bringing **Kamael FO/Repeater + Hacker** or other legal network sources. **MC23** opponent-side caution aligns with this.
4. **Two distinct scoring paths beat a third luxury ARO.** Hidden **Clipsos**, a linkable **Kosuil/Kamael FO**, or an AD **Gao-Tarsos Paramedic** must reach and complete missions after the main gun has fought.
5. **Current fireteam legality controls.** No Core; unlimited Triad/Haris and two Duos. Reex team requires Reex; Chaksa team requires Longarm. **Ioann Bann** has current Triad compatibility; don't import former Spiral fireteam charts. Jaan Staar and Kiiutan **share AVA1** and cannot appear together.

### Disagreements and edition boundaries

- **Source-backed ranking is not statistical truth.** RS26 is unusually explicit about “take” and “avoid” but is one player's experience. TA25 and MX26 are valuable balancing perspectives. **RS-tier26's top-of-C faction verdict** does not mean every Tohaa profile is weak.
- **Ectros NCO:** [existing guide](../../notes/factions/tohaa.md) allows the LT-order conversion angle; **RS26 calls its premium a trap**. Keep both viewpoints: cost and lack of Mimetism tip the default ranking to avoid.
- **Kiel-Saan:** RS26 is decisively negative; MX26 has a defender. Treat as deliberate off-meta assault investment, **not** literally impossible to win with.
- **Makaul:** formerly a near-auto Triad warband; modern **Mirrorball** and **Ioann Bann** reduce the need to buy one in *every* list. Still excellent for reusable Eclipse + HFT + serious CC.
- **Gorgos:** TA25/LoL25 debate capability relative to price; RS26 finds it hard to fit. It is the **only current TAG**, not directly dominated by Sukeul's much lighter chassis.
- **N4 sources are strategic context only**; Sept 2026 Army roster controls availability, current costs, legal teams and exact profiles. **No conventional REMs/VH units** appear in current base Tohaa roster, and the Motorcycle Bounty Hunter is not a VH.

**Bottom line:** Near-default **Kaeltar + Sukeul + 5pt Specialist Delegate**; fill core go-to roles using **Kriigel/Taqeul, Ioann Bann/Makaul, Kaauri/10pt Chaksa, Taagma/Kosuil**, then select independent striker or hidden scorer packages to match the mission. Avoid **Ectros NCO, Kiel-Saan, 24pt Neurocinetics Chaksa**, and overpriced secondary Spitfires as general-purpose default purchases; keep disputed niches explicitly conditional.

### Whole-unit purchase skips — full model rather than weak profile (2026-10-30)

These are **collection priorities**, judged across the current unit's usable profiles. **Skip by default** means the speaker's negative assessment covers the core purpose of the *whole* unit, but a named exception or dissent remains. It is **not** a claim that the unit is universally unplayable.

| Entire unit/model | Buying verdict | Why and when to reconsider |
|---|---|---|
| **Kiel-Saan (49pt)** | **Skip by default — strongest Tohaa whole-model candidate, disputed** | [Robert Shepherd Tohaa 2026 (RS26)](https://www.youtube.com/watch?v=93L3POjJKkU) considers its attack price/link restrictions too steep for modern Tohaa; Sukeul, Ioann Bann and Samsa provide more efficient routes. **MX26** reports an actual player who uses it. Buy if that specific Reex/Chaksa assault plan is desired, not simply for a “must-have” melee piece. |
| **Hatail Aelis Keesan (25pt)** | **Defer — low priority, niche** | RS26 criticizes a premium KHD without robust local hacking support. Buy when **WIP14, Sensor, D-Charges or K1/AP Classified coverage** fills a missing role. |
| **Kumotail (21pt)** | **Defer if recovery/classifieds are already covered** | RS26 sees limited broad-list demand; combined Doctor+Engineer plus Chaksa Servants gives distinct reach that a generic gun cannot replace. |
| **Chaksa Auxiliary as a unit family** | **Do not skip** | Only its **24pt Neurocinetics HMG** is strongly criticized; cheap **10pt Baggage/Sensor/HFT** versions are genuine role-efficient purchases. |
| **Ectros, Sakiel, Kamael, Gao-Rael, Sukeul, Kaeltar and Greif** | **Do not skip based on this audit** | Their condemned HMG/Spitfire/ML/CoC/non-Impersonation **profiles** do not invalidate their differently useful command, specialist or gun configurations. |

**Other optional, not all-profile avoids:** Rasail (reportedly won a scenario for RS26), Neema, Kerail and Gorgos all have distinct plausible uses or positive opposing accounts. Sources and dissent are detailed above in [the avoid audit](#3-generally-avoid--never-take-audit). See [cross-faction shortlist](../../notes/factions/model-purchase-avoid-summary-2026.md).

### Worst-value, rarely needed and proxy-first Tohaa miniatures (2026-10-30)

**Scope:** The [pinned September 2026 standard Tohaa faction roster](tohaa.md) is **one army**, not a family of currently fieldable sub-sectorials. This covers every standard Tohaa unit family relevant to a low-priority purchase. **Former Spiral Corps is a distinct discontinued NA2 army**; a Spiral sculpt may be a physical proxy, but its historical Fireteams, options and model access do not transfer into Tohaa. The companion [Tohaa tactical guide](../../notes/factions/tohaa.md) is the basis for the role comparison; the recordings below were previously transcript-reviewed for the main guide. No fresh pick-rate dataset was obtained. **“Rare” means a situational job in the reviewed list plans, not statistically established low tournament inclusion.**

**Verdict key:** **Skip/defer dedicated buy** = reasonable whole-miniature purchasing priority because the *usual job* compares poorly with other existing Tohaa tools, but named exceptions remain. **Avoid profile only** = same troop has good selectable alternatives; **do not avoid its sculpt or entire unit**. **Proxy first** = inference for a good-but-specialized model, before buying an expensive new miniature. **Extra copies** = the first unit can be exceptional, but buy duplicates only when you need **distinct simultaneous physical troopers** in a proven legal list. **Direct negative** identifies a particular recorded speaker, not mathematical strict dominance or population-wide consensus.

#### 1. Most defensible entire-unit purchases to postpone

| Entire troop / model family | Why its usual job often fails the buying test | Shopping decision and valid counterexample |
|---|---|---|
| **Kiel-Saan49** | **Strongest direct whole-model deferral.** [Robert Shepherd Tohaa 2026](https://www.youtube.com/watch?v=93L3POjJKkU) (~80min) considers it too expensive and awkwardly confined to **Reex / Chaksa-specific Fireteams** rather than the flexible conventional Triad; **Sukeul HMG/K1**, **Samsa** or **Ioann Bann** are often more useful attacking investments. **[July 2026 Mexican-player interview](https://open.spotify.com/episode/1ryq6mbCHeSBdcfNIiiqpO) is not unanimous**: one player voluntarily uses Kiel-Saan, the other is skeptical. | **Skip dedicated purchase by default; proxy/test one with a compatible HI silhouette/base.** Buy only for a deliberate **Reex/Kiel-Saan or Chaksa/Longarm/Kiel-Saan** package you actually intend to field. **Do not buy a Kiel-Saan on the assumption it joins ordinary Triads.** Buying two to AVA2 is a still narrower skew. |
| **Hatail Aelis Keesan25** | **Direct niche criticism, Shepherd** (~80min): pays for a **Killer Hacking Device** in an army without a natural wide conventional Repeater/hacking grid. **Kriigel/Taqeul Pheroware is not standard hacking**, and another Specialist often scores cheaper. *Exceptions:* WIP14, Sensor, Triangulated Fire, AP/E-M or K1, D-Charges and specific Classified requirements. | **Defer/proxy whole character first** unless her *precise* KHD/Sensor/anti-tech toolkit is a known mission requirement. This is **niche, not useless**, and the AP and K1 variants need not be separately bought if only one Aelis is on-table. |
| **Kumotail21** | **Direct Shepherd** (~80–82min) generally cuts it absent scenario/recovery needs; a 21pt one-wound Doctor+Engineer can cost more than a good mission scor­er or cheaper role-specific Kosuil. *Exception:* a **real Doctor+Engineer** is uniquely useful in particular rescue/Classified lists, with **Chaksa Servants** extending access. Kosuil Engineer isn't a Doctor, and its Minelayer loadout is not an Engineer. | **Proxy first; buy when double recovery/classified coverage is part of your recurring plan**. No categorical “Kumotail bad”: the breadth of Doctor+Engineer is its legitimate point. Include separate correctly based Servant models if fielded. |
| **Neema Saatar32–41** | **Direct negative in mainstream shooting by Shepherd** (~76–79min): expensive elite 3W character, often less cost-efficient than **Sukeul's Mimetism gun** or **Taqeul's Mirrorball/LT economy**. But Neema's distinct **WIP15, AP Spitfire, command +1 Order or +1 Command Token, durable close offense** are real. **Neema 36pt LT +1 Order / +1 SWC and 41pt LT +1 Command Token have different effects**, not an all-in-one profile. | **Proxy before dedicated purchase** if just filling “another premium gun” slot. Buy for deliberate **elite WIP15 lieutenant/command utility or tough AP attack**. AVA1 means one mini for mutually exclusive profiles suffices. |
| **Rasail Boarding Team27–34 plus appropriate Chaksa** | **Direct Shepherd (~104–108min) mixed review:** impressive Symbiont active Wounds, Nanoscreen, LT and shotgun/HFT **Peripheral** body, but often too slow/order-hungry versus Sukeul/Kosuil/Kriigel and hidden scoring. **He also reports winning a scenario with Rasail**; “never” would misrepresent the account. | **Proxy-test a complete Rasail + Chaksa package** when that selected profile includes the companion. Don't buy several to AVA4 for a default list; buy one if the **durable self-screening LT/area-holder** frequently matters. A single Rasail sculpt does not represent its separately deployed Chaksa. |
| **Kerail Preceptors25–33 plus one/two SymbioBeasts** | **Direct nuanced Shepherd (~100–105min):** nerfed, sometimes difficult to order efficiently, and overlaps **Makaul Eclipse/CC, Ioann Bann rush, Igao camo melee**. Yet he demonstrates practical **Surda** staging/close attacks and is actively testing them. Current options include **25pt + 1 Surda**, **33pt + 2 Surdas**, **30pt + 1 Mutan**. | **Proxy-test full controller + correct beast quantity/type** first. **Do not buy every Kerail/beast combination** before finding one reliable assault lane. More beasts are not independent Regular Orders. Legitimate specialist miniatures, not source-backed dead weight. |
| **Gorgos63–70**, the only current Tohaa TAG | **Highly disputed whole-model *investment*, not weak gun.** Shepherd rarely finds room for the 63pt AP HMG, while [Tactical Awareness Tohaa](https://open.spotify.com/episode/5zhPiR44EzbQ4GFKkICRvG) defends the **BS14 AP-HMG / Tactical Awareness / ARM7 / Peripheral** pressure; [Loss of Lieutenant TAG review](https://open.spotify.com/episode/1h5CJfZC5zBPxdg66o7xIN) has more reserved early-N5 rankings. Tohaa can instead use **Sukeul K1 + Kosuil K1 / Makaul** for armor. | **Proxy/borrow TAG-sized Gorgos before buying** if unsure about a TAG-centered list. **63pt Gorgos has no Chaksa peripheral; 67pt has a Pulzar/E-M Chaksa; 70pt has a Light Shotgun/E-M Chaksa.** Represent the extra body only when selected. **Do not mistake “expensive to buy/build around” for “bad TAG.”** |
| **Chaksa Longarms21–29 as a whole gun team** | **Reasoned, moderately lower-priority:** need **at least one Longarm** to anchor their named **Chaksa Duo/Haris**, while **Portable Autocannon29/1.5, ML24/1.5, Mk12/AP Mine25/0, Combi/E-M21/0** compete for points/SWC with **Sukeul, Taagma sniper, Nikoul and basic Kaauri/Chaksa**. These are **not** the same as **10pt Chaksa Auxiliary FTO**. A strong autocannon/A-P long lane or required legal team anchor can justify one. | **Proxy a Longarm + intended team first**, and **defer collecting all four**. Buy **one** when the specific anti-armor long gun / inexpensive team composition wins; buy second/third only for a tested actual team. **Do not mistake auxiliary FTO for the required Longarm anchor.** |
| **Chaksa Auxiliary24/1 Neurocinetics HMG considered as a dedicated model purchase** | **Strong direct negative for a *profile*, not a unit**, [Shepherd ~83–86min](https://www.youtube.com/watch?v=93L3POjJKkU): costly static reactive shooting competes poorly with **Kaauri11 E/M Minelayer**, **Nikoul25 Viral Sniper**, **Taagma22 MSV2 Viral Sniper** and multiple cheap defenders. The **10pt Baggage/Sensor/HFT FTO** is excellent. | **Defer the *HMG-only sculpture/purchase***; **do not skip acquiring an Auxiliary** for its 10pt utility. **15pt Guided HRL** is another distinct specialist shooting job, not generic standard missile network. Proxy optional HMG/HRL with a clearly identified S2 model. |
| **Reex Escort packages purchased as a default attack link without Kriigel or a real niche** | **Reasoned:** Reex **S1/STR1**, BS11, 12–16pt are *legitimate* cheap required anchors for a **Kriigel Mirrorball/Eraser Reex Haris/Duo** or Kiel-Saan experiment. But without the special team/cheap K1/Thunderbolt goal, standalone Reex offer less than a proper Triad specialist, 10pt Chaksa or 11pt Kaauri screen. Mexican-player discussion highlights how the former Spiral approach's efficiency changed. | **Proxy first if trying a Reex-specific team**; don't buy two just because AVA2. **Buy at least one separate Reex miniature if using the real Reex team**, or a proxy with its **S1 footprint**. Kriigel “counts as Reex” does **not** waive the one-Reex anchor requirement. |

**Whole-model shortlist:** most defensible **default skips** are **Kiel-Saan** and, absent their particular niche, **Aelis** and **Kumotail**; next **proxy-first investment candidates** are **Neema, Rasail/Chaksa, Kerail/beasts, Gorgos, Longarms, and a standalone-only Reex buy**. The last group is *situational, contested or architecture-dependent*, not evidence for a universal “never take.”

#### 2. Avoid paying for weak *profiles*, not the entire unit

| Specific loadout / intended use | Recorded criticism / role competition | Model recommendation / exception |
|---|---|---|
| **Ectros HMG NCO41/1.5** as an everyday ranged LT-order sink | **Direct negative RS26 ~78–80min**: expensive hackable **BS13 without Mimetism**, whereas **Sukeul HMG33/1.5** presents much better attack modifiers/value, and **Taqeul LT** can use extra LT Orders on *its own* Pheroware. **Older tactical note [tohaa.md](../../notes/factions/tohaa.md)** legitimately acknowledges an Ectros NCO order-conversion tactic; it isn't zero utility. | **Strong default avoid of the *41pt HMG NCO profile***, not all Ectros. **33pt Viral Combi, 32pt Vulkan Shotgun, 33pt LT and 39pt HMG** can serve resilient Triad/command/mid-range roles. Proxy alternate Ectros guns; do not buy an extra sculpt for NCO alone. |
| **Sakiel Spitfire22/1.5** as main aggressive gun | **Direct Shepherd ~37–42min**: BS12 gun costs serious SWC without Sukeul's attack modifiers. **Sakiel FO20/0 / Paramedic21/0** are valuable Symbiont Triad scorers/support. | **Avoid *Spitfire by default*; keep Sakiel for FO/Paramedic/LT needs.** One Sakiel can represent legal alternate weapon/role when not fielded concurrently. |
| **Kamael Spitfire18/1** (plain BS11 gun) | **Direct Shepherd ~32–37min**: swallows SWC while the 13pt **Kamael FO** and 17pt/.5 Hacker or cheaper line orders do useful team/scoring work; **Sukeul** wins the important fights. | **Avoid gunfighter variant**, *not* regular **Kamael** as Triad/cheap specialist. Proxy an occasional gun choice; do not buy a Spitfire model just to complete the roster. |
| **Gao-Rael Spitfire30/1.5** as an automatic MSV smoke shooter | **Direct Shepherd ~80–82min**: middling BS12, slower MI and costly SWC versus a **Taagma MSV2 Viral Sniper22/1.5**, **Nikoul25 Viral** or better general Sukeul offense. **Rangebands and weapon are different**, so not strict domination. | **Avoid *Spitfire as generic main gun***; other Gao-Rael long-range/visor/fireteam uses remain meaningful. **Proxy alternate weapon sculpt**. |
| **Sukeul Missile Launcher34/1.5** as the default Sukeul ARO | **Direct but *disputed* Shepherd ~51–53min**: he favours **K1 Sniper28/1** for 6pt/.5SWC saving. He acknowledges defenders who choose ML for **explosive/template/high-consequence ARO**. **Sukeul HMG33/1.5 and K1 FO29/0** are very strong and *not interchangeable* jobs. | **Avoid buying a dedicated Sukeul ML first** unless you want that specific reactive template role. **Prioritize HMG / K1 FO**, then proxy ML to test; **never skip Sukeul as a family**. |
| **Kaeltar 28/.5 CoC + two SymbioMates by default** | **Direct Shepherd ~28–31min**: he often prefers **15pt 1 Mate/1 Bomb** and **21pt CoC + 1 Mate/1 Bomb** for role economy; 28pt concentrated two-Mate CoC is a premium. **Two Kaeltars cost 36pt combined**, so do not falsely say two models save points versus one 28pt package. | **Avoid premium loadout unless two Mates on one model solve a specific list constraint**; buy first **Kaeltar(s)** for the highly praised protection/CoC system. **The Mate/Bomb markers are equipment, not separate extra troopers.** |
| **Greif non-IMP variants23–25/0** when buying an impersonation attacker | **Direct Shepherd ~96–98min**: inferior at the main early disruption job compared with **21pt Greif IMP-2**. **Samsa26** offers an unrelated Infiltration/Decoy/Plasma specialist job; **Kiiutan** offers a more durable IMP-2 angle. | **Avoid *non-IMP Greif for impersonation purpose***. Proxy an occasional off-meta gun/scout variant; don't blacklist **Greif IMP-2**. |
| **Tohaa Diplomatic Delegate Journalist(+3)5/0 when you actually need a Specialist** | **Direct high-value competing profile**: the **5pt Specialist Operative** offers scoring/mission interaction along with Eraser/Nanopulser; Journalist is a separate 5pt profile and cannot press buttons merely because the miniature looks similar. [Shepherd ~88–90min](https://www.youtube.com/watch?v=93L3POjJKkU). | **Pick Specialist for normal objective scenarios**, but **buy/proxy one Delegate**; no second model for the alternate card, and the unit's **Irregular** order stays Irregular. |
| **Chaksa Auxiliary Guided HRL15/1 as a free Guided ML replacement** | **Role/profile trap:** this is a specific **Guided Heavy Rocket Launcher** source loadout, **not a normal REM missile truck**. Tohaa has sparse conventional hacking/Spotlight projection: **Kamael Hacker + Repeater**, Wardriver and Sukeul/Kamael deployed repeaters require deliberate support. Not every Tohaa list can generate valuable Targeted states. | **Avoid purchasing a dedicated Guided artillery model until a legal, repeatable target chain exists**; an **Auxiliary FTO10** is the generally useful alternate model. **Do not assume the HRL option is itself eligible for the FTO-only Chaksa team.** |
| **Kamael Hacker17/.5 or Wardriver14–16/1 solely to imitate another faction's mass-hacking engine** | **Role-based inference:** Tohaa's **Pheroware Eraser/Endgame is not conventional Hacking/Spotlight** and does not affect all STR/TAG targets; a single inexpensive Hacker or Wardriver can be mission-relevant but doesn't create a whole projected repeater grid. | **Proxy a dedicated hacker/Disco Baller variation first**, buy only for actual anti-hackable/mission job. **Kamael FO/Repeater and ordinary Kamael/Kriigel are still solid buys.** |
| **Unnecessary third premium sniper/ARO model** (Nikoul, Taagma MSV2, Gao-Rael, Armand, Longarm) | **Synthesis of [Tohaa guide](../../notes/factions/tohaa.md):** these *different* ARO tools have genuine uses, but 1.5SWC guns/static sightlines compete and do not themselves score. **Armand** has a stronger independent sniper profile but much larger premium; **Nikoul Viral** is matchup-dependent versus W/STR. | **Proxy the additional sniper/weapon variant rather than automatically purchasing all models**; first correct ARO piece can be an excellent buy. Mix E/M/Kaauri/Chaksa screen and one meaningful long lane. |

**Do not translate any row here into “never buy Kaeltar, Sukeul, Sakiel, Kamael, Gao-Rael, Greif, Chaksa or Ectros.”** The bad verdicts concern a **particular weapon, role or price/SWC opportunity cost**. They were checked against the current [Tohaa profiles](tohaa.md) rather than older Spiral/Symbiont assumptions.

#### 3. Other situational whole miniatures better tested as proxies

These are **buy-later, not a negative tier ranking**. They fill jobs that can be excellent, but are unlikely to be part of *every* ordinary Sukeul/Kaeltar/Taqeul/Mirrorball/mission-specialist build.

| Model / niche | What makes the pick situational | Best buying decision |
|---|---|---|
| **Igao23–26** | Camouflaged close-combat assassin with conditional **Mirrorball** possibility, strong melee payoff, but **not a button-pushing Specialist** and may spend the game waiting or die before CC. Can be a very good surprise piece against a protected target. [RS26; Tohaa guide](../../notes/factions/tohaa.md). | **Proxy first or buy one**, not both to AVA2 unless marker-saturation melee play is intentional. An appropriately based **camo/close-combat infantry** stand-in is better than buying two specialist sculpts blind. |
| **Jaan Staar30/1 vs Kiiutan27–29/.5** | Both have real enemy-DZ Impersonation threats and alternate attack modes; **their current AVA1 is shared**. Kiiutan Zapper is often more efficient for disruption, Jaan has a specialized stronger melee assassination case. | **Buy/proxy only one Impersonator initially**, and test the other with a clearly identifiable compatible infantry sculpt. **You may not field Jaan and Kiiutan together** in current standard Tohaa; never buy two expecting a legal dual-assassin list. |
| **Second/third Gao-Tarsos, or Cube Jäger15–18** | **Gao-Tarsos Paramedic24** has more established resilient **Combat Jump/Parachutist objective reach**, while **Cube Jäger** is inexpensive **Irregular** Parachutist/Paramedic with Monofilament. They have different entry and Order economics. Too many off-table attackers weaken turn-one presence. | **Proxy the *second* airborne operative or Cube Jäger before buying**. Buy one after repeated mission use; respect **Combat Jump vs Parachutist** and correct identity. |
| **Draal32–38 Dazer/Mine specialist, Kotail holo/FO, Clipsos FO hidden scorer** | Each can legitimately win objectives with **Forward Deployment Mimetism(-6) + Dazer**, **Holo/Super-Jump scoring**, or **Hidden Deployment Mimetism(-6)** respectively. But **three expensive midfield specialists** may duplicate roles and displace a cheap **Kamael/Sakiel/Kosuil** specialist. Clipsos often justifies a dedicated first model. | **Proxy the *additional* midfield specialty trooper**, not a blanket skip of Draal or Clipsos. Buy if that exact deployment/hidden/zone-control skill repeatedly earns Orders/points. |
| **Rasail/Kerail specialist peripheral packages** | Their controllers' attached **Chaksa / SymbioBeasts** vary by selectable profile and are *separate bodies*, though they do not all produce independent Orders. Multi-body model count increases cost and deployment/hobby work even if the points look attractive. | **Proxy the *entire* chosen package** before buying, including each peripheral at the correct silhouette/base. **Kerail25=1 Surda, 33=2 Surdas, 30=1 Mutan; Gorgos63=no Chaksa, 67/70=one different Chaksa.** |
| **Motorized Bounty Hunter, Cube Jäger, Libertos or other Irregular-only additions** | **Motorcycle** brings fast side pressure, **Libertos Minelayer8/1** cheap mine/camo brake, and Cube Jäger parachute mission option; different roles and useful in right list. **Irregular/Impetuous do not provide pooled Regular Orders**. Current Tohaa motorcycle is **LI, not an N5 Vehicle (VH)**. | **Proxy uncommon rider / extra Irregular trooper first**; **do not skip the first Libertos Minelayer** merely because the order is Irregular—RS26 regularly values its mine control. |
| **Extra Makaul to AVA6 or extra Ioann Bann alternative** | **Makaul14 Eclipse/HFT/CC** still provides a unique reliable close visual-control tool. **Ioann Bann32** provides a different Irregular dog-warrior/Super-Jump/smoke attack and now has current Tohaa Triad compatibility. Multiple impetuous bodies can crowd the expensive gun/specialist structure. | **First Makaul is a compelling purchase** if Eclipse delivery is essential. **Proxy the third-to-sixth Makaul or another close attacker** if you never use them simultaneously. Do not downgrade Ioann solely because the presenter uses him in nonstandard teams. |
| **Additional Kaauri, Chaksa FTO and niche rear-defense copies** | **Kaauri11 E/M Minelayer/MSV1/SS** and **Chaksa Auxiliary FTO10 HFT/Baggage/Sensor** are cheap and generally *better* value than most expensive sniper AROs. But AVA4 each is not a target; maximum-screen lists can have too little active scoring. | **Buy the first affordable defensive pieces; proxy third/fourth copies** as needed. **Chaksa FTO requires Longarm anchor for its named team**; if unlinked, the 10pt body still has native utility. |
| **Second Sukeul, Kaeltar, Kosuil or specialist Triad variant** | **Sukeul HMG33 / K1 FO29**, **Kaeltar15 or CoC21**, and **Kosuil Engineer20/K1 Engineer25** have genuinely high ordinary list utility. Many lists want **two** Sukeul roles and **one or two** Kaeltar. But **Sukeul AVA4** and **Kaeltar AVA2** don't require buying four and two models before a list is tested. | **Buy physical simultaneous core roles you repeatedly use**; proxy **third/fourth Sukeul** and alternate weapons, or a second Kaeltar until real lists require them. A *good* unit can have low priority for extra sculpts. |
| **Special-interest characters/mercenaries** (Samsa, Armand Le Muet, Wardriver, Neema, Aelis, Taagma sniper) | **Samsa26** is an excellent individual threat (infiltrating Decoy/Plasma specialist) but **one-Wound** and finesse-heavy; **Armand** costs a premium for independent long-range gun, Wardriver pays for a sparse cyber trick, and Taagma has cheap Counterintel and expensive sniper mutually exclusive roles. | **Proxy individual specialist characters or weapon sculpts first**, then buy favourites that demonstrate a repeated unique job. **Do not imply Samsa and Taagma Counterintelligence are “bad”** because they need a particular plan. |

#### 4. Practical model-for-model proxy choices and buying order

**No current, authoritative Tohaa physical inventory** was found under the expected repository inventory paths, and no concrete owned counts for Tohaa have been verified. Consequently these are **model categories and plausible substitutions**, not fabricated ownership claims or a guarantee a particular mini is available for you.

| Unit you want to test | Good *type* of temporary physical proxy | Correctness and repeat-purchase rule |
|---|---|---|
| **Kiel-Saan, Neema, Ectros and other expensive single HI/command choices** | A spare distinct **compatible-silhouette Tohaa/other Corvus Belli heavy infantry** with the same base footprint; clearly identify exact weapon and profile. | **Kiel-Saan cannot use a generic Triad** and **Neema AVA1** needs only one figure even if several LT loadouts exist. No S2 infantry assumption for every large/complex model; check current silhouette. |
| **Aelis, Kumotail, Taagma, Samsa, Nikoul, Armand or other one-off support/sniper** | An unused, clearly distinct infantry/MI **specialist, hacker or sniper** mini of matching base/silhouette; maintain a printed roster note. | Use one correctly represented **AVA1 character/model per simultaneous trooper**; alternative gun/skill profiles are **not extra bodies**. For a Nikoul or sniper, LoF silhouette/cover geometry must be appropriate. |
| **Kamael, Sakiel, Sukeul, Gao-Rael, Kosuil weapon variants** | A spare **same-family or compatible-size Tohaa gunner** declared as HMG/K1/FO/Spitfire/ML etc.; optional simple weapon swap. | **Buy extra weapon sculpt only if multiple different profiles are on the table together**, e.g. Sukeul HMG + K1 FO, not because HMG and ML are both selectable on a single trooper. An FTO or LT marker is not a physical second unit. |
| **Kiiutan versus Jaan Staar, Greif impersonation, Igao camo assassin** | A **distinct suitable-silhouette infiltrator/assassin** figure with clear identity and required Impersonation/Camo markers. | **Jaan/Kiiutan are mutually exclusive under shared AVA1**, so their two dedicated models are an elective hobby purchase, never a way to deploy both. Greif is a different troop and **IMP-2** only on the relevant profile. |
| **Makaul/Eclipse melee and extra cheap Kaauri rear-guards** | Distinct **warband/guard miniatures** of correct size with clear Eclipse/HFT or E/M-mine roles; use temporary markers for mines. | Buy the **first** reliable Makaul and Kaauri when practical. More models only when **simultaneously** taking additional legal bodies; no need to purchase full AVA. |
| **Chaksa Auxiliary, Chaksa Longarm, Reex Escort** | **Auxiliary/Longarm** can use distinctly marked compatible S2-ish infantry only if actual silhouettes/bases match; **Reex is S1**, so not a generic normal-sized infantry stand-in. | **Reex team requires >=1 Reex; Chaksa team requires >=1 Longarm**; a player cannot proxy away required *trooper counts* or use a Kriigel/Chaksa Auxiliary in place of that legal anchor on the Army list. An Auxiliary FTO10 does **not** become the HMG24 profile's Fireteam rule. |
| **Gorgos + Chaksa; Rasail + Chaksa; Kerail + Surda/Mutan; Kumotail + Servant** | Correct-size TAG/infantry/controller **plus a separate appropriately sized physical model for each selected peripheral/Servant**. A borrowed TAG can test Gorgos if *silhouette and base* match; an infantry base can't silently represent a large TAG. | **Represent every fielded body at once**, including Gorgos67/70 Chaksa, Kerail25/30/33 beast(s), and chosen Servants. Equipment **SymbioMates/Bombs** are not extra autonomous troopers; don't confuse markers with figures. |
| **Gao-Tarsos, Cube Jäger, motorcycle mercenary or extra Kotail** | A distinct airborne infantry/rider/appropriate mobility model matched to current trooper footprint, not an imaginary off-board token once on table. | Check entry mode, facing and base. **Motorized Bounty Hunter** must be modeled with proper mounted geometry and remains LI; a TAG/VH proxy is not inherently appropriate. |
| **Former Spiral Corps or obsolete older Tohaa releases** | Reuse a previous sculpt **only as a clearly declared current roster unit** with compatible silhouette. Former Spiral names may still have a Tohaa entry (e.g. Draal/Kiel-Saan/Reex); former team permissions do not persist. | **Do not buy a box for a Fireteam or unit that the current Tohaa roster/chart doesn't allow**, and do not assume a special edition/resculpt changes rules. |
| **Kaeltar SymbioMate/SymbioBomb counters and marker-heavy tools** | Use labeled, non-confusing **equipment markers** for Mates/Bombs, Dazer, mines, Decoy, IMP and Holomask; field proper trooper figures where required. | **Markers are not new Regular troopers**. Buying multiple special-counter accessory packs is normally unnecessary if you already have clear rule-appropriate tokens. |

**Suggested collection order absent inventory and mission details:**

1. **First-model priorities (not a fixed army list):** **Kaeltar15**, one **Sukeul HMG33 or K1 FO29**, **Delegate5 Specialist**, a real visibility plan (**Kriigel21, Taqeul35 or Makaul14**), and cheap **Kaauri11 / Chaksa FTO10** where useful. Add the scoring specialist your selected missions require; note the Delegate is **Irregular**. [RS26](https://www.youtube.com/watch?v=93L3POjJKkU) and [TA25](https://open.spotify.com/episode/5zhPiR44EzbQ4GFKkICRvG).
2. **Buy one legitimate distinct game plan next:** hidden **Clipsos FO**, **Draal** Dazer/area defense, **Samsa** independent infiltration, **Kiiutan/Greif** impersonation, **Taagma** anti-smoke sniper, or **Gorgos** supported TAG. Don't buy all of them solely to cover their cards.
3. **Proxy-tested specialist investments:** **Kiel-Saan/Reex/Longarm**, **Aelis**, **Kumotail**, **Neema**, **Rasail + Chaksa**, **Kerail + beasts**, **Ectros NCO or other alternative gun**, **Gao-Rael Spitfire**, **Armand**, expensive third/fourth Sukeul, extra Makauls/Chaksas/snipers.
4. **Buy the models your lists repeatedly need simultaneously**, with all required peripheral bodies and correct silhouettes—not every AVA gap or alternate weapon profile. One clearly declared proxy model can test **several mutually exclusive options in different games**, but cannot be several troops at once.

**Proxy/event caveat:** All temporary substitutions must be **clearly identified**, correctly **based and silhouetted**, with complete physical body count for deployed peripherals; get opponent approval in friendly games and check the **current ITS/event organizer's** proxy rules for tournaments. A proxy does not change **unit access, shared AVA, Symbiont/Transmutation state, link eligibility, Irregular orders or the rules printed on the selected profile**. Ancient Spiral Fireteams, unrelated combined-army biotech and older edition profiles are not restored by swapping miniatures.

**Bottom line:** **Whole-unit deferrals** — Kiel-Saan first, then *niche-with-caveats* Aelis/Kumotail/Neema/Rasail/Kerail/Gorgos/Longarms; **strong profile-only avoids** — Ectros NCO HMG, Sakiel/Kamael/Gao-Rael Spitfires as generic shooters, Chaksa Neuro HMG, expensive Sukeul ML when K1 sniper suffices, Kaeltar 28pt two-Mate premium, Greif non-IMP infiltration and non-specialist Delegate in missions requiring a Specialist. **Proxy-first even when the unit is good:** alternative Sukeul/Kaeltar/Makaul sculpts, a second Kiiutan/Jaan alternative (never both in one list), extra high-end snipers, specialist characters, multiple physical peripheral packages and the lone Gorgos TAG. **Do not avoid the basic Tohaa triad engine or cheap objective/defensive pieces because another profile of the same troop was reviewed negatively.**
