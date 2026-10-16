---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 904
sectorial_slug: ikari-company
sectorial_name: Ikari Company
parent_faction: Non-Aligned Armies (NA2)
rules_baseline: N5.3
army_source_version: "7.26246.159"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-16
coverage: "Complete current Ikari Company main roster, standard loadouts and AVA, current Fireteam chart and reverse access index, optional Spec-Ops/Team-Ops boundary, linked Reinforcements boundary, and derived tactical indexes."
---

# Ikari Company — N5.3 sectorial reference

## Overview and provenance

Repository-native reference for **Ikari Company** (Army sectorial ID `904`), part of the Non-Aligned Armies (NA2). It is intended to answer roster, profile, AVA, points/SWC, Lieutenant, specialist, hacking/network, deployment, peripheral and Fireteam questions without reopening Army.

Sources used:

- Corvus Belli Army-derived revision `7.26246.159` from `massayoshi/infinity-army-backup` commit `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b` (`army: N5.3 + ITS18`, 2026-09-03).
- Versioned source: `n5/ikari/7.26246.159.json`, blob `20d1c5d0c981606515e95c08d02f48b921b92b76`.
- Aggregate source: `n5/ikari/ikari.json`, blob `e8cd8b1cb702f4ea7dacb38e9fb25c39d41f91d2` at the pinned source commit.
- InfinityDB normalization/semantics: commit `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: N5.3 + N5 FAQ v0.1.

Coverage notes:

- Covers **36 standard Ikari roster entries** explicitly assigned to faction `904` by the current Army source.
- `Rumbler Spec-Ops` (ID `1925`) and `NA2 Team-Ops` (ID `1939`) are optional-mode entries and are kept separate from the standard roster.
- Generic Soldiers-of-Fortune / mercenary-catalogue objects with an empty `factions` array are excluded. Explicit Ikari entries such as Brawlers, Diggers, Yuan Yuan, Bashi Bazouks, Armand Le Muet, Triphammer and Kiiutan are retained.
- Linked Reinforcement army ID: **999**. This is a Reinforcement-army identifier; it happens to share the number `999` with the Tankō unit ID, but they are separate namespaces.
- Army raw Fireteam `DUO: 256` is the source sentinel for effectively unlimited Duo formations, not a literal limit of 256.
- Disabled subordinate forms/peripherals such as TurtleMek are documented with their parent unit and are not counted as independent roster entries.
- `FTO` and specific profile restrictions are preserved wherever the Fireteam chart relies on them. A profile carrying an FTO label does not independently create Fireteam access.

## Sectorial summary

| Field | Value |
|---|---|
| Sectorial | Ikari Company |
| Parent faction | Non-Aligned Armies (NA2) |
| Army ID | `904` |
| Rules baseline | N5.3 + FAQ v0.1 |
| Standard Main roster entries | 36 |
| Optional-mode entries | Rumbler Spec-Ops; NA2 Team-Ops |
| Reinforcement roster | Army ID `999` |
| Core | up to 1 |
| Haris | up to 1 |
| Duo | unlimited/source `256` sentinel |
| Fireteam families | Keisotsu; Wú Míng; Tankō; Druze; Mechanized; Krakot |
| Explicit Wildcards | Authorized Bounty Hunters; Brawlers; Diggers; Rumbler Spec-Ops |

## Fireteam chart limits and sectorial-level restrictions

| Constraint | Current source value / normalized meaning |
|---|---|
| Core | `1` |
| Haris | `1` |
| Duo | `256` — normalized as unlimited Duos |
| Main/Reinforcement mixing | Main roster and Reinforcement roster `999` remain separate |
| Wildcards | Only the explicit Wildcard rows listed below |
| Profile restrictions | Preserve `FTO`, `Spec-Ops`, counts-as comments, `required` flags and source minimums exactly |

The chart contains six named Fireteam families plus a separate Wildcard list. The canonical chart below is authoritative; do not import Fireteam permissions from old N4 Ikari charts or another NA2/JSA sectorial.

## Unit roster index

| Unit ID | Unit | AVA | Type | Classification | Regularity | Notes |
|---:|---|---:|---|---|---|---|
| 17 | Sierra Dronbot | 1 | REM | Support | Regular | Total Reaction |
| 162 | Yáopú Pangguling | 2 | REM | Support | Regular | Baggage; EVO/TR options |
| 158 | Tokusetsu Butai | 2 | LI | Support | Regular | Doctor/Engineer |
| 19 | Fugazi Dronbot | 1 | REM | Support | Regular | Repeater |
| 379 | Druze Shock Teams | 4 | MI | Veteran | Regular | Hacker/KHD; Fireteam anchor |
| 154 | Karakuri Special Project | 2 | HI | Spec. Trained | Regular | STR 3; FO |
| 378 | Yuan Yuan | 4 | WB | Mercenary | Irregular, Impetuous | Airborne smoke warband |
| 1565 | Motorized Bounty Hunters | 1 | LI | Mercenary | Irregular, Impetuous | Bike |
| 987 | Brawlers | 4 | MI | Spec. Trained | Regular | Wildcard; counts as Druze |
| 1568 | Diggers | 2 | HI | Mercenary | Regular, Impetuous | Wildcard; counts as Druze |
| 160 | Yáoxiè Lù Duān | 1 | REM | Support | Regular | Holoprojector; MSV1 |
| 159 | Yáoxiè Rui Shi | 1 | REM | Support | Regular | MSV1/2 |
| 1834 | Yojimbo, Sword for Hire | 1 | WB | Character | Irregular, Impetuous | Foot identity |
| 161 | Yáozăo | 2 | REM | Support | Peripheral | Servant |
| 265 | Wardrivers | 1 | LI | Mercenary | Regular | Hacker / Commlink |
| 343 | Al Fasid Regiment | 1 | HI | Veteran | Regular | Smoke GL; Minelayer |
| 224 | Yojimbo, Motorized Sword for Hire | 1 | WB | Character | Irregular, Impetuous | Motorized identity |
| 1569 | Triphammer | 1 | TAG | Mercenary | Regular + Tactical Awareness | Mechanized Fireteam |
| 986 | Security Chief Arslan | 1 | MI | Character | Regular | Lt option; counts as Druze in chart |
| 752 | Desperadoes | 2 | WB | Spec. Trained | Irregular, Impetuous | Bike; smoke |
| 49 | Authorized Bounty Hunters | 2 | LI | Mercenary | Regular | Wildcard max 2 |
| 129 | Wú Míng Assault Corps | 5 | HI | Line | Regular | Fireteam anchor |
| 999 | Tankō Zensenbutai | 3 | HI | Line | Regular, Impetuous | Fireteam anchor |
| 1002 | Daiyōkai Dengekitai | 1 | HI | Headquarters | Regular | NCO |
| 1538 | Táowù | 1 | LI | Character | Regular | Counterintelligence; CoC option |
| 50 | Warcor | 1 | LI | Mercenary | Irregular | Journalist |
| 16 | Pathfinder Dronbot | 1 | REM | Support | Regular | Sensor; FO; TacAware option |
| 18 | Clipper Dronbot | 1 | REM | Support | Regular | Guided or FTO +1B ML |
| 756 | Krakot Renegades | 2 | LI | Mercenary | Regular, Impetuous | Duo anchor |
| 144 | Keisotsu Butai | 5 | LI | Line | Regular | Fireteam anchor; Lt options |
| 956 | Cube Jäger | 1 | LI | Mercenary | Irregular | Parachutist; Paramedic |
| 135 | Ninjas | 1 | SK | Spec. Trained | Regular | Hidden Deployment; Hacker/KHD/FO |
| 380 | Scarface & Cordelia | 1 | TAG + LI | Character | Regular + Tactical Awareness | Composite; Mechanized Fireteam |
| 1309 | Kiiutan Imposters | 1* | SK | Spec. Trained | Regular | IMP-2; source shared-AVA note with Jaan Staar |
| 325 | Bashi Bazouks | 4 | LI | Mercenary | Irregular | Airborne Holoprojector |
| 680 | Armand Le Muet | 1 | MI | Character | Regular | Mimetism -6 sniper |

Optional-mode entries are listed separately below and are not included in the 36-entry count.

## Unit details

### Sierra Dronbot

**Unit ID:** 17 · **Slug:** `sierra-dronbot` · **AVA:** 1 · **REM / Support / Regular**  
`MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | STR 1 | S 3`. Remote Presence, Courage, Total Reaction, 360º Visor.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 23 | 1 | HMG, PARA CCW (-3) |
| 2 | 18 | 0 | Thunderbolt (+1B), PARA CCW (-3) |

### Yáopú Pangguling

**Unit ID:** 162 · **Slug:** `yaopu-pangguling` · **AVA:** 2 · **REM / Support / Regular**  
`MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 2 | BTS 3 | STR 1 | S 4`. Baggage, Remote Presence, Courage, Immunity (Shock).

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 8 | 0 | PARA CCW (-3); **Repeater, Deactivator** |
| 2 | 15 | 0.5 | PARA CCW (-3); **EVO Hacking Device** |
| 3 | 19 | 0 | Combi Rifle, PARA CCW (-3); **Repeater, Total Reaction** |
| 4 | 12 | 0 | **FTO label in profile**; Light Shotgun, PARA CCW (-3); Repeater |

**Important:** the current Ikari Fireteam chart does not include Pangguling. Profile 4's FTO label alone does not create Fireteam access.

### Tokusetsu Butai

**Unit ID:** 158 · **Slug:** `tokusetsu-butai` · **AVA:** 2 · **LI / Support / Regular**  
`MOV 10-10 | CC 15 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Courage.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 14 | 0 | Combi Rifle, Pistol, CCW; **Doctor, MediKit** |
| 2 | 14 | 0 | Combi Rifle, D-Charges, Pistol, CCW; **Engineer, Deactivator, GizmoKit** |
| 3 | 15 | 0 | As profile 2 + **Deployable Cover** |
| 4 | 17 | 0 | As profile 2 + **Armed Turret (Combi Rifle)** |

### Fugazi Dronbot

**Unit ID:** 19 · **Slug:** `fugazi-dronbot` · **AVA:** 1 · **REM / Support / Regular**  
`MOV 15-15 | CC 13 | BS 8 | PH 11 | WIP 13 | ARM 0 | BTS 3 | STR 1 | S 3`. Repeater, Remote Presence, Courage, Mimetism (-3).

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 7 | 0 | Flash Pulse, PARA CCW (-3) |

### Druze Shock Teams

**Unit ID:** 379 · **Slug:** `druze-shock-teams` · **AVA:** 4 · **MI / Veteran / Regular**  
`MOV 10-10 | CC 16 | BS 12 | PH 11 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`. X-Visor, BS Attack (SR-1), Warhorse.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 20 | 0 | Combi Rifle, Chain-colt, Viral Pistol, CCW |
| 2 | 28 | 1.5 | HMG, Chain-colt, Viral Pistol, CCW |
| 3 | 21 | 0 | Combi Rifle, Chain-colt, Panzerfaust, Viral Pistol, CCW |
| 4 | 24 | 1 | Combi Rifle, Chain-colt, Grenade Launcher, E/M Grenade Launcher, Viral Pistol, CCW |
| 5 | 23 | 0 | Shock Marksman Rifle, Chain-colt, Viral Pistol, CCW |
| 6 | 25 | 0.5 | Combi Rifle, Pitcher, D-Charges, Viral Pistol, CCW; **Hacking Device** |
| 7 | 23 | 0 | Combi Rifle, Pitcher, D-Charges, Viral Pistol, CCW; **Killer Hacking Device** |

### Karakuri Special Project

**Unit ID:** 154 · **Slug:** `karakuri-special-project` · **AVA:** 2 · **HI / Spec. Trained / Regular**  
`MOV 10-10 | CC 10 | BS 13 | PH 10 | WIP 13 | ARM 3 | BTS 6 | STR 3 | S 2`. Courage, GizmoKit (PH=12), Immunity (Enhanced), Forward Observer, Remote Presence.

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 31 | 0 | Heavy Shotgun, Chain Rifle, Panzerfaust, Flash Pulse, Pistol, CCW |
| 3 | 35 | 0 | MULTI Rifle, Chain Rifle, Panzerfaust, Flash Pulse, Pistol, CCW |
| 4 | 38 | 0 | Mk12, Chain Rifle, Panzerfaust, Flash Pulse, Pistol, CCW |
| 5 | 31 | 0 | E/Mitter, Chain Rifle, Panzerfaust, Flash Pulse, Pistol, CCW |

### Yuan Yuan

**Unit ID:** 378 · **Slug:** `yuan-yuan` · **AVA:** 4 · **WB / Mercenary / Irregular, Impetuous**  
`MOV 10-10 | CC 22 | BS 10 | PH 14 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Booty, Parachutist, Combat Jump (PH=11), No Cover, Super-Jump (Jet Propulsion), Impetuous.

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 2 | 6 | 0 | Chain Rifle, Smoke Grenades, Heavy Pistol, AP CCW |
| 3 | 7 | 0 | Chain Rifle, Smoke Grenades, Pistol, DA CCW |
| 4 | 11 | 0 | Boarding Shotgun, Smoke Grenades, Pistol, AP CCW |
| 5 | 11 | 0 | Rifle, Smoke Grenades, Pistol, AP CCW |

### Motorized Bounty Hunters

**Unit ID:** 1565 · **Slug:** `motorized-bounty-hunters` · **AVA:** 1 · **LI / Mercenary / Irregular, Impetuous**  
`MOV 20-15 | CC 17 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 4`. Motorcycle, Booty (ReRoll), Limited Cover, Mimetism (-3), Impetuous.

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 8 | 0 | Boarding Shotgun, Pistol, PARA CCW (-6), Heavy Riotstopper |
| 2 | 9 | 0 | SMG, Chain-colt (+1B), Pistol, PARA CCW (-6) |
| 3 | 16 | 0.5 | Red Fury, Breaker Pistol, PARA CCW (-6) |

### Brawlers, Mercenary Enforcers

**Unit ID:** 987 · **Slug:** `brawlers-mercenary-enforcers` · **AVA:** 4 · **MI / Spec. Trained / Regular**  
`MOV 10-10 | CC 17 | BS 12 | PH 11 | WIP 12 | ARM 2 | BTS 3 | W 1 | S 2`. Sixth Sense.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 15 | 0 | Rifle, Light Shotgun (+1B), Pistol, CCW |
| 2 | 15 | 1.5 | Heavy Rocket Launcher, Assault Pistol, CCW; X-Visor |
| 3 | 25 | 1.5 | MULTI Sniper Rifle, AP Mine, Pistol, CCW; **MSV2** |
| 5 | 16 | 0.5 | SMG, Cybermine, Pistol, CCW; **Hacking Device** |
| 6 | 19 | 0 | Rifle, Light Shotgun (+1B), D-Charges, Pistol, CCW; **Engineer, Deactivator, GizmoKit** |
| 7 | 19 | 0 | Rifle, Light Shotgun (+1B), Pistol, CCW; **Doctor, MediKit** |
| 9 | 15 | 0 | Rifle, Light Shotgun (+1B), Pistol, CCW; **Lieutenant** |

Brawlers are explicit Wildcards with source comment `(Druze)` and maximum 2 in the Wildcard row.

### Diggers, Armed Prospectors

**Unit ID:** 1568 · **Slug:** `diggers-armed-prospectors` · **AVA:** 2 · **HI / Mercenary / Regular, Impetuous**

| State | MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Full Power | 10-10 | 21 | 11 | 13 | 12 | 3 | 0 | 2 | 2 |
| Battle-Ravaged | 10-10 | 21 | 10 | 12 | 12 | 2 | 0 | 2 | 2 |

CC Attack (+1B), Booty, Courage, Dodge (+2.5), Natural Born Warrior, Impetuous, Transmutation (1), No Cover.

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 18 | 0 | Rifle, Light Shotgun, Grenades, Pistol, AP CCW |
| 2 | 14 | 0 | Chain Rifle (+1B), Grenades, Pistol, AP CCW |

Diggers are explicit Wildcards with source comment `(Druze)` and maximum 2 in the Wildcard row.

### Yáoxiè Lù Duān

**Unit ID:** 160 · **Slug:** `yaoxie-lu-duan` · **AVA:** 1 · **REM / Support / Regular**  
`MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 6 | STR 1 | S 4`. Holoprojector, MSV1, Remote Presence, Surprise Attack (-3), Courage, BS Attack (+1B).

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 24 | 0 | Mk12, Heavy Flamethrower, PARA CCW (-3), E/M Mine |
| 2 | 20 | 0 | Thunderbolt, E/M Carbine, PARA CCW (-3), E/M Mine |

### Yáoxiè Rui Shi

**Unit ID:** 159 · **Slug:** `yaoxie-rui-shi` · **AVA:** 1 · **REM / Support / Regular**  
`MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 6 | STR 1 | S 4`. Repeater, Remote Presence, Courage.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 23 | 1 | Spitfire, PARA CCW (-3); **MSV2** |
| 2 | 21 | 0.5 | Red Fury, Mine Dispenser (Shock), PARA CCW (-3); **MSV1** |

### Yojimbo, Sword for Hire

**Unit ID:** 1834 · **Slug:** `yojimbo-sword-for-hire` · **AVA:** 1 · **WB / Character / Irregular, Impetuous**  
`MOV 15-5 | CC 24 | BS 12 | PH 14 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Martial Arts L4, Dodge (+2.5), Immunity (Critical), Minelayer, Stealth, No Cover, NWI.

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 19 | 0 | Contender (+1B), Nanopulser, Smoke Grenades, CrazyKoala, Pistol, DA CCW (PS=3) |

Source note: only one Yojimbo may appear in an Army List. Ikari also contains the motorized Yojimbo identity below; do not treat their separate roster rows as permission to duplicate the character.

### Yáozăo

**Unit ID:** 161 · **Slug:** `yaozao` · **AVA:** 2 · **REM / Support / Peripheral**  
`MOV 15-10 | CC 11 | BS 8 | PH 10 | WIP 13 | ARM 0 | BTS 3 | STR 1 | S 1`. Peripheral (Servant), Courage, Mimetism (-3).

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 3 | 0 | PARA CCW (-3); Servant, no Order generated |

### Wardrivers, Mercenary Hackers

**Unit ID:** 265 · **Slug:** `wardrivers-merc-hackers` · **AVA:** 1 · **LI / Mercenary / Regular**  
`MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 2`. Sixth Sense.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 14 | 1 | Boarding Shotgun, Flash Pulse, Cybermine, Pistol, CCW; **Hacking Device, Zero Pain upgrade** |
| 2 | 16 | 1 | As profile 1 + **Disco Baller** |
| 4 | 14 | 0 | Boarding Shotgun, Flash Pulse, Cybermine, Pistol, CCW; **Hacker, Commlink, Zero Pain** |

### Al Fasid Regiment

**Unit ID:** 343 · **Slug:** `al-fasid-regiment` · **AVA:** 1 · **HI / Veteran / Regular**  
`MOV 10-10 | CC 17 | BS 13 | PH 14 | WIP 14 | ARM 5 | BTS 6 | W 2 | S 5`. Albedo (-3), Warhorse, Minelayer, Sixth Sense, Combat Instinct.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 50 | 1.5 | HMG, Grenade Launcher, Smoke Grenade Launcher, Shock Mines, Heavy Pistol, CCW; BS Attack (SR-1) |
| 2 | 44 | 1.5 | Heavy Rocket Launcher, SMG, Shock Mines, Heavy Pistol, CCW; BS Attack (+1SD) |

### Yojimbo, Motorized Sword for Hire

**Unit ID:** 224 · **Slug:** `yojimbo-motorized-sword-for-hire` · **AVA:** 1 · **WB / Character / Irregular, Impetuous**  
`MOV 20-15 | CC 24 | BS 12 | PH 14 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 4`. Motorcycle, Martial Arts L4, Limited Cover, Dodge (+5), Mimetism (-3), Minelayer, NWI.

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 741 | 20 | 0 | Contender (+1B), Nanopulser, Smoke Grenades, Smoke Grenade Launcher, CrazyKoala, Pistol, DA CCW (PS=3) |

Source note: only one Yojimbo may appear in an Army List; this identity and the foot Yojimbo above are alternatives, not independently stackable characters.

### Triphammer, Repurposed Industrial TAG

**Unit ID:** 1569 · **Slug:** `triphammers-repurposed-industrial-tags` · **AVA:** 1 · **TAG / Mercenary / Regular + Tactical Awareness**

| State | MOV | CC | BS | PH | WIP | ARM | BTS | STR | S |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Full Power | 15-10 | 17 | 13 | 16 | 12 | 7 | 3 | 3 | 7 |
| Battle-Ravaged | 10-10 | 15 | 12 | 14 | 12 | 4 | 0 | 3 | 7 |

Booty, Tactical Awareness, Transmutation and source TAG support rules. Each current loadout includes a **TurtleMek** ancillary peripheral.

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 2 | 53 | 1.5 | AP Spitfire, Heavy Flamethrower, AP CCW; TurtleMek |
| 3 | 52 | 1.5 | AP Spitfire, Chain-colt (+1B), AP CCW; TurtleMek |
| 4 | 52 | 0 | Heavy Shotgun, Thunderbolt (+1B), AP CCW; TurtleMek |
| 5 | 48 | 0 | Heavy Shotgun, Heavy Rocket Launcher, Panzerfaust (+1B), AP CCW; TurtleMek |

### Security Chief Arslan

**Unit ID:** 986 · **Slug:** `security-chief-arslan` · **AVA:** 1 · **MI / Character / Regular**  
`MOV 10-10 | CC 17 | BS 13 | PH 11 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`. MSV1, X-Visor, BS Attack (SR-1), Courage, Dodge (+3), Warhorse, NWI.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 35 | 0 | MULTI Rifle, Light Shotgun, Viral Pistol, CCW, Disco Baller |
| 2 | 35 | 0 | Same; **Lieutenant** |

### Desperadoes

**Unit ID:** 752 · **Slug:** `desperadoes` · **AVA:** 2 · **WB / Spec. Trained / Irregular, Impetuous**  
`MOV 20-10 | CC 21 | BS 11 | PH 13 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 4`. Motorcycle, Courage, Dodge (+2.5), Sixth Sense, Mimetism (-3), Impetuous, No Cover.

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 2570 | 7 | 0 | Chain Rifle, Smoke Grenade Launcher, Smoke Grenades, Heavy Pistol (+1B), AP CCW (PS=7) |
| 2571 | 7 | 0 | Chain Rifle, Smoke Grenade Launcher, Smoke Grenades, Assault Pistol (+1B), Shock CCW (PS=7) |
| 2572 | 9 | 0 | Boarding Shotgun, Smoke Grenade Launcher, Smoke Grenades, Heavy Pistol (+1B), AP CCW (PS=7) |

### Authorized Bounty Hunters

**Unit ID:** 49 · **Slug:** `authorized-bounty-hunters` · **AVA:** 2 · **LI / Mercenary / Regular**  
`MOV 10-10 | CC 16 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Booty (ReRoll), Stealth.

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 2 | 12 | 0 | Boarding Shotgun, Pistol, PARA CCW (-6), Heavy Riotstopper |
| 3 | 19 | 0.5 | Sniper Rifle, Breaker Pistol (+1B), PARA CCW (-6) |
| 4 | 21 | 1 | Spitfire, Boarding Pistol, PARA CCW (-6) |
| 5 | 12 | 0 | SMG, Akrylat-Kanone, Breaker Pistol, PARA CCW (-6) |

Explicit Wildcard, maximum 2 in the source Wildcard row.

### Wú Míng Assault Corps

**Unit ID:** 129 · **Slug:** `wu-ming-assault-corps` · **AVA:** 5 · **HI / Line / Regular**  
`MOV 10-10 | CC 17 | BS 13 | PH 12 | WIP 12 | ARM 4 | BTS 3 | W 2 | S 2`. No Cube, Hackable, Dodge (+2.5).

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 2 | 27 | 0 | MULTI Rifle, Grenade Launcher, E/M Grenade Launcher, Boarding Pistol, CCW |
| 3 | 22 | 0 | Boarding Shotgun, Boarding Pistol, CCW; TinBot Firewall (-6) |
| 4 | 33 | 1.5 | AP HMG, Boarding Pistol, CCW |
| 5 | 19 | 0 | AP SMG, E/Marat, Boarding Pistol, CCW |
| 6 | 23 | 1.5 | Heavy Rocket Launcher, E/M Carbine, Boarding Pistol, CCW |
| 9 | 22 | 0 | AP SMG, E/Mitter, Boarding Pistol, CCW |

### Tankō Zensenbutai

**Unit ID:** 999 · **Slug:** `tank-zensenbutai` · **AVA:** 3 · **HI / Line / Regular, Impetuous**  
`MOV 15-5 | CC 23 | BS 13 | PH 13 | WIP 13 | ARM 3 | BTS 3 | W 2 | S 2`. Martial Arts L2, Limited Cover, Courage, Dodge (+2.5), Stealth, Impetuous.

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 18 | 0 | Blitzen, Light Shotgun, Pistol, Monofilament CCW, Shock CCW (PS=6) |
| 2 | 19 | 0 | Blitzen, SMG, Pistol, Monofilament CCW, Shock CCW (PS=6) |
| 3 | 19 | 0 | Flammenspeer, Contender, Pistol, Monofilament CCW, Shock CCW (PS=6) |
| 4 | 26 | 1.5 | Missile Launcher, Pistol, Monofilament CCW, Shock CCW (PS=6) |
| 7 | 19 | 0 | Blitzen, Light Shotgun, Disco Baller, Pistol, Monofilament CCW, Shock CCW (PS=6); Deactivator |

### Daiyōkai Dengekitai

**Unit ID:** 1002 · **Slug:** `daiy-kai-dengekitai` · **AVA:** 1 · **HI / Headquarters / Regular**  
`MOV 10-10 | CC 21 | BS 13 | PH 14 | WIP 13 | ARM 5 | BTS 3 | W 2 | S 5`. Martial Arts L2, BS Attack (SR-1), Courage, Stealth, NWI, **NCO**.

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 46 | 0 | MULTI Marksman Rifle, Panzerfaust, Pistol, AP+DA CCW |
| 2 | 47 | 1 | Red Fury, Panzerfaust, Pistol, AP+DA CCW |
| 3 | 50 | 1 | HMG, Panzerfaust, Pistol, AP+DA CCW |

### Táowù, Mastermind and Schemer

**Unit ID:** 1538 · **Slug:** `taowu-mastermind-and-schemer` · **AVA:** 1 · **LI / Character / Regular**  
`MOV 10-10 | CC 19 | BS 12 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`. Holomask, BS Attack (+1B), Counterintelligence, Dodge (+3), Natural Born Warrior, Immunity (Shock), Specialist Operative, Stealth.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 19 | 0 | Light Shotgun, E/Marat, Flash Pulse, Viral Pistol, PARA CCW (-9) |
| 2 | 16 | 0 | Contender, Pulzar, Flash Pulse, Viral Pistol, PARA CCW (-9) |
| 4 | 21 | 0 | As profile 2; **Chain of Command** |

Source Fireteam comment `(Druze)` in the Druze family.

### Warcor

**Unit ID:** 50 · **Slug:** `warcors-war-correspondents` · **AVA:** 1 · **LI / Mercenary / Irregular**  
`MOV 10-10 | CC 11 | BS 9 | PH 11 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Journalist.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CCW (-3); 360º Visor |
| 2 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CCW (-3); Sixth Sense |

### Pathfinder Dronbot

**Unit ID:** 16 · **Slug:** `pathfinder-dronbot` · **AVA:** 1 · **REM / Support / Regular**  
`MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | STR 1 | S 3`. Deactivator, Repeater, Remote Presence, Courage, Triangulated Fire, Forward Observer, Sensor.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 14 | 0 | Combi Rifle, Flash Pulse, PARA CCW (-3) |
| 2 | 17 | 0 | Same; **Tactical Awareness** |

### Clipper Dronbot

**Unit ID:** 18 · **Slug:** `clipper-dronbot` · **AVA:** 1 · **REM / Support / Regular**  
`MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 0 | BTS 3 | STR 1 | S 3`. Remote Presence, Courage.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 16 | 1.5 | Missile Launcher, PARA CCW (-3); **BS Attack (Guided)**; non-FTO |
| 5 | 19 | 1.5 | **FTO**; Missile Launcher (+1B), PARA CCW (-3); **no Guided skill on this loadout** |

Only profile **5** may fill the Clipper FTO rows in Wú Míng and Druze Fireteams. Do not transfer Guided from profile 1 to the FTO profile.

### Krakot Renegades

**Unit ID:** 756 · **Slug:** `krakot-renegades` · **AVA:** 2 · **LI / Mercenary / Regular, Impetuous**  
`MOV 15-5 | CC 23 | BS 11 | PH 13 | WIP 12 | ARM 1 | BTS 0 | W 1 | S 2`. Berserk (+1), Forward Deployment (+10), Warhorse, MetaChemistry (ReRoll), Super-Jump, Religious Troop, No Cover, Dodge (+5).

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 14 | 0 | Chain Rifle, Chest Mine, Grenades, Heavy Pistol, DA CCW; BS Attack (+1B) |
| 2 | 16 | 0 | Boarding Shotgun, Chest Mine, Heavy Pistol, AP CCW |
| 4 | 17 | 0 | SMG (+1B), Chest Mine, Heavy Pistol, DA CCW |
| 5 | 24 | 1 | Red Fury, Chest Mine, Heavy Pistol, AP CCW |

### Keisotsu Butai

**Unit ID:** 144 · **Slug:** `keisotsu` · **AVA:** 5 · **LI / Line / Regular**  
`MOV 10-10 | CC 17 | BS 11 | PH 10 | WIP 12 | ARM 1 | BTS 0 | W 1 | S 2`. Courage.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 10 | 0 | Combi Rifle, Pistol, CCW |
| 2 | 18 | 1 | HMG, Pistol, CCW |
| 3 | 15 | 1.5 | Missile Launcher, Pistol, CCW |
| 4 | 16 | 0.5 | Combi Rifle, CrazyKoala, Pistol, CCW; **Hacking Device, ECM: Hacker (-6)** |
| 7 | 11 | 0 | Combi Rifle, Flash Pulse, Pistol, CCW; **Forward Observer** |
| 8 | 12 | 0 | Combi Rifle, Pistol, CCW; **Paramedic, MediKit** |
| 9 | 10 | 0.5 | Combi Rifle, Pistol, CCW; **Lieutenant** |
| 11 | 9 | 0 | AP Rifle, Pistol, CCW |
| 12 | 12 | 0 | Thunderbolt, Pistol, CCW; BS Attack (-3) |
| 13 | 9 | 0.5 | AP Rifle, Pistol, CCW; **Lieutenant** |

### Cube Jäger, Mercenary Recoverers

**Unit ID:** 956 · **Slug:** `cube-jaeger` · **AVA:** 1 · **LI / Mercenary / Irregular**  
`MOV 10-10 | CC 16 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Immunity (Shock), Stealth, Parachutist; MediKit chassis.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 15 | 0 | Boarding Shotgun, Pistol, Monofilament CCW; **Paramedic** |
| 2 | 18 | 0 | SMG, E/Mitter, Pistol, Monofilament CCW; **Paramedic** |

### Ninjas

**Unit ID:** 135 · **Slug:** `ninjas` · **AVA:** 1 · **SK / Spec. Trained / Regular**  
`MOV 10-10 | CC 23 | BS 11 | PH 12 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Martial Arts L3, Camouflage, Hidden Deployment, Infiltration, Mimetism (-6), Surprise Attack (-3), Stealth, Climbing Plus.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 24 | 0 | Tactical Bow (+1SD), Shock Mine, Pistol, DA CCW |
| 4 | 27 | 0 | SMG, Pistol, DA CCW |
| 6 | 33 | 0.5 | SMG, Pistol, DA CCW; **Hacking Device** |
| 7 | 26 | 0 | Tactical Bow (+1SD), Shock Mine, Pistol, DA CCW; **Killer Hacking Device** |
| 9 | 30 | 0.5 | Boarding Shotgun, Flash Pulse, Pistol, DA CCW; **Forward Observer** |

### Scarface & Cordelia, Mercenary Armored Team

**Unit ID:** 380 · **Slug:** `scarface-and-cordelia` · **AVA:** 1 · **TAG + LI / Character / Regular**

**Scarface TAG:** `MOV 15-10 | CC 22 | BS 13 | PH 16 | WIP 13 | ARM 7 | BTS 6 | STR 3 | S 7`; Tactical Awareness and source TAG/transmutation package. Includes TurtleMek ancillary support.  
**Cordelia Turner:** `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`; Engineer, Deactivator, GizmoKit.

| Composite option ID | Pts | SWC | Included loadout |
|---:|---:|---:|---|
| 1 | 80 | 1.5 | Scarface Alpha: Mk12 (+1B), Heavy Rocket Launcher (+1B), DA CCW + Cordelia |
| 2 | 76 | 1.5 | Scarface Beta: AP HMG, Panzerfaust, DA CCW + Cordelia |
| 3 | 76 | 1.5 | Scarface Gamma: AP Spitfire (+1B), Panzerfaust, DA CCW + Cordelia |

Army stores Scarface and Cordelia as components of the composite selection; the Mechanized Fireteam chart references `SCARFACE` and `CORDELIA TURNER` separately.

### Kiiutan Imposters

**Unit ID:** 1309 · **Slug:** `kiiutan-imposters` · **AVA:** 1* · **SK / Spec. Trained / Regular**

| State | MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Active | 10-10 | 17 | 12 | 11 | 13 | 2 | 6 | 2 | 2 |
| Inactive Symbiont Armor | 10-10 | 17 | 12 | 10 | 13 | 0 | 0 | 2 | 2 |

Surprise Attack (-3), Courage, Dodge (+3), Stealth, Impersonation (IMP-2), Transmutation (1).

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 4862 | 29 | 0.5 | Combi Rifle, Zapper, Viral Pistol, CCW |
| 5100 | 27 | 0.5 | SMG, E/Mitter, Viral Pistol, CCW |

Source note: AVA 1* is shared with Jaan Staar globally. Jaan Staar is not a normal Ikari roster entry, but the source shared-identity/AVA note is preserved rather than discarded.

### Bashi Bazouks

**Unit ID:** 325 · **Slug:** `bashi-bazouks` · **AVA:** 4 · **LI / Mercenary / Irregular**  
`MOV 10-10 | CC 16 | BS 11 | PH 10 | WIP 12 | ARM 2 | BTS 0 | W 1 | S 2`. Holomask, Holoprojector, Surprise Attack (-3), Parachutist, Terrain (Zero-G).

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 13 | 0 | Contender (+1SD), Boarding Pistol (+1B), CCW |
| 2 | 14 | 0 | T2 Boarding Shotgun, Boarding Pistol (+1B), CCW; BS Attack (AP) |
| 3 | 16 | 0 | Rifle, Light Shotgun, E/M Mine, Boarding Pistol (+1B), CCW; **Specialist Operative** |
| 5 | 14 | 0 | Breaker Rifle, Boarding Pistol (+1B), CCW; **Specialist Operative** |
| 8 | 12 | 0 | SMG, Boarding Pistol (+1B), CCW; **Specialist Operative** |

### Armand Le Muet, Freelance Killer

**Unit ID:** 680 · **Slug:** `armand-le-muet-freelance-killer` · **AVA:** 1 · **MI / Character / Regular**

| State | MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Active | 10-10 | 21 | 13 | 12 | 13 | 2 | 3 | 2 | 2 |
| Inactive Symbiont Armor | 10-10 | 21 | 13 | 12 | 13 | 0 | 0 | 2 | 2 |

BS Attack (Shock), Forward Deployment (+10), Natural Born Warrior, Mimetism (-6), Stealth, Transmutation.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 2338 | 33 | 1.5 | MULTI Sniper Rifle, Nanopulser, Shock Mine, Breaker Pistol (+1B), Viral CCW; **Minelayer** |
| 2339 | 34 | 1.5 | MULTI Sniper Rifle, Nanopulser, Breaker Pistol (+1B), Viral CCW; **MSV1** |

## Lieutenant and order-control index

| Unit/profile | Function |
|---|---|
| Keisotsu profile 9 | Lieutenant, 10 pts / 0.5 SWC |
| Keisotsu profile 13 | Lieutenant with AP Rifle, 9 pts / 0.5 SWC |
| Brawler profile 9 | Lieutenant, 15 pts / 0 SWC |
| Arslan profile 2 | Lieutenant, 35 pts / 0 SWC |
| Táowù profile 4 | Chain of Command, 21/0 |
| Daiyōkai | NCO on every current profile |
| Pathfinder profile 2 | Tactical Awareness |
| Triphammer | Tactical Awareness on every current profile |
| Scarface | Tactical Awareness inside each composite Scarface & Cordelia option |
| Táowù chassis | Counterintelligence |

## Hacking and network index

### Hackers

- **Hacking Device:** Druze profile 6; Brawler profile 5; Wardriver profiles 1–2; Keisotsu profile 4; Ninja profile 6.
- **Killer Hacking Device:** Druze profile 7; Ninja profile 7.
- **EVO Hacking Device:** Pangguling profile 2.
- **Wardriver profile 4:** source encodes Hacker + Commlink/Zero Pain rather than a normal Hacking Device equipment row; preserve that distinction.

### Network / projection

- **Pitcher:** Druze profiles 6–7.
- **Repeaters:** Pangguling profiles 1/3/4; Fugazi; Rui Shi; Pathfinder.
- **Cybermines:** Brawler Hacker; Wardrivers.
- **Disco Baller:** Wardriver profile 2; Arslan; Tankō profile 7.
- **Sensor:** Pathfinder.
- **Guided:** **Clipper profile 1 only**. The Fireteam-capable FTO profile 5 has Missile Launcher (+1B) but does not carry the Guided skill in the current source.

## Deployment / marker-state index

- **Combat Jump / Parachutist:** Yuan Yuan.
- **Parachutist:** Cube Jäger; Bashi Bazouks.
- **Impersonation:** Kiiutan (IMP-2).
- **Hidden Deployment / Camouflage:** Ninjas.
- **Infiltration:** Ninjas.
- **Forward Deployment:** Krakot (+10); Armand (+10); Kiiutan operates through Impersonation rather than normal FD.
- **Holoprojector / Holomask:** Bashi Bazouks; Lù Duān; Táowù.
- **Fast attack:** Motorized Bounty Hunters; Desperadoes; motorized Yojimbo; airborne Yuan Yuan/Bashi.

## Vision-control and sensor index

- **Smoke:** Yuan Yuan; Desperadoes; both Yojimbo identities; Al Fasid Smoke Grenade Launcher.
- **MSV2:** Rui Shi profile 1; Brawler MULTI Sniper.
- **MSV1:** Rui Shi profile 2; Lù Duān; Arslan; Armand profile 2339.
- **Sensor:** Pathfinder.

## Canonical Fireteam definitions

Current chart limit: **1 Core, 1 Haris, unlimited Duos** (`DUO: 256` source sentinel).

### FT-01 — Keisotsu Fireteams

**Types:** Haris, Core  
**Anchor:** Keisotsu has source `min: 1`.

| Member | Unit ID | Required | Min | Max | Counts as / comment | Profile restriction |
|---|---:|---|---:|---:|---|---|
| Keisotsu | 144 | no | 1 | 5 | — | all |
| Tankō | 999 | no | 0 | 1 | — | all |

### FT-02 — Wú Míng Fireteams

**Types:** Haris, Core  
**Anchor:** Wú Míng has source `min: 1`.

| Member | Unit ID | Required | Min | Max | Counts as / comment | Profile restriction |
|---|---:|---|---:|---:|---|---|
| Wú Míng | 129 | no | 1 | 5 | — | all |
| Clipper Dronbot | 18 | no | 0 | 1 | `FTO` | **profile 5 only** |

### FT-03 — Tankō Fireteams

**Types:** Duo, Haris  
**Anchor:** Tankō has source `min: 1`.

| Member | Unit ID | Required | Min | Max | Counts as / comment | Profile restriction |
|---|---:|---|---:|---:|---|---|
| Tankō | 999 | no | 1 | 3 | — | all |
| Daiyōkai | 1002 | no | 0 | 1 | — | all |

### FT-04 — Druze Fireteams

**Types:** Duo, Haris  
**Anchor:** Druze has source `min: 1`.

| Member | Unit ID | Required | Min | Max | Counts as / comment | Profile restriction |
|---|---:|---|---:|---:|---|---|
| Druze | 379 | no | 1 | 3 | — | all |
| Arslan | 986 | no | 0 | 1 | `(Druze)` | all |
| Táowù | 1538 | no | 0 | 1 | `(Druze)` | all |
| Clipper Dronbot | 18 | no | 0 | 1 | `FTO` | **profile 5 only** |

### FT-05 — Mechanized Fireteam

**Type:** Duo

The current source has unusual raw required semantics: `SCARFACE` is `required: true, min: 1`, while `TRIPHAMMER` is also `required: true` but retains `min: 0`. Preserve those fields exactly rather than silently rewriting the chart into a different composition rule.

| Member | Unit ID | Required | Min | Max | Counts as / comment | Profile restriction |
|---|---:|---|---:|---:|---|---|
| Scarface | 380 | **yes** | 1 | 1 | — | Scarface component of composite selection |
| Triphammer | 1569 | **yes** | 0 | 1 | — | all current TAG profiles |
| Cordelia Turner | 380 | no | 0 | 1 | — | Cordelia component of composite selection |
| Motorized Bounty Hunter | 1565 | no | 0 | 1 | — | all |

Do not simplify the Triphammer row to `required: false` merely because its numeric minimum is zero; the source stores both values.

### FT-06 — Krakot Renegades Fireteams

**Type:** Duo

| Member | Unit ID | Required | Min | Max | Counts as / comment | Profile restriction |
|---|---:|---|---:|---:|---|---|
| Krakot Renegade | 756 | no | 1 | 2 | — | all |

### Wildcards

| Unit | Unit ID | Counts as / comment | Max | Profile restriction | Notes |
|---|---:|---|---:|---|---|
| Authorized Bounty Hunter | 49 | — | 2 | all | explicit Wildcard row |
| Brawler | 987 | `(Druze)` | 2 | all | explicit Wildcard row |
| Digger | 1568 | `(Druze)` | 2 | all | explicit Wildcard row |
| Rumbler Spec-Ops | 1925 | `Spec-Ops` | 1 | optional mode only | explicit Wildcard row |

Do not import additional Wildcards or Fireteam permissions from older Ikari references, JSA, Druze Bayram Security, Dashat, or another NA2 sectorial.

## Unit → Fireteam access index

| Unit | Fireteam | Types | Access | Profile restriction | Min–max / notes |
|---|---|---|---|---|---|
| Keisotsu | FT-01 | Haris/Core | native anchor | all | 1–5 |
| Tankō | FT-01 | Haris/Core | native | all | 0–1 |
| Wú Míng | FT-02 | Haris/Core | native anchor | all | 1–5 |
| Clipper | FT-02 | Haris/Core | FTO member | **profile 5** | 0–1 |
| Tankō | FT-03 | Duo/Haris | native anchor | all | 1–3 |
| Daiyōkai | FT-03 | Duo/Haris | native | all | 0–1 |
| Druze | FT-04 | Duo/Haris | native anchor | all | 1–3 |
| Arslan | FT-04 | Duo/Haris | counts as Druze | all | 0–1 |
| Táowù | FT-04 | Duo/Haris | counts as Druze | all | 0–1 |
| Clipper | FT-04 | Duo/Haris | FTO member | **profile 5** | 0–1 |
| Scarface | FT-05 | Duo | source required member | composite Scarface | min 1, max 1 |
| Triphammer | FT-05 | Duo | source required flag | all | raw min 0, max 1 |
| Cordelia Turner | FT-05 | Duo | native | composite Cordelia | 0–1 |
| Motorized Bounty Hunter | FT-05 | Duo | native | all | 0–1 |
| Krakot | FT-06 | Duo | native anchor | all | 1–2 |
| Authorized Bounty Hunter | Wildcard | permitted teams | Wildcard | all | max 2 |
| Brawler | Wildcard | permitted teams | Wildcard, counts as Druze | all | max 2 |
| Digger | Wildcard | permitted teams | Wildcard, counts as Druze | all | max 2 |
| Rumbler Spec-Ops | Wildcard | permitted teams | optional Wildcard | Spec-Ops mode | max 1 |

If this reverse index ever conflicts with the canonical Fireteam tables above, the canonical tables win.

## Optional-mode units

### Rumbler Spec-Ops

**Unit ID:** 1925 · **Slug:** `rumbler-spec-ops` · **Mode:** Infinity Spec-Ops · **Normal Ikari status:** optional only.  
The Fireteam chart exposes Rumbler as an explicit Wildcard (`Spec-Ops`, max 1) when the mode is enabled.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 28 | 1 | HMG, D-Charges, Pistol, CCW |
| 2 | 28 | 1 | AP Spitfire, D-Charges, Pistol, CCW |
| 3 | 23 | 0 | MULTI Rifle, Pistol, CCW; Specialist Operative, GizmoKit |
| 4 | 26 | 0.5 | AP Combi Rifle, D-Charges, Pistol, CCW; Hacking Device |
| 5 | 23 | 0 | MULTI Rifle, Flash Pulse, D-Charges, Pistol, CCW; Forward Observer |
| 6 | 23 | 0 | AP Combi Rifle, D-Charges, Pistol, CCW; Paramedic, MediKit |

### NA2 Team-Ops

**Unit ID:** 1939 · **Slug:** `na2-team-ops` · **Mode:** Team-Ops · **Normal Ikari status:** optional only.  
Contains Rumbler-1, Rumbler Heavy and Gort SpecBot Team-Ops profiles. It is not counted as an ordinary matched-play Ikari roster entry and is not automatically substituted for Rumbler Spec-Ops in the Fireteam chart.

## Character and source constraints

- Both **Yojimbo** roster entries carry the source note that there can only be **one Yojimbo in each Army List**. Treat the foot and motorized identities as alternatives, not two independent characters.
- **Kiiutan Imposters** retain the source `AVA 1*` note shared globally with Jaan Staar. Jaan Staar is not a standard Ikari roster entry, so this normally does not create an additional Ikari roster choice; the source restriction is recorded for identity consistency.
- The current Ikari snapshot's top-level `relations` array is empty. Do not invent relation groups that are not present; use the explicit unit notes above where the source carries the restriction directly.

## Reinforcements boundary

Army links Ikari Company to Reinforcement roster ID **999**. Reinforcement-only profiles, AVA and Fireteam permissions remain outside this Main reference. Do not merge Reinforcement Fireteam permissions into the Main chart above.

`999` is also the unit ID of Tankō Zensenbutai; the matching number is coincidental because unit IDs and reinforcement-army IDs occupy different namespaces.

## Derived tactical index

This section is analytical and non-authoritative; the source profile data and Fireteam chart above take precedence.

| Block / tag | Strong Ikari candidates |
|---|---|
| Long-range attack | Scarface; Triphammer; Wú Míng AP HMG; Daiyōkai HMG; Al Fasid HMG; Rui Shi |
| Long-range ARO | Tankō ML; Clipper FTO (+1B ML); Brawler HRL/MSV2 sniper; Sierra TR; Pangguling TR; Armand sniper |
| Mid-range attack | Daiyōkai; Wú Míng; Druze; Karakuri; Lù Duān; Rui Shi; Arslan |
| Close assault | Yojimbo; Krakot; Tankō; Ninjas; Diggers; Desperadoes; Yuan Yuan |
| Specialist | Keisotsu FO/Paramedic/Hacker; Druze Hacker/KHD; Brawler Hacker/Engineer/Doctor; Wardriver; Tokusetsu; Pathfinder; Karakuri FO; Táowù; Cube Jäger; Ninjas; Bashi; Cordelia |
| Cheerleader / cheap orders | Keisotsu; Fugazi; Warcor; Authorized Bounty Hunters |
| TAG + support | Scarface + Cordelia; Triphammer + Tokusetsu/Brawler Engineer/Yáozăo |
| REM + support | Sierra/Pangguling/Fugazi/Lù Duān/Rui Shi/Pathfinder/Clipper + Tokusetsu/Brawler Engineer |
| DZ defense | Sierra; Pangguling TR; Tankō ML; Brawler ARO profiles; Clipper; Warcor |
| Midfield defense | Ninjas; Kiiutan; Krakot; Diggers; Táowù; Bounty Hunters |
| Midfield specialist | Ninja FO/Hacker/KHD; Táowù; Bashi Specialists; Karakuri FO |
| Warband | Yuan Yuan; Desperadoes; Yojimbo; Krakot; Diggers |
| Airborne troops | Yuan Yuan; Cube Jäger; Bashi Bazouks |
| Enemy-DZ attacker | Yuan Yuan; Bashi; Cube Jäger; Kiiutan; Ninjas |
| Network projection | Druze Pitcher; Pangguling/Fugazi/Rui Shi/Pathfinder Repeaters; Wardriver Cybermine/Disco Baller |
| Vision control | Yuan Yuan/Desperado/Yojimbo/Al Fasid smoke; Rui Shi/Brawler MSV2 can exploit it |
| Hacker | Druze; Brawler; Wardriver; Keisotsu; Ninja |
| KHD | Druze; Ninja |
| Tech-counter | Pathfinder Sensor; Tokusetsu/Brawler/Cordelia Engineers; Yáozăo servant support |
| Group-2 efficient | Warcor; Fugazi; Pangguling EVO/TR; Sierra TR; airborne Irregulars; Bounty Hunters |

## Source-normalization and validation notes

- Standard roster count is **36 normal entries + 2 optional-mode entries**.
- Generic `merc-*` catalogue objects with empty `factions` arrays are excluded even though the aggregate dataset contains them. Explicit faction-`904` mercenary/guest entries are retained.
- Source `DUO: 256` is normalized as effectively unlimited Duos.
- Keisotsu, Wú Míng, Tankō, Druze and Krakot anchors use positive source `min` values despite `required: false`; those minimums are preserved.
- Mechanized Fireteam has unusual source semantics: Scarface is `required: true, min: 1`; Triphammer is `required: true, min: 0`. Both raw facts are preserved rather than normalized into a guessed rule.
- Clipper FTO access means **profile 5 only**. Profile 1 has Guided but is not the FTO loadout; profile 5 is FTO with Missile Launcher (+1B) but lacks the Guided skill in the current source.
- Pangguling profile 4 is labelled FTO in its unit data but the current Ikari chart has no Pangguling row; no Fireteam access is inferred.
- Brawlers and Diggers are explicit Wildcards with `(Druze)` source comments. Authorized Bounty Hunters are explicit Wildcards without a counts-as comment.
- Rumbler Spec-Ops is an explicit Wildcard only when the optional Spec-Ops mode is enabled.
- Disabled TurtleMek subordinate entries are not counted as independent roster selections.
- Main and Reinforcement roster `999` remain separate.

## Provenance

- Sectorial ID: `904`
- Parent faction: Non-Aligned Armies (NA2)
- Corvus Belli Army-derived revision: `7.26246.159`
- Source commit: `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b` (`army: N5.3 + ITS18`)
- Army data changed on: 2026-09-03
- Versioned source: `n5/ikari/7.26246.159.json`
- Versioned source blob: `20d1c5d0c981606515e95c08d02f48b921b92b76`
- Aggregate source: `n5/ikari/ikari.json`
- Aggregate source blob at pinned commit: `e8cd8b1cb702f4ea7dacb38e9fb25c39d41f91d2`
- InfinityDB commit: `4e2662be3f43387fbae42b3790a711b3e98570c4`
- Rules baseline: N5.3 + N5 FAQ v0.1
