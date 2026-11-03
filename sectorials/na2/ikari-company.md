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

## Tactical research — Ikari Company (reviewed 2026-10-23)

**Use this after the verified roster/Fireteam reference above.** Tactical opinions come from transcript-reviewed analysis and games. **[P1]** is a September 2025 experienced-player review and generally more useful for *how Ikari plays* than the N5 launch reaction **[V1]** or N4 retrospective **[P2]**; nevertheless, exact N5.3 Army 7.26246.159 profiles and the canonical chart above always win. Do not port JSA/Yu Jing/NA2 Fireteam rights, pre-update point values or early-N5 Guided interactions into Ikari.

### At a glance — what works and why

| Plan / block | Buy it for | Failure mode and decision rule |
|---|---|---|
| **Cheap regular-order core + many attacks** | 9–12pt Keisotsu, an economical Wú Míng attacker, and multiple cheap fast threats mean another piece can take over after the first dies. Copper calls Ikari **wide rather than deep**: several good-enough gunfighters and attackers instead of one perfect solution. [P1] | Hard 15-trooper ceiling and too many Irregular warbands can choke Orders; identify two priority attackers and keep enough Regular Orders to run them. |
| **Wú Míng Core/Haris** | **AP HMG 33/1.5** fights armor; **HRL/E/M Carbine 23/1.5** deters lane crossing; **E/M GL 27/0 SWC** attacks threatening targets without a straight face-to-face. **TinBot Firewall (-6) 22/0** and Brawler Hacker can protect/use the formation. [P1, V1] | BTS3 and Hackable; full Core can become an expensive single point of failure. Shorter team if room/Orders matter more than extra Fireteam dice. |
| **Tankō + Daiyōkai Haris OR Keisotsu ARO Core** | **Tankō ML 26/1.5** threatens distant lanes, inexpensive Blitzen/Disco Baller profiles cover corners; Daiyōkai's NCO and 2W+NWI support mobile, mixed-range pressure. [V1, P1] | **Only one Tankō in a Keisotsu team**; old N4 “missile Tankō in cheap link gets huge bonuses” expectations are outdated. Limited Cover/Impetuous Tankō still need a careful ARO lane. |
| **Druze KHD + small Duo/Haris** | KHD **23/0 with Pitcher and D-Charges**, Warhorse, X-Visor: network projection, hacker hunting and button pushing. Pair with a Digger or Brawler to get helpful Fireteam roles while avoiding an expensive Druze-heavy group. [P1, V1] | KHD **does not itself provide ordinary Spotlight**; include HD/FO where needed. Ikari's Druze family is **Duo/Haris, not Core**. |
| **Warband/motorcycle pressure** | **Motorized Yojimbo 20/0**, Desperadoes 7–9, Yuan Yuan from 6 and Regular Krakots 14+ bring smoke, trades, flanking and close combat. Smoke can set up Brawler MSV2 or Rui Shi MSV2 shooting. [V1, P1] | The fast models are vulnerable when isolated; their Irregular/Impetuous Orders and S4 bike lanes demand a budget. Do not use them all because they are individually cheap. |
| **Objectives over tabling** | **Ninja FO/HD/KHD**, Karakuri FO, Pathfinder FO, Druze specialists, cheap Keisotsu FO and airborne Bashi specialists offer different approaches. [P1, V1] | **Weak midfield Camo presence** beyond the Ninja; several specialists must walk from the DZ. Reserve a protected objective-taker before spending all points on fights. |

**Default construction test:** Can the list (1) deploy safely going second, (2) clear a long ARO, (3) reach a midfield button, (4) threaten armor/hackers with AP/E/M/para or hacking, and (5) keep a useful second attacker after the first fails? **[P1]** recommends designing for going second and roughly **three Irregular models** as *his* preference—not a rule; adapt by mission and Orders.

### Strong unit choices; preserve disagreements

- **Wú Míng versus Daiyōkai:** Copper [P1] prefers Wú Míng **33pt AP HMG** as the primary gun because it saves **17pt** against Daiyōkai HMG (50pt) *and* shoots AP, while the Wú Míng HRL and E/M GL offer cheap follow-ups. **Opposing case:** Daiyōkai has **ARM5, NWI, NCO, BS Attack (SR-1)** and better independent fighting/CC options, and makes a **Tankō Haris**; it is not simply a worse AP HMG. Pay extra if the NCO order and Haris mobility matter. [V1, P1, P2]
- **Armand Le Muet MSV1 sniper (34/1.5) versus disposable AROs:** Copper [P1] considers him unusually valuable: **Mimetism (-6)** plus MSV1, forward deployment, MULTI sniper, symbiont transmutation, backup pistols/CC make him both lane controller and active sweeper. **Counterweight:** he costs ~3 Keisotsu and cannot replace specialist/fast-trade coverage; the cheaper **33pt Minelayer** profile trades MSV for an extra defensive mine. [P1]
- **Tankō:** The **18–19pt Blitzen/Disco Baller** options are robust affordable close support, with hard CC threat; **26pt ML** is a major ARO commitment and may eat 1.5 SWC that could fund another gun. A Tankō is not automatically an advantaged gunfighter just because it joins cheap Keisotsu. [V1, P1]
- **Karakuri (31–38; AVA2, not Fireteam-linkable in Ikari):** ARM3/BTS6/STR3 with **Immunity (Enhanced)**, FO and GizmoKit means an independent specialist can absorb danger while moving to an objective. **Mk12** pushes direct midrange gunfights; **MULTI Rifle** broadens ammunition; **E/Mitter** offers technical suppression. Expensive relative to button-only alternatives, slow starting position, and cannot borrow JSA's different Karakuri Fireteam access. [P1, V1, P2]
- **Keisotsu (9–18):** 9pt AP-rifle filler / 9pt LT costs **0.5 SWC**; 10pt combi LT also 0.5; 11pt FO adds a cheap mission Order. The **16pt ECM: Hacker (-6) + CrazyKoala** hacker is useful when Druze Pitchers project the hacking network. The **12pt Thunderbolt BS Attack (-3)** can complicate ARO dice from a Core, but does not become a premium active HMG. [V1]
- **Brawler hacker (16/0.5), MSV2 sniper (25/1.5), HRL (15/1.5):** Wildcard utility across fireteams: native **Sixth Sense** hacker and TinBot-supported Wú Míng group can punish repeaters/Stealth; MSV2 shoots through smoke; HRL adds a cheap long-lane deterrent. **Disagreement:** [V1] favors the new cheaper Keisotsu hacker and considers Brawler hacker less essential; [P1] values Sixth Sense and supporting the Wú Míng team. SWC/desired lane decide.
- **Yojimbo:** [V1] rates the **motorized identity** highly for smoke launcher, CrazyKoala/Minelayer, Mimetism (-3), NWI, CC and mobility. **Foot identity** may handle stairs/tight spaces but gives up the motorcycle's reach; V1 strongly favors motorized. **Only one Yojimbo total**, across the two identities. Desperadoes compete with motorized bounty hunters for Irregular slots: Desperado 7pt smoke/chain rifle is usually more efficient for trade/smoke; **Motorized Bounty Hunter** brings alternate Booty/Red Fury/riotstopper utility, including Mechanized Duo eligibility. [V1, P1]
- **Bashi Bazouk T2/AP Boarding Shotgun (14) vs Cube Jäger:** Bashi can appear from a flank to trade into a hardened target or Lieutenant; cheap Specialist Operative variants solve late objectives. Cube Jäger (15–18) is a Parachutist/Paramedic and different classifieds tool. Copper [P1] favors Bashi's kill potential; [V1] also prefers a Bashi specialist over Jäger for many missions, but Jäger wins where **Paramedic** or precise recovery is needed.
- **Arslan versus cheap Lieutenant:** Copper [P1] dislikes **35pt Arslan** as an expensive short/midrange gun for what it buys; **9pt Keisotsu LT** or **15pt Brawler LT** hides more cheaply. **Opposing case:** Arslan's WIP13, MSV1, NWI, Disco Baller and ability to fight are genuine upsides; is the list already equipped to protect a fighting LT? **Táowù Chain of Command (21/0)** can insure, but has an opportunity cost. [V1, P1]
- **Al Fasid (44–50):** ARM5/BTS6, Sixth Sense, Minelayer, Albedo and HMG+smoke/HRL make it a credible **standalone** anchor with area denial. Copper [P1] finds it squeezed out by cheaper **linkable** Wú Míng guns/HRL. [V1] is also skeptical of its inability to link despite the attractive profile. Worth reconsidering when independent fire support, layered smoke and no Fireteam order dependency are valuable. **Warhorse is not synonymous with all hacking attacks being impossible**; apply actual N5 rules.
- **Krakots versus more Irregular warbands:** Unlike Desperado/Yuan Yuan, Krakots are **Regular, Impetuous**, with Forward Deployment, Super-Jump and close combat; useful to preserve the Regular order pool and threaten midfield. Their direct fighting is relatively short-ranged; do not spend many Orders reaching an overprotected target. [V1, P1]

### TAGs, REMs, Vehicles — comparative tactical value

| Choice (current Ikari only) | Why it works | Why/when to skip |
|---|---|---|
| **Scarface & Cordelia** (76–80 / 1.5 *composite*) | Scarface's AP HMG or AP Spitfire, STR3/ARM7, Tactical Awareness, plus bundled Engineer Cordelia and TurtleMek specialist, supply a credible sustained attack package. [V1, T1, P2] | Mandatory ~quarter-list package vs **33pt AP HMG Wú Míng** + specialists/cheap threats; Cordelia cannot repair a TAG left exposed deep in enemy territory. V1's hosts and [T1] disagree on how often it deserves a slot. |
| **Triphammer** (48–53 / 0–1.5) | Independent budget TAG with Tactical Awareness, ARM7, transmutation, TurtleMek specialist and Booty; **48/0 HRL+heavy shotgun+Panzerfaust** preserves scarce SWC, **AP Spitfire** pressures armor. [T1, V1] | Ordinary BS13 and BTS3, no superior negative-shooting mods; sometimes a Wú Míng plus extra orders performs better. **Mechanized Duo** has a Scarface required source row; **do not assume Triphammer can create a legal Duo alone**. |
| **Rui Shi** (23/1 Spitfire MSV2; 21/0.5 Red Fury MSV1 + Mine Dispenser) | The fast **MSV2 Spitfire + smoke + EVO support** is a genuine way to sweep Mimetism/hidden ARO lanes. Red Fury variant invests in objective-area mine coverage rather than just direct killing. [V1, Y1] | Fragile ARM1/STR1, repeater makes hacking relevant; **not linkable in Ikari**, unlike possible cross-sectorial build-outs; EVO is optional unless it improves more than one planned REM/airborne job. V1 favors MSV2 but sees value in both. |
| **Lù Duān** (24 Mk12/FT or 20 Thunderbolt/E/M) | Holoprojector, MSV1, Surprise Attack, BS Attack (+1B), E/M Mine: deceptive angle attacker/defensive trap, with an E/M Carbine option for technological targets. [V1] | **Contested:** V1's JSA-playing guest says N5 lost its old Holomask, Minelayer and deployable repeater and weakened its distinctiveness; host values the new B4 Mk12/strong templates. Use *current* Holoprojector and mine profile only—**no Minelayer or deployable repeater on present Lù Duān**. |
| **Pathfinder** (14 FO; 17 TacAware FO) | AVA1, Sensor+FO+Repeater, tactical movement and classified/objectives; excellent answer to Ikari's thin midfield specialist presence. [V1, P1] | Soft STR1 and not Fireteam-linkable; mission may demand a hidden Ninja or resilient Karakuri instead. |
| **Clipper Guided** (16/1.5) | Backfield indirect threat if Druze HD/Pitcher + Keisotsu/Brawler hackers, FO and repeater order economy make Targeted useful. [V1, P1] | **NOT Fireteam eligible**: this is non-FTO profile **1**, with Guided. V1's early-N5 video incorrectly argues it can join Druze Haris and get the Guided special die. Current roster/chart prohibits it. Guided has additional attack/Reset/order friction; do not build the list around an illegal burst combo. |
| **Clipper FTO** (19/1.5) | **Profile 5 ONLY** enters Wú Míng or Druze teams; direct missile launcher (+1B) brings an attack/ARO weapon, **not Guided**. | Costs more, eats SWC and has no Guided; select this for *direct lane coverage*, not off-table missile exploitation. |
| **Sierra TR** (23/1 HMG; 18/0 Thunderbolt +1B) | Compact reactive deterrent, 360° and Total Reaction; choose Thunderbolt when SWC is already going to Wú Míng, Tankō or Rui Shi. [V1, P1] | Cannot withstand repeated engineered hard-counter attacks; may be more useful concealed until turn 2/3 than as first-turn sacrifice. |
| **Pangguling** (8 Baggage/Repr; 15 EVO; 19 TR rifle; 12 FTO-labelled) | 8-point Regular Baggage+Repeater/Deactivator supplies ammunition support and network coverage; EVO improves appropriate Rui Shi/Sierra/airborne plans; TR profile offers extra defensive fire. [V1, Y1] | **FTO label ≠ actual Fireteam access**: **no Ikari Pangguling Fireteam row**. Larger S4 model crowds DZ; EVO isn't mandatory just because it is cheap. |
| **Fugazi** (7) | Fast Regular Flash Pulse Repeater and Mimetism (-3), cheap order/network defence. | **AVA1** here; do not apply PanO/other sectorials' AVA or assume multiple Fugazis. |
| **Yáozăo and TurtleMek** | Servant Yáozăo extends Tokusetsu/Brawler support reach; TurtleMek ancillary specialists embedded with TAGs can act on objectives. | Peripherals do **not** generate separate Regular Orders; respect parent/composite restrictions. |

**Vehicle (VH) audit:** Current 36-entry Ikari **Main roster has no troop with VH type**. **Yojimbo motorized, Desperadoes and Motorized Bounty Hunters are WB/LI motorcycles, not VH**; no actual Vehicle-only N5 tactics/profile/Fireteam should be imported. **TAGs: exactly Scarface composite and Triphammer**. REMs: **Sierra, Pangguling, Fugazi, Lù Duān, Rui Shi, Yáozăo, Pathfinder, Clipper**, plus embedded TurtleMeks; all are counted by the existing roster/peripheral contract.

### Conflicting testimony and corrections to retain

1. **Faction strength:** [L1] December 2024 hosts initially considered post-N4 Fireteam restrictions a major Ikari weakness, revising their assessment slightly when accounting for cheap durable guns. [P1] September 2025 specialist argues those same cheap Wú Míng, Tankō and Irregular/Regular threats create **redundancy**, and no single piece must win the game. Treat placement/tier as dated opinion, not a settled win-rate fact.
2. **Daiyōkai/Al Fasid versus Wú Míng:** [V1] launch discussion values Daiyōkai HMG and [P2] N4 runs Daiyōkai/Tankō as primary guns. [P1] explicitly drops expensive Daiyōkai/Al Fasid from optimized lists because **AP Wú Míng 33** and cheaper HRL cover more jobs per point. Both arguments have conditional validity (NCO/ARM versus AP/cost/team).
3. **Guided commitment:** [V1] highlights Druze Pitcher and purported linked Guided Clipper; [P1] prefers **SWC-free Wú Míng E/M GL** more often because Guided Clipper consumes scarce SWC and setup orders. **Current N5.3 legality resolves the earlier premise**: Clipper Guided **not linkable**.
4. **Rui Shi versus Lù Duān:** [V1] favors MSV2 Spitfire smoke-shooting Rui Shi as the reliable job; equally discusses Lù Duān's new deceptive high-burst toolkit but guest mourns old repeater/minelayer and has not settled on performance. Do not present a unanimous ranking.
5. **Scarface versus cheaper packages:** [V1]/[T1] acknowledge useful AP/TAG fighting; [P1] centers inexpensive infantry/warbands, while [P2] previously relied on Scarface in a TAG-led tournament plan. It is a *style/mission tradeoff*, not settled inferiority.
6. **“Strong all-purpose” does not mean unlimited composition:** Ikari cannot create a Keisotsu Duo, Wú Míng Duo or Karakuri link from the current chart; has **Keisotsu/Wú Míng Core or Haris, Tankō Duo/Haris, Druze Duo/Haris, Krakot Duo, Mechanized Duo**. Fireteams: **1 Core + 1 Haris + unlimited permitted Duos**. Never import other JSA or Yu Jing links.

### Best videos/podcasts, what to watch, transcript status

**Direct Ikari first**
- **[P1] WIP12 [E191: Ikari with Copper](https://open.spotify.com/episode/0XooAPvaG5RXEX9wUgsDvy) (2025-09)** — **Podcast MCP transcript reviewed**. Best practical source: flexibility/order management (~27–30m), Armand (~32–36m), Wú Míng/EM GL and Brawler (~42–48m), Tankō and Fireteams (~51–60m), bad/ugly on Daiyōkai/Arslan/Al Fasid (~63–73m), specialist & Lieutenant limitations (~76–81m).
- **[V1] Infinity the Dante + Josh (Loss of Lieutenant), [Ikari Company N5 Initial Reaction — Biggest Glowup in N5???](https://www.youtube.com/watch?v=6kZ2YeFDoNI) (2025-01)** — **YouTube MCP transcript reviewed**. Best profile-by-profile counterview, including early-N5 Fireteams, cheap Keisotsu, Rui Shi vs Lù Duān, TAGs, REMs; **linked Guided Clipper assumption is obsolete/wrong**.
- **[L1] Loss of Lieutenant, [Episode 132: N5 Faction Tierlist — Ikari at 11:40](https://www.youtube.com/watch?v=RCf46MeSE84) (2024-12)** — **YouTube and Podcast MCP transcript reviewed**; useful skeptical launch take on AROs, linked bonuses and revised optimism. Not a current ranking.
- **[P2] WIP12 [E163: Cobraprime takes Ikari to IGL](https://open.spotify.com/episode/6sA5fiWOLSIILRw7DO06tv) (2024-07)** — **Podcast MCP transcript reviewed**. Competitive N4 historical baseline: Scarface, Daiyōkai/Tankō, Yojimbo and surviving obvious Lieutenant assassinations; **not N5.3 validation**.
- **[V2] Tabletop Throwdown, [Akial Interference: Tunguska vs Ikari](https://www.youtube.com/watch?v=G6Y6QgEp1Lg) (N5)** — **YouTube MCP transcript reviewed**. Practical list interaction with Scarface, Brawlers, Pathfinder, repeaters; *single game*, not a rankings survey.
- **[V3] Champion of Terra, [Ikari Company vs Svalarheima](https://www.youtube.com/watch?v=EcyodGckZUU) (N5)** — **YouTube MCP transcript reviewed**. Karakuri, Tankō and Wú Míng mission play; game specifics should not be overgeneralized.

**Shared TAG / REM analysis (do not import the other faction's roster/Fireteams)**
- **[T1] Loss of Lieutenant, [Episode 142 — N5 TAG Tier List](https://www.youtube.com/watch?v=dZo_gQWQYSY)**; [podcast episode](https://open.spotify.com/episode/1h5CJfZC5zBPxdg66o7xIN) (2025-04) — **YouTube and Podcast MCP transcripts reviewed**; Scarface ~2h20, Triphammer ~2h23–2h27; supports conflicting assessments of Scarface's bundled cost and the 0-SWC Triphammer.
- **[Y1] Robert Shepherd, [N5 Imperial Service Faction Focus](https://www.youtube.com/watch?v=Yskl69PVzWA) (2025)** — **YouTube MCP transcript reviewed**; MSV2 Rui Shi + smoke/EVO concept, and overlapping Wú Míng cost/EM-Carbine reasoning. **ISS-specific buffs, Fireteams and support characters do not transfer.**
- **[Y2] Robert Shepherd, [N5 Yu Jing Faction Focus](https://www.youtube.com/watch?v=mn4yHSNxsnA) (2025)** — **YouTube MCP transcript reviewed**; Pangguling EVO/Marksmanship, remote + engineer and specialist support; **not a substitute for the Ikari AVA/legality chart**.
- **Infinity the Dante, [Qapu Khalqi Faction Focus — The Sky is Falling!](https://www.youtube.com/watch?v=z4kV-SFZ5Uw) (N5)** — **YouTube MCP transcript reviewed**; Scarface/Triphammer in another mercenary-linked setting, but **QK mechanized formations and support differ**.
- **[N5 Ikari community video/podcast index](https://forum.corvusbelli.com/threads/n5-recap-ikari-company-tacticas.43626/)** — curated third-party discovery and episode links; secondary, not Army rules.

**Source caution:** None of these opinions override the pinned N5.3 factual tables above. Some transcripts are speech-to-text and misrender unit names, weapon names, timestamps or current profiles; tactical conclusions were reconciled with the local reference rather than transcribing them as rules.

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

## Warband cheap trading / order economy — N5.3

**Yuan Yuan Chain+Smoke6/0 / DA CC7/0, AVA4** is elite *cheap* AD pressure: Combat Jump(PH11) succeeds **55%** before any valid +3 EVO, ordinary Parachutist flank avoids landing roll but not ARO. **Motorized Bounty Hunter8 BSG+Riotstopper /9 SMG+Chain-colt** is a 20-15 bike without smoke. **Bashi SMG12/T2 BSG14** is an Irregular Holoprojector Parachutist with different tempo. Buy one 6pt Yuan if it can trade away a critical defender; **do not count Irregular and Impetuous Orders as pooled Regular**. Check Ikari LT and CoC alternatives separately.

[Current cross-faction warband apex/value, opponent counters, Lt/CoC packages](../../notes/list-building/warbands-and-cheap-trading-units-apex-value.md). This faction's own pinned profile and Fireteam rows control legality.

## TAG tactical cross-reference (2026-10-23)

**Triphammer** is the roster's budget TAG: choose its AP Spitfire/short-range loadout to pressure a side lane while Ikari retains inexpensive midfield and mission bodies. Its damaged-state payoff is **variance**, not guaranteed efficiency. Count legal Mechanized Fireteam members and the Engineer/support cost before calling a low price 'free' armor.

For the two-tier **apex/points-value** comparison, TAG counterplay, matchup matrix and direct transcript sources: [N5.3 TAG field guide](../../notes/list-building/tags.md). Treat current profiles, points/SWC and canonical Fireteam data above as authoritative.

## Hacker and KHD tactical cross-reference (2026-10-23)

**Druze KHD+Pitcher 23/0 vs HD+Pitcher 25/0.5** is the main hacker-or-heavy choice: the KHD removes enemy Hackers, the HD stops ordinary TAG/HI with Carbonite/Oblivion. **Brawler HD 16/0.5** and **Keisotsu HD 16/0.5 with ECM: Hacker(-6)** are budget normal devices; **Ninja Hidden KHD26/0** supplies mission-winning specialist surprise, not a stronger backfield network. **Wardriver** is rarely better pure value than one Druze KHD. **Why:** combine the actual **Druze Pitcher / Baggage / Repeater network** with one anti-Hacker and one anti-heavy program; Ikari's weapon-rich HI need screens and don't inherit Qapu Fireteams.

See the [cross-game apex/value Hacker/KHD tier guide](../../notes/list-building/hackers-and-killer-hackers.md). **The sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative; device upgrades are profile-specific.**


## Cheerleader / Order-generation tactical cross-reference (2026-10-23)

See the N5.3 [cross-game apex/value rankings and transcript-backed competing assessments](../../notes/list-building/cheerleaders-and-order-generators.md). The current roster and official Fireteam definitions above remain authoritative; unit access/cost may differ from vanilla.

- Cheap Authorized/Motorized Bounty Hunter — usually a Regular trading body with Booty, not always a protected static S2 Order; exact bike/profile/Fireteam legality varies.
- Keisotsu — inexpensive S2 Regular bodies, line-FT material and possible utility upgrades; optimize the cheapest legal role rather than premium heavy guns.
- 7pt Fugazi — fast Flash/Repeater bot; cheap Regular Order plus hacking relay if available.
- Karakuri — durable multiple-role attacker/specialist, not a minimal-cost backline cheerleader; compare total Order demand.
- 3pt Warcor — very useful Irregular Flash ARO/cheap screen, NOT an ordinary transferable Order.

**Selection rule:** Count deployed, transferable Regular Orders per Combat Group, not total models or restricted bonus Orders; choose the lowest-cost protected Regular profile that *also* contributes a relevant Repeater, Baggage, Fireteam, template, ARO or Specialist job. Check Group slots and DZ hiding space before buying a third large-base REM or replacing a needed scoring piece.


## ARO apex/value cross-reference (2026-10-23)

See [Best ARO Units in N5.3 — apex, cost-value, Hidden Deployment, reactive traps, opposed podcast views](../../notes/list-building/aro-units-apex-and-value.md). **Only the legal roster above** establishes options, exact costs/AVA, upgrades and Fireteam permissions in this army.

- **Authorized Bounty Hunter cheap body** — small-base template/Panzerfaust or close ARO if profile equipped, useful only in legal team/roster
- **Ninja hidden/camo** — anti-impersonation or corridor trap if positioned near scoring; may be more valuable unrevealed for own active turn
- **Sierra Thunderbolt TR** — 18pt/0SWC where authorized, all-arc cheap regular ARO and Engineer-restorable lane
- **Fugazi Flashbot** — 7pt Regular cheap Flash/Repeater tax; not substitute for anti-armor hard ARO
- **Druze Fireteam weapon/EM** — durable midlane or utility link option where current source permits; multiple roles beat pure unused sniper SWC

**List test:** a strong ARO consumes enemy Orders by forcing Smoke, rerouting, poor range, discoveries or risky trades. A robust list normally prefers *serial, different* defenders—a cheap visible or marker/template screen, a covered second gate, and a preserved attack/scoring unit—rather than two adjacent visible snipers. Plan for opponent pie-slicing, AD, anti-camo, hacking and recovery; evaluate whether extra SWC is better spent on mission attackers.

## Doctor / Engineer / Recovery cross-reference (2026-10-23)

**Scarface & Cordelia (76–80pt combined)** brings a TAG and its Engineer in one mandatory composite purchase, unusual direct access to a valuable STR casualty; still protect Cordelia and a safe recovery lane. **Tokusetsu Doctor14 / Engineer14 WIP13 + Yáozăo3** cover **Karakuri Remote Presence/other STR** or VITA respectively, with token rerolls only on qualifying targets. Cheap recovery network can outperform taking extra premium doctors. [Recovery support tiers, probabilities and transcript disputes](../../notes/list-building/doctors-engineers-and-recovery-apex-value.md).

## Close-combat assassins and counter-CC — N5.3 (2026-10-23)

**Yuan Yuan6/0 CC22 + Smoke + Combat Jump(PH11)/Parachutist** is outstanding cheap flank *trade*, but **Combat Jump is only 55% base** without eligible landing bonuses and a successful deployment **is not yet base contact**. **Daiyōkai46/0 CC21 MA2 AP+DA** is a durable ranged/short-fighting HI, not a Shinobu substitute; **Tokusetsu** score/repair. **Scarface & Cordelia** form a **TAG composite**, so Scarface CC22/Berserk does not belong in 20–30pt foot-assassin ranking. Use Yuan Yuan to disrupt rear defenders while guns and HI exploit revealed angles. [N5.3 melee apex/value and counter-CC guide](../../notes/list-building/dedicated-close-combat-assassins-apex-value.md).

## Anti-TAG / Anti-HI without hacking — N5.3 (2026-10-23)

**Cube Jäger15 Monofilament Parachutist /18 E/Mitter+Mono** has outstanding one-target ceiling for the cost, but requires an actual legal flank/contact and contributes an Irregular Order. **Tankō18 Blitzen+Mono**, **Wú Míng19 E/Marat**, **Táowù19 E/Marat**, **Lù Duān20 E/M Carbine+Mine**, and **Druze21 Panzerfaust** offer near-budget deterrence. **Wú Míng33 AP HMG** is sustained lethal B4 AP; **Scarface+Cordelia76** is TAG-scale investment. Yuan Yuan6 Smoke is delivery/cheap trade, **not** intrinsic E/M or Panzerfaust. [Non-hacking anti-armor apex/value, E/M and AP+EXP comparison](../../notes/list-building/anti-tag-anti-heavy-infantry-non-hacking-apex-value.md).

## N5.3 objective holding, zone domination & carried-objective choices

**Karakuri FO31/0 (AVA2)** gives one of the game's strongest actual **STR3/Enhanced-Immunity 0SWC Supply Box carriers**, with Heavy Shotgun/Chain Rifle/Panzerfaust. It remains a genuine FO while keeping objective behind terrain; **35/0 MULTI or38/0 Mk12** are better only if shooting pays. **Daiyōkai46/0**, ARM5 W2+NWI/NCO, and **Al Fasid HRL44/1.5** offer heavyweight *zone VP and ARO*, but are **not automatically Supplies Specialists**. **Yojimbo/Warband Smoke** covers transfer/extraction; **Rui Shi MSV2** hunts camo. **Disagreement:** Karakuri + cheap backup Engineer/Smoke holders protect the box better than using a pricey HMG hero to stand on an exposed console; when mission is pure quadrant scoring, Daiyōkai's 46pts can flip zone faster.

[Cross-game holding and carrier apex/value, scenario rules and transcript disagreements](../../notes/list-building/objective-holding-zone-domination-and-carriers-apex-value.md). Use pinned local roster/Fireteam chart.

## Anti-Tech — enemy visors, Mimetism, markers and Impersonation (2026-10-23)

**Pathfinder FO/Sensor** is Ikari's cheap **Camo/Hidden** sweep and utility REM; **Rui Shi MSV2 Spitfire23/1** or **Brawler MSV2 MULTI Sniper25/1.5** is for direct anti-Mimetism shooting. **Tankō Disco19/0** and **Wardriver Disco16/1** are actual anti-enemy-MSV/Marksmanship *passage* tools; ordinary Smoke from Yuan Yuan/Desperados/Al Fasid is not reliable against MSV2. **Counter:** the Brawler and Rui Shi can themselves be shut down by White Noise/Albedo; preserve a conventional gun/cheap screen and do not assume all Tankō variants carry Disco.

[Full anti-tech N5.3 apex/value, exact mechanics, matchup selection and opposing transcripts](../../notes/list-building/anti-tech-msv-mimetism-camo-impersonation-apex-value.md).

## N5.3 peripheral / synchronized / multi-body apex-value update

**Ikari** gets primarily **Servants and Ancillary**, not imported Nomad Puppetactica. **Yáozăo Servant3/0** extends engineer/doctor contact to expensive Karakuri/O-Yoroi on distant flank; one servant patient per Order, no extra Order generation. **Scarface+Cordelia** is a composite pair with Cordelia an actual independently placed Engineer where roster says, unlike synchronized bots. **Karakuri31/0 is a separate 3STR FO model with its own Regular Order** (not multiple G:Jumper Proxies sharing one), excellent holding a scored position, and **Daiyōkai46/0** another independent hard model. **Yojimbo CrazyKoala** is deployable equipment, **not a Pupnik or autonomous live shooter**. **Counter:** spend 3pt servant if saving recovery movement is the need; buy 19pt Yojimbo to create passive smoke/Koala corner denial, not to multiply target attacks like Chimera+3 Pupniks19 elsewhere.

[N5.3 Peripheral & Multi-Body apex/value tiers and transcript debates](../../notes/list-building/peripheral-synchronized-multibody-apex-value.md). Pinned source roster/Fireteam restrictions remain authoritative.

## Mission performance — battle-report evidence (2026-11-01)

| Mission(s) | Tested composition / scoring mechanism | Evidence |
|---|---|---|
| **Akial Interference / Classifieds** | Armand Le Muet sniper + Brawler Hacker, Wu Ming/TinBot and cheap Yuan Yuan/Desperado/Tanko can open diverse missions, but ensure specialist variety. | [#185](../../notes/battle-reports/181-190-n5-battle-report-tactical-analysis.md) |
| **Area of Interest / marker and zone control** | Brawler/Hacker/warband and available heavy support gave access under opposing WinterFor guns; outcome was scenario-dependent. | [#075](../../notes/battle-reports/071-080-n5-battle-report-tactical-analysis.md) |
| **Provisioning** | Brawler/Druze specialist options and inexpensive opportunistic attackers require clear carry route instead of only heavy damage. | [#138](../../notes/battle-reports/131-140-n5-battle-report-tactical-analysis.md) |

**Limits:** Low confidence for a general Ikari mission edge: the reports document tools and tactical interactions, not independently repeated wins. Game-era qualitative evidence, not a win-rate or current Fireteam claim. [Full mission evidence audit](../../notes/battle-reports/cross-report-mission-performance-by-sectorial.md).

## Counterplay — observed N5 battle-report responses (2026-11-02)

| Threat / target | Observed response and limitation | Battle reports |
|---|---|---|
| **Against Camo/zone denial** | Brawler MSV2 sniper + Druze Hacker, Yojimbo Smoke, Wu Ming/Tanko and Armand Le Muet long gun attacked TAK/Vystrel/marker shells, but #067 Camo/Decoy still wasted Orders. | [#067](../../notes/battle-reports/061-070-n5-battle-report-tactical-analysis.md), [#075](../../notes/battle-reports/071-080-n5-battle-report-tactical-analysis.md) |
| **Vs HI/TAG tech** | Brawler Hacker/Wu Ming TinBot, cheap Yuan Yuan/Desperado and hard long-range ARO create more than one angle, however #185 Classified tally was debated due to cancellation rules. | [#185](../../notes/battle-reports/181-190-n5-battle-report-tactical-analysis.md) |
| **Counterexample: protected room** | Heavier Ikari units did not simply overcome WinterFor mobile Shona/Liang Kai and Area of Interest score; score zones instead of chasing premium gun. | [#075](../../notes/battle-reports/071-080-n5-battle-report-tactical-analysis.md) |

**Limit:** Weak repeated outcome evidence for a specific anti-Impersonator or TAG killer; do not inflate Ikari's counter tier. Game-era tactical evidence, not current N5.3 profile/Fireteam or faction win-rate claims. [Full cross-report counterplay analysis](../../notes/battle-reports/n5-cross-report-counterplay-tags-hi-hacking-camo-impersonators-fireteams.md).

---

## Must-have / Go-to / Avoid — source-backed recommendations (2026)

Dated source-backed tactical preferences and miniature purchasing priorities; opinions do not override N5.3 roster, profile or Fireteam data above.

**Original audit title:** NA2 mercenary sectorials — Must-have / Go-to / Avoid (N5.3)

**Audit date:** 25 October 2026. **Scope:** Druze Bayram Security, Ikari Company, StarCo Free Company of the Star, Dahshat Company, White Company. This companion to the other faction selection audits in this folder evaluates competitive **standard 300-point N5.3** lists. It does not import Reinforcement, optional Spec-Ops/Team-Ops, or a neighboring faction's Fireteam permissions.

**Authority order:** The five repository-native N5.3 sectorial references linked below are authoritative for available troops, particular profiles, AVA, points/SWC, and Fireteams (Army data 7.26246.159, 3 September 2026, verified 16 October). YouTube/podcast transcripts are evidence for **a speaker's opinion**, not a measured tournament inclusion rate or a guarantee of efficiency. Several sources predate N5.3; their strategic observations must be reconciled with the pinned roster. In particular, N5 fireteam changes invalidate some older linked Guided claims.

**Labels used here:**
- **Must / near-must:** An actual presenter's explicit almost-every-list recommendation, or a defensible near-universal list-building package. Near-must does **not** mean compulsory in every mission or list style.
- **Go-to:** Efficient, consistently defensible use of points, SWC, Order slots and a defined tactical job. The alternatives are often mutually exclusive.
- **Avoid / never take:** An **explicit reviewer rejection**, or a specific profile or construction displaced in its intended role by a better same-roster investment. Mark as **contested/conditional** when any credible niche or dissent exists. Do not invent categorical bans when only an older negative opinion is available.
- **Evidence:** **Direct** = explicit recommendation/rejection in a transcript; **Corroborated** = source rationale plus previously transcript-audited repository guide; **Contested** = meaningful opposing speaker's interpretation; **Edition-limited** = interpretation of pre-current Army data.

### Quick comparison

| Sectorial | Most defensible must / near-must | Reliable go-to choices | Strongest sourced avoid | Absolute never-take? |
|---|---|---|---|---|
| **Druze** | Druze **KHD + Pitcher** (direct repeated default) | Brawler HRL, Hunzakut FO, Valerya, Yuan Yuan, Digger, Scarface or Bulleteers | **Anaconda as default TAG** vs Scarface/Triphammer; ordinary Druze HMG value | No: Anaconda has a scenario/total-cost niche |
| **Ikari** | No single compulsory unit; **cheap Keisotsu regular-order base** and **Wú Míng AP HMG** are most convincing defaults | Motorized Yojimbo, Yuan Yuan/Desperado, Tankō, Armand, Druze KHD, Karakuri/Pathfinder | **Security Chief Arslan** as value pick (explicit rejection) | No |
| **StarCo** | **Al Hawwa' KHD**, **Irmandinho** (direct auto-take claims); **Knauf FTO + Uhahu** as a standout package | Brawler/Digger PMC, Bandit Minelayer, Hellcat Paramedic, Mobile Brigada LT, Riot Grrls/Avicenna | **Alguacil premium guns**; **unsupported TAG investment** (Anaconda itself contested) | No |
| **Dahshat** | **Mimetism(-3) Libertos** (direct strong 9-point profile default) | Hunzakut, McMurrough, Zúyŏng + Rui Shi, Valerya, Zhēnchá, Maghariba | Redundant **Al Fasid HMG** or ordinary **Ghulam HMG as main attack** | No |
| **White Company** | No proven single must; **Hǎidào's multi-profile Wildcard role** is a near-default toolbox | Hawkwood K1, Karhu/Kaplan, Laxmee, Varangian/Shona, Guiláng, Tiger, Peacemaker/Sierra | **Fusilier SWC guns as premium shooters**; niche Longarms/Wild Bill | No |

### 2. Ikari Company

**Current reference:** [Ikari N5.3](ikari-company.md). **Direct sources:** [I1: WIP12 E191, Ikari with Copper](https://open.spotify.com/episode/0XooAPvaG5RXEX9wUgsDvy) (September 2025, podcast transcript previously and selectively rechecked for this audit, particularly Arslan/expensive attackers); [I2: Infinity the Dante, Ikari N5 Initial Reaction](https://www.youtube.com/watch?v=6kZ2YeFDoNI) (N5 launch, YouTube transcript reviewed in current sectorial analysis); [I3: WIP12 E163, Cobraprime takes Ikari to IGL](https://open.spotify.com/episode/6sA5fiWOLSIILRw7DO06tv) (2024/N4, podcast transcript historically reviewed). [Current Ikari tactical research](ikari-company.md#tactical-research--ikari-company-reviewed-2026-10-23) includes the contrary TAG/Daiyōkai arguments.

#### Must / near-must

- **No single current source establishes a literally compulsory individual troop.** The common **cheap Regular Keisotsu backbone (9–11 pts)** supports almost every wide Ikari design by giving Orders, a concealed inexpensive LT and economical FO. **Corroborated [I1,I2]**; the number and Fireteam configuration vary, so do not call a particular Keisotsu profile mandatory.
- **Wú Míng AP HMG, 33/1.5 — Copper's attack-piece default [I1].** A legal Wú Míng team provides inexpensive AP long-range shooting compared with **Daiyōkai HMG (50 pts)**, retaining room for smoke, anti-tech and specialists. **Exception:** Scarface-led, Tankō/Daiyōkai-NCO, or deliberately low-SWC lists. Thus this is a **near-must in inexpensive gunfighter Ikari**, not every legal Ikari list.

#### Go-to

| Unit/profile | Why it is good | Opportunity cost / exception | Evidence |
|---|---|---|---|
| **Motorized Yojimbo, 20/0** | Fast smoke, CrazyKoala/Minelayer, NWI and CC; helps MSV2 smoke-shooting | One of the Irregular fast attackers; foot Yojimbo alternative may solve tiny corridors | I1,I2 |
| **Yuan Yuan, 6+ / Desperado, 7–9** | Disposable aerial trade or immediate bike smoke/chain-rifle defense | Too many Irregular troopers choke Regular activations | I1,I2 |
| **Tankō ML (26/1.5), Blitzen/Disco Baller (18–19)** | Standoff ARO or cheap E/M close defense; Daiyōkai/Tankō Haris | ML eats SWC; old N4 Keisotsu bonus claims not current | I1,I2 |
| **Armand Le Muet, MSV1 MULTI sniper 34/1.5** | Mimetism(-6), forward deployment, survivable transmutation and versatile active/reactive lane threat | About three Keisotsu worth of list points | I1 |
| **Druze KHD, 23/0** | X-Visor Pitcher, Warhorse, D-Charges, hacker hunting | Not an ordinary HD; Ikari Druze family permits Duo/Haris, **not Core** | I1,I2 |
| **Karakuri FO 31–38 / Pathfinder 14–17** | Durable STR3 objective body vs very economical Sensor/FO/TacAware specialist | Karakuri **not linkable** in Ikari, unlike JSA; Pathfinder soft | I1,I2 |
| **Rui Shi MSV2 Spitfire, 23/1** | Efficient solo MSV2 smoke-shooting, optional EVO Marksmanship | **Not linkable** here; fragile/hackable | I2 |
| **Scarface + Cordelia / Triphammer** | Alternative armored AP striking or 0-SWC budget TAG plan | Compete with AP Wú Míng and required specialist slots; conditional [I1 vs I3] | I2,I3 |

#### Avoid / never-take candidates

- **Security Chief Arslan as general-purpose 35pt shooter/LT — Direct strong avoid [I1].** Copper explicitly calls him a poor-value unit: midrange shooting and other tools do not justify paying so much when **9pt Keisotsu LT / 15pt Brawler LT** and **33pt Wú Míng AP HMG** cover primary purposes cheaper. **Exception:** specific MSV1/WIP13/Warhorse, NWI and Fireteam command plan. Do not mislabel all Druze Shock Teams as bad.
- **Al Fasid 44–50pt as generic main gun — Conditional, shared skepticism [I1,I2].** An independent premium solo anchor is often beaten in slot economy by *linkable* Wú Míng HMG + supporting pieces. **Counter:** ARM5/BTS6, Sixth Sense, Albedo, smoke/Minelayer may be needed where you want independent defense and no Fireteam exposure.
- **Daiyōkai HMG as a pure damage-per-point replacement for Wú Míng — Contested [I1 vs I2,I3].** Copper saves 17 points with AP Wú Míng; others value NCO/armor, a mobile Tankō Haris and close combat. It is **not** a general never-take.
- **Early video “linkable Guided Clipper” shortcut — invalid construction**, not a troop veto. Guided Clipper is unlinked; the link-eligible FTO is direct ML without Guided. Do not merge them.

### Cross-sectorial ranking principles / edition checks

1. **A “must” is a reported list-building default, not tournament telemetry.** Most explicit Druze/StarCo/Dahshat endorsements are a named player's preferences; there is no verified representative inclusion-rate database here.
2. **Do not call every TAG “never take.”** Druze Anaconda has strongly negative direct testimony, whereas **StarCo Anaconda gets a persuasive later rehabilitation in a supported Haris**, and WhiteCo uses a different Kaplan Duo. It is the *same chassis with different team architecture*. The Triphammer's 0-SWC entry can also be right even if it loses raw shootout comparisons.
3. **Do not conflate FTO label and permission:** Druze Guided Clipper differs from Fireteam FTO direct ML; Ikari Guided Clipper similarly does not link; WhiteCo Clipper FTO has no Fireteam row at all; StarCo Stempler FTO likewise has no current StarCo chart row. Always use the exact current Fireteam chart and profile option.
4. **Irregular versus Regular economy is decisive:** Irregular smoke/assault excels individually in Ikari, StarCo and Dahshat, but 15 slots and too few pooled Orders can make even a roster of efficient units dysfunctional. The **Regular** cheap Keisotsu, Fusiliers, Fugazi/Fanous/Transductor and specialist options have systemic value.
5. **Mission scoring and delivery beat theoretical damage:** Druze/Dahshat Hunzakut, Ikari Karakuri/Pathfinder, StarCo Al Hawwa'/Hellcat and WhiteCo Guiláng/Tiger change whether a gun-heavy list can reach a console on time.
6. **No illegal legacy data:** Current N5.3 Army references override early N5/N4 transcripts: old StarCo Alguacil LT SWC tax, old N4 Dahshat Zúyŏng LT, imported Karakuri Fireteams, early linked-Guided Clipper assumptions and other-faction TAG/REM permissions are not reliable.

### Source coverage and limitations

- **Direct full/partial transcripts checked in the immediate research:** Druze N5 Dante, WIP12 Druze E75; StarCo N5 Dante, Loss of Lieutenant E158 StarCo section; WIP12 Ikari E191 sections, Dahshat E165 Libertos sections; WhiteCo N5 Robert Shepherd and tournament report. Remaining linked recordings were **already transcript reviewed in the corresponding existing GitHub tactical files**; do not portray every transcript as newly reviewed in this commit.
- **N4-era sources:** Druze WIP12 E75 (2022), Dahshat WIP12 E165/E166 (2024), WhiteCo WIP12 E160 (2024), Ikari IGL E163 (2024). Their exact points, team bonuses, and equipment are not current evidence. The N5.3 sectorial files take priority for such facts.
- **Dahshat N5 coverage is comparatively thin:** one substantive current N5 battle report plus cross-faction unit reviews; especially avoid inventing consensus “never take” choices. **WhiteCo tournament footage** demonstrates actual successful packages but some event formats/rules and mission requirements differ from standard play.
- **Contrary opinions intentionally retained:** Ikari Daiyōkai/Al Fasid vs cheap Wú Míng; Druze Scarface vs cheaper direct solutions; StarCo Anaconda before/after later podcast; Dahshat Maghariba vs discount swarm; WhiteCo Guiláng vs Nøkken and K2 vs heavier support.

### Whole-unit purchasing audit — can I omit an entire miniature? (2026-10-30)

This section is intentionally **sectorial-specific**: buying the same Anaconda sculpt for *Druze* versus *StarCo* gives materially different Fireteam/support access. **Skip by default** = low purchasing priority in mainstream 300pt builds, **not** a proven prohibition on every list.

| Sectorial | Entire model/unit to defer | Why / decisive exception |
|---|---|---|
| **Druze Bayram Security — Anaconda** | **Skip by default — strong single-source-pair negative** | [D1] presenters favor **Scarface + Cordelia** as the efficient TAG/repair purchase. Anaconda remains valid as a **59pt standalone/Mechanized Duo** role that Scarface's full package cannot duplicate. Do not transfer this verdict to StarCo. |
| **Ikari — Security Chief Arslan (35pt)** | **Skip by default for normal attack/LT plans** | [I1] Copper directly rates his cost inefficient against **Keisotsu/Brawler LT** and **Wú Míng AP HMG** covering those jobs. Buy if specifically leveraging **MSV1, Warhorse, NWI or command/team role**. Not a dismissal of Druze Shock Teams. |
| **StarCo — Anaconda / Triphammer** | **Defer blind standalone TAG purchases; no entire-unit hard skip** | [S1] condemns both; later [S2] argues for Anaconda's **Brawler Engineer + Digger Armored Haris**, while Triphammer buys **0 SWC**. Purchasing one for a supported role can be rational. |
| **Dahshat** | **No source-backed whole-model avoid** | Al Fasid and Ghulam **generic guns** duplicate other attacks, but retain real support/defensive profiles and there is too little current direct evidence to blacklist units. |
| **White Company — Chaksa Longarms** | **Defer as first main gun; low confidence** | [W1,W3] prefer K2, Nisse and ORC for the usual ranged role, but Longarms' legal Duo/Haris and unusual weaponry still create distinct angles. Anaconda can use a Kaplan Duo, unlike Druze/StarCo constructions. |

**Important:** The ordinary Druze HMG, Alguacil SWC, Fusilier SWC, Clockmaker-without-repair-target and Hawkwood CoC criticisms are **profile/usage warnings**, not full model skips. See [all-armies buying shortlist](../../notes/factions/model-purchase-avoid-summary-2026.md).

### Worst-value, rare-use and proxy-first mercenary miniature purchases (2026-10-30)

**Scope and evidence.** This is a **miniature-buying audit**, not a re-ranking of every profile. It covers each current NA2 army separately: [Druze Bayram Security](../non-aligned-armies/druze.md), [Ikari Company](ikari-company.md), [StarCo](../non-aligned-armies/starco-free-company-of-the-star.md), [Dahshat Company](dahshat-company.md), and [White Company](white-company.md). References are the **pinned N5.3, September 2026 Army 7.26246.159 rosters and Fireteam charts**. **Direct negative** means the speaker actually criticized that use in the earlier [transcript-backed source register](#source-coverage-and-limitations). **Proxy first**, **conditional whole-model deferral**, and **extra-copy defer** are *reasoned buying suggestions*, not claims the media said those literal words. **Rare** means unusual in reviewed all-comers constructions, *not a measured tournament inclusion rate*. When the existing podcast reviews predate current Army, the **current printed profiles** govern. No all-profile universally unplayable unit is established.

**Four distinctions matter:** a **weak gun profile** can belong to a very good unit; a **conditional whole-model deferral** is not a zero-win-rate label; a **rare specialized peripheral/character** can deserve a proxy even when genuinely excellent; and **AVA / alternate weapon sculpts** alone never create a shopping need. Also **one bought model can be reused across different legal sectorials**, not fielded twice simultaneously. No current complete inventory of the five mercenary armies was found at the expected inventory paths; the cross-army proxy examples below **do not assume ownership** of NA2-exclusive models.

#### 2. Ikari Company — weak Arslan value and optional expensive solo HI

| Unit / option / purchase | Comparison, evidence and exception | Buy / proxy decision |
|---|---|---|
| **Security Chief Arslan35/0** as default gun/LT | **Direct negative — [WIP12 E191 with Copper](https://open.spotify.com/episode/0XooAPvaG5RXEX9wUgsDvy):** **Keisotsu9pt LT/cheap body** or **Brawler LT** is a cheaper command plan, and **Wú Míng AP HMG33/1.5** is a better long-range main-gun purchase. Arslan still has **MSV1, Disco Baller, Warhorse, NWI and a distinctive Wildcard/command** niche. | **Strong whole-miniature default defer / proxy first** unless the precise Disco/MSV/LT combination is your plan. This is a critical *Ikari-specific* review; in Druze the team opportunities differ. |
| **Al Fasid HMG50/1.5 or HRL44/1.5** bought as a normal link replacement | **Conditional reviewer skepticism — [WIP12 Ikari](https://open.spotify.com/episode/0XooAPvaG5RXEX9wUgsDvy), [Dante Ikari](https://www.youtube.com/watch?v=6kZ2YeFDoNI)**: **Wú Míng AP HMG33** in an affordable team and **Tankō/Keisotsu** screen often spend points more effectively. But **Al Fasid S5 ARM5/BTS6, Albedo, Sixth Sense, smoke GL/Minelayer** is a unique autonomous terrain/ARO package; it is *not* a direct S2 Wú Míng proxy. | **Defer dedicated S5 Al Fasid** until that independent **smoke, Albedo or unusual defender** angle is used. **Not** an all-profile negative: HMG and HRL are different supported functions. |
| **Daiyōkai HMG NCO50/1** bought solely to mimic Wú Míng AP HMG33 | **Direct disputed comparison:** Copper prefers economical Wú Míng, but other Ikari voices value **NCO, extra armor, NWI, CC**, and a **Tankō Haris** alongside a strong LT. **Daiyōkai MMR46/0 / Red Fury47/1** also have different distance/SWC jobs. | **Proxy first if your entire need is one AP long-range gun**; buy the S5 Daiyōkai when a **real NCO/LT/Tankō attack module** repeatedly exploits it. **Do not label it never-take**. |
| **Scarface+Cordelia76–80 or Triphammer48–53 as another default premium gun** | Both have legitimate **TAG/AP strike** and **TurtleMek** ancillary roles. But with affordable linked **Wú Míng** and defensive Tankō, TAG spending can leave few Regular scoring Orders; Scarface **composite** requires *both* Engineer and TAG representations. **Triphammer48/0** is legitimately useful in an SWC-constrained list. | **Borrow/proxy properly sized S7 TAG plus relevant S1 TurtleMek; for Scarface represent Cordelia separately**, test before buying large kit. **Not a blanket TAG ban**. |
| **Multiple Wú Míng weapon sets or full 5-body unit simply because AVA5** | **Wú Míng AP HMG33/1.5 is a strong default**, but **SMG19/22, BSG+TinBot22, E/M grenade launcher27, ML/HRL** serve different link and firewall jobs; not every gun sculpt is required. A **five-model block** can exhaust the budget for midfield specialists. | **Buy a first Wú Míng gun and real eligible team roles; proxy second/third extra guns** until needed simultaneously. Avoid full AVA as acquisition plan. |
| **Fourth Yuan Yuan or Bashi Bazouk, duplicate Desperado/Motorized Bounty Hunter and Krakot** | **Reasoned, not poor-unit verdict:** **Yuan Yuan**, **Desperado**, **motorized Yojimbo**, **Krakot**, **Bashi** all add different smoke, short-range, AD/Parachutist and Irregular order effects. They cannot collectively generate pooled Regular Orders for the Wú Míng gun. **Bashi** has specialist options; Irregular does not mean not useful. | **Proxy surplus Irregular traders and rare AD models before buying extra**. For **motorcycles use correct S4 base**; a Bashi/Digger/Yuan Yuan S2 mini is not automatically a motorbike. |
| **Foot Yojimbo19 and motorized Yojimbo20 as two simultaneous roster units** | **Hard identity restriction**, same as other JSA armies: **one Yojimbo only**. The user's [Shinden inventory](../../inventory/shindenbutai.md) already records **one foot and one mounted Yojimbo**. | **Don't buy any Yojimbo for Ikari** if reusing the same owned sculpts in separate games. Select the correct legal profile and form; **no legal double-Yojimbo**. |
| **Karakuri Mk12/FO38 and all Karakuri gun variants without protected scoring goal** | **Credible valuable specialist**, but **Ikari Karakuri are solo, not automatically linked** as in JSA. You pay 31–38pts for STR3, FO, Remote Presence and durability, versus **Pathfinder Sensor/FO** or cheap Ninja/Cube Jäger mission reach. | **Proxy a Karakuri first and extra sculpts** until its durable solo scoring genuinely beats the cheaper alternative. **Do not dismiss the first Karakuri** when objectives must survive hostile fire. |
| **Guided Clipper16/1.5 combined with FTO19/1.5 linked launcher fantasy** | **Current roster correction:** **16pt Guided** not link-eligible; **19pt FTO +1B direct ML** **not Guided**. Cheap **Druze KHD Pitcher23** needs ordinary Spotlight from another Hacker/FO for Guided. | **Avoid the illegal plan, not the missile REM**. **Proxy one right-size Clipper** to choose a legal option; don't buy multiple models for a single AVA1 weapon variant. |
| **Specialized single purchase: Armand sniper34/1.5, Kiiutan IMP-2, Saito-like hidden Ninjas, Cube Jäger Paramedic** | **Real distinct jobs but non-default:** **Armand** Mimetism(-6) forward sniper, **Kiiutan** unexpected Impersonation, **Ninja** hidden scoring, **Cube Jäger** Irregular flank medic. Their jobs matter in particular matches, but an army that already buys 2–3 Irregular attack pieces may not afford all. | **Proxy the *second* rare attacker or niche named sculpt first**; don't mistake a specialty all-star on some missions for a needed model in every Ikari list. |
| **Extra Rui Shi/Lù Duān, Pangguling and Pathfinder remote collection** | **Efficient individual REM roles:** Rui Shi MSV2 Spitfire, Lù Duān Holoprojector, Pangguling Baggage, Pathfinder FO/Sensor. But **Rui Shi is not a linked Ikari gun**, unlike some JSA/Shinden Fireteam configurations. | **Use matching-footprint shared REM sculpts** from other armies, and only acquire another chassis when two different remotes really deploy concurrently. |

**Ikari priority:** cheap **Keisotsu LT/Orders**, **Wú Míng AP HMG33**, Smoke/deliverability (one **Yojimbo/Desperado/Yuan Yuan**), **Druze KHD Pitcher23** if cyber support, a real objective getter. **Best whole-model defers** are **Arslan**, nonplanned **Al Fasid S5**, and another large TAG/expensive solo sniper/assassin; no single current unit is universally unusable.

#### 6. Cross-mercenary — reuse, proxy rules and multi-body purchase traps

**Inventory note:** no separately verified, complete Druze/Ikari/StarCo/Dahshat/WhiteCo miniature inventories were found. The project *does* contain physical inventories for [Shindenbutai](../../inventory/shindenbutai.md), [Caledonia](../../inventory/caledonia.md), [Kestrel](../../inventory/kestrel.md), [Military Orders](../../inventory/military-orders.md) and [Steel Phalanx](../../inventory/steel-phalanx.md). **Cross-collection re-use is a candidate, not an assumption that the same sculpt is unoccupied in a simultaneous list.** In particular, two Yáoxiè Rui Shi/Lù Duān physical chassis, PanO Dronbot/Mulebot pools and both Yojimbo forms are documented in Shinden; Caledonia Cateran(s) and shared Warcor can be available where current roster allows. Check [inventory rows](../../inventory/shindenbutai.md) before ordering equivalents for an NA2 list.

| Physical category and example models | Recommended test/reuse | Do not overbuy or misrepresent |
|---|---|---|
| **Shared NA2 infantry characters** — Arslan, Valerya, Druze, Brawler, Digger, Aïda, Saito, Wild Bill, Hawkwood, Knauf, Uhahu, Parvati etc. | Use an appropriate, distinctly identified **same-size Corvus Belli infantry proxy** in each legal sectorial; prioritize characters actually in the intended list. One sculpt can represent **non-simultaneous** options across armies, or another legal unit if accepted. | **Do not import faction access.** Druze Arslan differs from Ikari Arslan value; StarCo Knauf cannot be WhiteCo Hawkwood by changing cards without an allowed physical proxy; one model can't be two deployed characters at once. |
| **Alguacil/Fusilier/Keisotsu/Ghulam/Druze/Brawler weapon variants and FTO** | Use existing generic or same-troop properly sized mini to test LT/FO/KHD/Doctor/Engineer/HMG/ML choices; clearly declare the selected loadout. | Buy **extra specific weapon sculptures** when they are actually **different legal simultaneous troopers**, not because a variant appears in Army. FTO status and link membership must be checked by exact sectorial. |
| **TAGs and supporting model counts** — Anaconda S7, Scarface+Cordelia+Turtlemek, Triphammer+Turtlemek, Maghariba S8+Jandab, Gūijiă+Shàngdiào | Borrow a *correct silhouette/base TAG* and **all separately deployed ancillary/Engineer figures** in the actual selected package. A Tag-equivalent S7 base does not automatically stand for an **S8 Maghariba**. Anaconda **Operator** appears on escape; plan an S2 model/representation then. | Scarface composite is **not just a Scarface TAG purchase**; regular physical count includes **Cordelia** and **TurtleMek**. Ancillaries aren't independent Regular Order generators. Buy large sculpts after real mission tests, not for one-time novelty. |
| **Peripherals/Servants** — Fiddler+Jackbot(s), Carmen+Bâtard, Peacemaker+Auxbot, Yáozăo/Nasmat/Zondbot, Yojimbo Koalas, Synchronized companions | Proxy **each fielded partner** with a separate, correctly based body; **equipment markers** (mine, Koala etc.) have their own marker requirements but don't make extra troopers. | Some options do **not** include companions (e.g. Fiddler FTO vs independent Jackbot; specific Peacemaker without Auxbot). Don't buy all option-specific peripherals without selecting their legal profiles. |
| **Shared JSA/Chinese/PanO REM chassis** — Yáoxiè Rui Shi/Lù Duān, Dronbot Pathfinder/Clipper/Sierra/Fugazi, Yáopú/Pangguling/Mulebot, Rafiq/Fanous, Traktor Mul | Reuse documented **2 Yáoxiè chassis**, **4 PanO Dronbots** and **2 PanO Mulebots** as **compatible-sized** temporary replacements, provided current event proxy permissions. **Traktor Mul S4** and **Maghariba S8** must be represented by their own size, not any spare S3 Dronbot. | Buy only chassis that actually **co-deploy in an NA2 list**, or are needed for correct base/size/appearance. The inventory's two Rui Shi/Lù Duān models are **two physical total**, not two of each. |
| **Smoke/Irregular warbands and airborne attackers** — Yuan Yuan, Bashi Bazouk, Hunzakut, Desperado, Libertos, Kum, Irmandinho, McMurrough, Motorized Bounty Hunter, Yojimbo | Proxy a rarely used cheap trader/AD with a **distinct correct-size** infantry/motorcycle/warband in the intended legal roster. The [Shinden inventory](../../inventory/shindenbutai.md) confirms foot+mounted Yojimbo; **motorcycle S4** differs from ordinary S2 smoke infantry. | Don't buy up to AVA automatically. **Hunzakut FO** and **Irmandinho Engineer** are Irregular; too many Irregular trades can starve the main gun of pooled Regular activations. |
| **Medium-heavy specialized silhouettes** — Al Fasid S5, Daiyōkai S5, Karakuri S2, Wú Míng S2, Riot Grrl S2, and vehicle/motorbike models | Use **correct silhouette/base** first and choose models with clearly different identities. **S5** is not an ordinary S2 stand-in; a TAG/Vehicle cannot be represented as common infantry at organized play without organizer permission. | Don't buy an S5 heavyweight simply because you already own a generic S2 HI; verify actual match and legal current unit. |
| **No actual rules on “linked Guided” unless exact profile supports both** | Druze/Ikari Clipper FTO direct ML is **not Guided**, while the Guided profile is **unlinked**; WhiteCo Clipper FTO has **no Fireteam access**; StarCo Stempler FTO likewise not linkable. Test individual **correct unit/profile/network** combinations in Army before purchase. | Do not buy REM artillery boxes for a nonexistent *FTO Guided* bonus. A Guided missile requires actual Targeted source, not merely an expensive KHD with a Pitcher. |
| **Legacy N4/early N5/Spec-Ops/Team-Ops minis** | Reuse sculpts as current legal proxies where sizes and organizer acceptance fit; edition-old fireteam boxes aren't automatically useful whole bundles. | **Do not buy optional-mode-only troops solely for standard play**. A saved N4 TAG/Fireteam roster isn't an N5.3 shopping list. |

**Combined “do not bother buying first” shortlist (not all-profile play bans):** **Druze** Anaconda without a real 59pt plan, HMG-only Druze and full Fiddler multi-bot kit; **Ikari** Arslan and unsupported Al Fasid/S5 or multiple TAGs; **StarCo** solo Anaconda/Triphammer without the relevant Armored plan, expensive optional Alguacil SWC guns, second Engineer/sniper collection; **Dahshat** Al Fasid as redundant gun, optional Ghulam HMG/ML, unproven extra guided/Maghariba TAG and excess Irregular duplicates; **WhiteCo** Chaksa Longarm box and Wild Bill before a specific team, Fusilier heavy weapon sculpts, nonplanned Anaconda and alternate Hawkwood/HD+ kits. **All** deserve re-evaluation if the exact mission, missing collection capability or verified legal Fireteam calls for them.

**Proxy policy/physical limit:** Always declare which legal Army profile each figure represents before playing. Keep its **proper base, silhouette, visibility geometry, different body for each simultaneous trooper, and actual peripheral/Ancillary count**; check current ITS and event organizer proxy policy before organized play. Proxies never change Army availability, AVA, SWC, Fireteam chart, model's real equipment, or independent Order generation.
