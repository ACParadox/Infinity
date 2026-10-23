---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 908
sectorial_slug: dahshat
sectorial_name: Dahshat Company
parent_faction: Non-Aligned Armies (NA2)
rules_baseline: N5.3
army_source_version: "7.26246.159"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-16
coverage: "Complete current Dahshat Company main roster, standard loadouts and AVA, current Fireteam chart and reverse access index, optional Spec-Ops/Team-Ops boundary, linked Reinforcements boundary, source relations, and derived tactical indexes."
---

# Dahshat Company — N5.3 sectorial reference

## Overview and provenance

Repository-native reference for **Dahshat Company** (Army sectorial ID `908`), part of the Non-Aligned Armies (NA2). Corvus Belli Army currently spells the sectorial **Dahshat Company** and uses slug `dahshat`; older/common shorthand such as “Dashat” should resolve to this reference.

Sources used:

- Corvus Belli Army-derived revision `7.26246.159` from `massayoshi/infinity-army-backup` commit `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b` (`army: N5.3 + ITS18`, 2026-09-03).
- Versioned source: `n5/dahshat/7.26246.159.json`, blob `66a9ffda81fe1db5d3b1688ca3605bde0f9e0d61`.
- Aggregate source: `n5/dahshat/dahshat.json`, blob `9039a979d341ab9634a0c3682ceeb8b29130f54b` at the pinned source commit.
- InfinityDB normalization/semantics: commit `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: N5.3 + N5 FAQ v0.1.

Coverage notes:

- Covers **39 standard Dahshat roster entries** explicitly assigned to faction `908` by the current Army source.
- `Rumbler Spec-Ops` (ID `1925`) and `NA2 Team-Ops` (ID `1939`) are optional-mode entries and are kept separate from the standard roster.
- Generic Soldiers-of-Fortune / mercenary-catalogue objects with an empty `factions` array are excluded. Explicit Dahshat entries such as Monstruckers, Triphammer, Bashi Bazouks, Motorized Bounty Hunters, Libertos, McMurrough, Diggers and Brawlers are retained.
- Linked Reinforcement army ID: **999**. Main and Reinforcement rosters remain separate.
- Army raw Fireteam `DUO: 256` is the source sentinel for effectively unlimited Duo formations, not a literal limit of 256.
- Disabled subordinate forms/peripherals such as Jandab, Jackbots and TurtleMek are documented with their parent units and are not counted as independent roster entries.
- `FTO` labels do not independently grant Fireteam access. Current examples with FTO-labelled profiles but no matching Dahshat chart row include the foot `112 Emergency Service` and `Húláng Shocktroopers`.

## Sectorial summary

| Field | Value |
|---|---|
| Sectorial | Dahshat Company |
| Parent faction | Non-Aligned Armies (NA2) |
| Army ID | `908` |
| Army slug | `dahshat` |
| Rules baseline | N5.3 + FAQ v0.1 |
| Standard Main roster entries | 39 |
| Optional-mode entries | Rumbler Spec-Ops; NA2 Team-Ops |
| Reinforcement roster | Army ID `999` |
| Core | up to 1 |
| Haris | up to 1 |
| Duo | unlimited/source `256` sentinel |
| Fireteam families | Ghulam; Brawlers; Odalisques; Zúyŏng; Assault |
| Explicit Wildcards | Authorized Bounty Hunters; Sforza FTO; Miranda Ashcroft; Valerya Gromoz; Diggers |

## Fireteam chart limits and sectorial-level restrictions

| Constraint | Current source value / normalized meaning |
|---|---|
| Core | `1` |
| Haris | `1` |
| Duo | `256` — normalized as unlimited Duos |
| Main/Reinforcement mixing | Main roster and Reinforcement roster `999` remain separate |
| Wildcards | Only the explicit Wildcard rows listed below |
| Profile restrictions | Preserve FTO, Spec-Ops, counts-as comments, `required` flags and source minimums exactly |

The chart contains five named Fireteam families plus a separate Wildcard list. The canonical chart below is authoritative; do not import Fireteam permissions from older N4 Dahshat charts or another NA2/Haqqislam/Yu Jing sectorial.

## Unit roster index

| Unit ID | Unit | AVA | Type | Classification | Order status / notes |
|---:|---|---:|---|---|---|
| 333 | Nasmat Remotes | 4 | REM | Support | Peripheral (Servant) |
| 317 | Shaytaniyah Remotes | 1 | REM | Support | Regular; Guided option |
| 51 | Miranda Ashcroft | 1 | LI | Character | Regular; Wildcard, counts as Odalisque |
| 309 | Maghariba Guard | 1 | TAG | Mechanized | Regular + Tactical Awareness; Baggage |
| 315 | Rafiq Remotes | 1 | REM | Support | Regular; FO/Sensor; profile 3 Assault FTO |
| 160 | Yáoxiè Lù Duān | 1 | REM | Support | Regular; Holoprojector/MSV1 |
| 159 | Yáoxiè Rui Shi | 1 | REM | Support | Regular; Zúyŏng Fireteam member |
| 1333 | Monstruckers | 2 | LI | Mercenary | Irregular Engineer; Brawler team member |
| 1569 | Triphammer | 1 | TAG | Mercenary | Regular + Tactical Awareness; Assault Duo |
| 325 | Bashi Bazouks | 4 | LI | Mercenary | Irregular; Parachutist/Holoprojector |
| 316 | Shihab Remotes | 1 | REM | Support | Regular; Total Reaction |
| 1565 | Motorized Bounty Hunters | 2 | LI | Mercenary | Irregular, Impetuous; Assault Duo |
| 1275 | Libertos Freedom Fighters | 2 | LI | Mercenary | Irregular; camouflage/minelayer options |
| 283 | McMurrough | 1 | WB | Character | Irregular, Impetuous; smoke/CC |
| 1564 | Fiddler | 1 | LI | Character | Regular Engineer; profile 1 Ghulam FTO |
| 324 | Odalisques | 4 | LI | Spec. Trained | Regular; native Duo/Haris |
| 310 | Hunzakuts | 2 | SK | Spec. Trained | Irregular infiltrators |
| 1259 | Zhēnchá | 1 | HI | Spec. Trained | Regular; camo/infiltration specialist |
| 668 | Saito Togan | 1 | SK | Character | Regular; hidden/infiltration/smoke |
| 464 | Valerya Gromoz | 1 | LI | Character | Regular Hacker; Wildcard |
| 1284 | 112 Emergency Service (Motorized) | 1 | LI | Support | Regular Doctor; smoke |
| 255 | 112 Emergency Service | 2 | LI | Support | Regular Doctor; FTO label but no chart access |
| 248 | Highlander Caterans | 1 | LI | Spec. Trained | Irregular camouflage sniper |
| 1568 | Diggers | 2 | HI | Mercenary | Regular, Impetuous; Wildcard counts as Brawler |
| 50 | Warcors | 1 | LI | Mercenary | Irregular |
| 257 | Traktor Mul | 2 | REM | Support | Regular; Baggage; Guided artillery options |
| 318 | Fanous Remotes | 3 | REM | Support | Regular Repeater |
| 256 | Dozers | 1 | LI | Support | Regular Engineer |
| 49 | Authorized Bounty Hunters | 4 | LI | Mercenary | Regular; explicit Wildcard max 4 |
| 313 | Kum Motorized Troops | 4 | WB | Line | Irregular, Impetuous; smoke |
| 1747 | Zellenkrieger | 1 | WB | Support | Irregular, Impetuous; profile 3 Brawler FTO |
| 987 | Brawlers | 5 | MI | Spec. Trained | Regular; Core/Haris/Duo anchor |
| 127 | Zúyŏng Invincibles | 5 | HI | Line | Regular; Core/Haris anchor; TacAware options |
| 198 | Father Lucien Sforza | 1 | MI | Character | Regular; NCO; FTO profiles 2–3 Wildcard |
| 314 | Najjarun Engineer | 1 | LI | Support | Regular Engineer |
| 334 | Kameel Remotes | 2 | REM | Support | Regular; Baggage/EVO/TR options |
| 1257 | Húláng Shocktroopers | 1 | HI | Veteran | Regular; FTO labels but no chart access |
| 343 | Al Fasid | 1 | HI | Veteran | Regular; Assault Duo; smoke option |
| 301 | Ghulam Infantry | 6 | LI | Line | Regular; Core/Haris anchor |

## Unit details and current profiles

### Nasmat Remotes

**Unit ID:** 333 · **Slug:** `nasmat-remotes` · **AVA:** 4 · **REM / Peripheral**  
`MOV 15-10 | CC 11 | BS 8 | PH 10 | WIP 13 | ARM 0 | BTS 3 | STR 1 | S 1`. Courage, Mimetism (-3), Peripheral (Servant).

| Profile | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 3 | 0 | PARA CCW (-3); Servant |

### Shaytaniyah Remotes

**Unit ID:** 317 · **Slug:** `shaytaniyah-remotes` · **AVA:** 1 · **REM / Support / Regular**  
`MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 0 | BTS 3 | STR 1 | S 3`. Remote Presence, Courage.

| Profile | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 16 | 1.5 | Missile Launcher; **BS Attack (Guided)** |
| 3 | 19 | 1.5 | Missile Launcher (+1B); **no Guided skill** |

There is no current Dahshat Fireteam chart row for Shaytaniyah; the +1B loadout does not imply Fireteam access.

### Miranda Ashcroft, Authorized Bounty Hunter

**Unit ID:** 51 · **Slug:** `miranda-ashcroft-authorized` · **AVA:** 1 · **LI / Character / Regular**  
`MOV 10-10 | CC 19 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Mimetism (-6), Specialist Operative, Marksmanship, Stealth.

| Profile | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 27 | 0 | MULTI Rifle, PARA Mine, Boarding Pistol, Monofilament CCW |
| 2 | 25 | 0 | Boarding Shotgun, PARA Mine, Boarding Pistol, Monofilament CCW |
| 3 | 28 | 0 | Combi Rifle, E/Mitter (+1B), PARA Mine, Boarding Pistol, Monofilament CCW |

Explicit Wildcard; current chart comment `(Odalisque)`.

### Maghariba Guard

**Unit ID:** 309 · **Slug:** `maghariba-guard` · **AVA:** 1 · **TAG / Mechanized / Regular**  
`MOV 15-10 | CC 16 | BS 14 | PH 17 | WIP 14 | ARM 8 | BTS 6 | STR 3 | S 8`. Baggage, ECM: Guided (-6), ECM: Hacker (-3), 360º Visor, Tactical Awareness, Religious Troop, Terrain (Desert), Dodge (PH=10), GizmoKit (PH=11). Includes disabled **Jandab Remote** ancillary, not an independent roster entry.

| Profile | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 72 | 1.5 | MULTI HMG, E/M Carbine (+2B), AP Heavy Pistol, CCW |
| 2 | 71 | 1.5 | MULTI HMG, HRL, Grenade Launcher, Heavy Pistol (+1B), CCW |
| 3 | 71 | 1.5 | MULTI HMG, Heavy Flamethrower (+1B), Mine Dispenser (Shock), AP Heavy Pistol, CCW |

All current profiles generate Tactical Awareness and may fill the Assault Fireteam Maghariba row.

### Rafiq Remotes

**Unit ID:** 315 · **Slug:** `rafiq-remotes` · **AVA:** 1 · **REM / Support / Regular**  
`MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | STR 1 | S 3`. Deactivator, Repeater, Forward Observer, Sensor, Remote Presence, Courage.

| Profile | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 13 | 0 | Rifle, Light Shotgun, Flash Pulse; Triangulated Fire |
| 3 | 19 | 0.5 | **FTO** Red Fury, Flash Pulse |

Only profile **3** fills the `RAFIQ REMOTE FTO` row in Assault Fireteams.

### Yáoxiè Lù Duān

**Unit ID:** 160 · **Slug:** `yaoxie-lu-duan` · **AVA:** 1 · **REM / Support / Regular**  
`MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 6 | STR 1 | S 4`. Holoprojector, MSV1, Remote Presence, Surprise Attack (-3), Courage, BS Attack (+1B).

| Profile | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 24 | 0 | Mk12, Heavy Flamethrower, E/M Mine |
| 2 | 20 | 0 | Thunderbolt, E/M Carbine, E/M Mine |

### Yáoxiè Rui Shi

**Unit ID:** 159 · **Slug:** `yaoxie-rui-shi` · **AVA:** 1 · **REM / Support / Regular**  
`MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 6 | STR 1 | S 4`. Repeater, Remote Presence, Courage.

| Profile | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 23 | 1 | Spitfire; **MSV2** |
| 2 | 21 | 0.5 | Red Fury, Mine Dispenser (Shock); **MSV1** |

Both current profiles may fill the Rui Shi row in Zúyŏng Fireteams.

### Monstruckers

**Unit ID:** 1333 · **Slug:** `monstruckers` · **AVA:** 2 · **LI / Mercenary / Irregular**  
`MOV 10-10 | CC 16 | BS 11 | PH 12 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Engineer, Climbing Plus, Deactivator, GizmoKit.

| Profile | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 15 | 0 | Boarding Shotgun, Adhesive Launcher Rifle, E/M Grenades |
| 2 | 12 | 0 | SMG, Chain Rifle, Drop Bears |
| 3 | 15 | 0 | SMG, Chain Rifle, Drop Bears, Armed Turret (AP Rifle) |
| 4 | 16 | 0 | Rifle, Light Shotgun, Akrylat-Kanone, D-Charges; 360º Visor |

Up to two may appear in a Brawlers Fireteam.

### Triphammer, Repurposed Industrial TAG

**Unit ID:** 1569 · **Slug:** `triphammers-repurposed-industrial-tags` · **AVA:** 1 · **TAG / Mercenary / Regular**

Full power: `MOV 15-10 | CC 17 | BS 13 | PH 16 | WIP 12 | ARM 7 | BTS 3 | STR 3 | S 7`. Battle-ravaged: `MOV 10-10 | CC 15 | BS 12 | PH 14 | WIP 12 | ARM 4 | BTS 0 | STR 3 | S 7`. Tactical Awareness, Booty, Transmutation and source industrial TAG package. Includes disabled TurtleMek ancillary.

| Profile | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 2 | 53 | 1.5 | AP Spitfire, Heavy Flamethrower, AP CCW |
| 3 | 52 | 1.5 | AP Spitfire, Chain-colt (+1B), AP CCW |
| 4 | 52 | 0 | Heavy Shotgun, Thunderbolt (+1B), AP CCW |
| 5 | 48 | 0 | Heavy Shotgun, HRL, Panzerfaust (+1B), AP CCW |

All current profiles may fill the Assault Fireteam Triphammer row.

### Bashi Bazouks

**Unit ID:** 325 · **Slug:** `bashi-bazouks` · **AVA:** 4 · **LI / Mercenary / Irregular**  
`MOV 10-10 | CC 16 | BS 11 | PH 10 | WIP 12 | ARM 2 | BTS 0 | W 1 | S 2`. Holomask, Holoprojector, Surprise Attack (-3), Parachutist, Terrain (Zero-G).

| Profile | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 13 | 0 | Contender (+1SD), Boarding Pistol (+1B), CCW |
| 2 | 14 | 0 | T2 Boarding Shotgun, Boarding Pistol (+1B), CCW; BS Attack (AP) |
| 3 | 16 | 0 | Rifle, Light Shotgun, E/M Mine, Boarding Pistol (+1B); Specialist Operative |
| 5 | 14 | 0 | Breaker Rifle, Boarding Pistol (+1B); Specialist Operative |
| 8 | 12 | 0 | SMG, Boarding Pistol (+1B); Specialist Operative |

### Shihab Remotes

**Unit ID:** 316 · **Slug:** `shihab-remotes` · **AVA:** 1 · **REM / Support / Regular**  
`MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | STR 1 | S 3`. 360º Visor, Remote Presence, Total Reaction, Immunity (Shock), Courage.

| Profile | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 23 | 1 | HMG |
| 2 | 18 | 0 | Thunderbolt (+1B) |

### Motorized Bounty Hunters

**Unit ID:** 1565 · **Slug:** `motorized-bounty-hunters` · **AVA:** 2 · **LI / Mercenary / Irregular, Impetuous**  
`MOV 20-15 | CC 17 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 4`. Motorcycle, Booty (ReRoll), Limited Cover, Mimetism (-3), Dodge (+5).

| Profile | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 8 | 0 | Boarding Shotgun, Heavy Riotstopper |
| 2 | 9 | 0 | SMG, Chain-colt (+1B) |
| 3 | 16 | 0.5 | Red Fury, Breaker Pistol |

Up to two are allowed in the Assault Fireteam row.

### Libertos Freedom Fighters

**Unit ID:** 1275 · **Slug:** `libertos-freedom-fighters` · **AVA:** 2 · **LI / Mercenary / Irregular**  
`MOV 10-10 | CC 16 | BS 11 | PH 11 | WIP 12 | ARM 0 | BTS 0 | W 1 | S 2`. Camouflage (1 Use), Forward Deployment (+20), Dogged, Frenzy and aquatic terrain package.

| Profile | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 8 | 0 | SMG, Chain-colt |
| 2 | 9 | 0 | SMG, Chain-colt; Mimetism (-3) |
| 3 | 9 | 1 | Light Shotgun, Shock Mine; Mimetism (-3), Minelayer |
| 4 | 8 | 1 | Light Shotgun, Shock Mine; Minelayer |

### McMurrough, Mercenary Dog-Warrior

**Unit ID:** 283 · **Slug:** `mcmurrough-merc-dog-warrior` · **AVA:** 1 · **WB / Character / Irregular, Impetuous**  
`MOV 15-10 | CC 23 | BS 11 | PH 16 | WIP 14 | ARM 4 | BTS 3 | W 2 | S 6`. Martial Arts L2, Berserk, Super-Jump, Dogged, No Cover, Immunity (ARM), Dodge (+5).

| Profile | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 23 | 0 | Chain Rifle (+1B), Grenades, Smoke Grenades, AP+DA CCW |

### Fiddler, Aristeia!'s ex-toymaker

**Unit ID:** 1564 · **Slug:** `fiddler-aristeia-s-ex-toymaker` · **AVA:** 1 · **LI / Character / Regular**  
`MOV 15-10 | CC 18 | BS 12 | PH 12 | WIP 14 | ARM 1 | BTS 3 | STR 1 | S 2`. Engineer, NWI, GizmoKit, strong Dodge/CC modifiers.

| Profile | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 29 | 0 | **Fiddler FTO**; Contender (+1B), Drop Bears, D-Charges, Breaker Pistol; Super-Jump |
| 2 | 36 | 0 | Same weapons; Climbing Plus; includes 1 Jackbot |
| 3 | 43 | 0 | Same weapons; Climbing Plus; includes 2 Jackbots |

Only profile **1** may fill the Fiddler FTO row in Ghulam Fireteams. Jackbots are disabled subordinate peripherals, not independent roster entries.

### Odalisques

**Unit ID:** 324 · **Slug:** `odalisques` · **AVA:** 4 · **LI / Spec. Trained / Regular**  
`MOV 15-5 | CC 19 | BS 12 | PH 10 | WIP 14 | ARM 2 | BTS 3 | W 1 | S 2`. Sixth Sense, NWI, Natural Born Warrior, Combat Instinct, Discover (PH=15), Stealth.

| Profile | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 4 | 19 | 0 | SMG, Contender, Pulzar (+1B), Pistol |
| 12 | 21 | 0 | As above + Disco Baller |
| 13 | 24 | 0 | Rifle, Light Shotgun, Pulzar; BS Attack (+1B) |
| 14 | 22 | 0 | Boarding Shotgun, Pulzar; BS Attack (+1B) |
| 15 | 26 | 0 | Viral Marksman Rifle, Pulzar (+1B), MULTI Pistol; Marksmanship |
| 16 | 21 | 0 | SMG, Pulzar (+1B), Flash Pulse (+1B); Paramedic, MediKit |

Native Odalisque Fireteams are Duo/Haris.

### Hunzakuts

**Unit ID:** 310 · **Slug:** `hunzakuts` · **AVA:** 2 · **SK / Spec. Trained / Irregular**  
`MOV 10-10 | CC 14 | BS 11 | PH 12 | WIP 14 | ARM 0 | BTS 0 | W 1 | S 2`. Camouflage, Infiltration, Mimetism (-3), Surprise Attack (-3), Stealth.

| Profile | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 18 | 0.5 | Rifle, Grenade Launcher, Shock Mine; Deployable Repeater |
| 2 | 18 | 0.5 | Sniper Rifle, Shock Mine |
| 3 | 19 | 0 | Rifle, Light Shotgun, Shock Mine; Deployable Repeater, Forward Observer |
| 4 | 15 | 0 | Boarding Shotgun, D-Charges; Forward Observer |

### Zhēnchá, Armored Reconnaissance Regiment

**Unit ID:** 1259 · **Slug:** `zhencha` · **AVA:** 1 · **HI / Spec. Trained / Regular**  
`MOV 10-10 | CC 16 | BS 12 | PH 13 | WIP 13 | ARM 3 | BTS 6 | W 1 | S 2`. Camouflage, Infiltration, Mimetism (-3), Surprise Attack (-3), NWI, Stealth, Climbing Plus.

| Profile | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 30 | 0 | Boarding Shotgun, Flash Pulse, D-Charges, Silenced Pistol; Forward Observer |
| 2 | 31 | 0 | SMG, Panzerfaust, Flash Pulse, Shock Mine, Silenced Pistol; Forward Observer |
| 3 | 31 | 0 | SMG, Panzerfaust, Flash Pulse, Silenced Pistol; Deployable Repeater, Forward Observer |
| 4 | 34 | 0.5 | Boarding Shotgun, D-Charges, Silenced Pistol; Hacking Device (Upgrade: Trinity) |
| 5 | 32 | 0.5 | SMG, Panzerfaust, Shock Mine, Silenced Pistol; Minelayer (2) |

### Saito Togan

**Unit ID:** 668 · **Slug:** `saito-togan` · **AVA:** 1 · **SK / Character / Regular**  
`MOV 10-10 | CC 24 | BS 11 | PH 13 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Martial Arts L4, Camouflage, Hidden Deployment, Infiltration, Mimetism (-6), Surprise Attack (-3), Stealth.

| Profile | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 33 | 0 | T2 Boarding Shotgun, Smoke Grenades, Pistol, EXP CCW |

### Valerya Gromoz, Mercenary Hacker

**Unit ID:** 464 · **Slug:** `valerya-gromoz-mercenary-hacker` · **AVA:** 1 · **LI / Character / Regular**  
`MOV 10-10 | CC 15 | BS 11 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`.

| Profile | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 19 | 0.5 | Combi Rifle, Zapper, Pitcher, Pistol, CCW; Hacking Device, Upgrade: Total Control (+1B) |

Explicit Wildcard.

### 112, Emergency Service (Motorized)

**Unit ID:** 1284 · **Slug:** `112-emergency-service-motorized` · **AVA:** 1 · **LI / Support / Regular**  
`MOV 20-10 | CC 16 | BS 11 | PH 12 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 4`. Doctor, Mimetism (-3), Limited Cover, Motorcycle, MediKit.

| Profile | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 4761 | 19 | 0 | Light Shotgun, Smoke Grenade Launcher, Smoke Grenades, Boarding Pistol, CCW |

### 112, Emergency Service

**Unit ID:** 255 · **Slug:** `112-emergency-service` · **AVA:** 2 · **LI / Support / Regular**  
`MOV 10-10 | CC 16 | BS 11 | PH 12 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Doctor, MediKit, Courage.

| Profile | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 11 | 0 | **112 FTO**; Light Shotgun, Boarding Pistol, CCW |

Despite the profile name, the current Dahshat Fireteam chart contains no 112 row and 112 is not a Wildcard; **no Fireteam access is inferred**.

### Highlander Caterans

**Unit ID:** 248 · **Slug:** `highlander-caterans` · **AVA:** 1 · **LI / Spec. Trained / Irregular**  
`MOV 10-10 | CC 22 | BS 12 | PH 13 | WIP 12 | ARM 0 | BTS 0 | W 1 | S 2`. Camouflage (1 Use), Mimetism (-3), Surprise Attack (-3), Stealth, Climbing Plus.

| Profile | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 21 | 1 | T2 Sniper Rifle |
| 2 | 21 | 0.5 | AP Sniper Rifle |
| 3 | 23 | 1 | T2 Sniper Rifle; Forward Deployment (+10) |

### Diggers, Armed Prospectors

**Unit ID:** 1568 · **Slug:** `diggers-armed-prospectors` · **AVA:** 2 · **HI / Mercenary / Regular, Impetuous**  
Full power `MOV 10-10 | CC 21 | BS 11 | PH 13 | WIP 12 | ARM 3 | BTS 0 | W 2 | S 2`; battle-ravaged BS10/PH12/ARM2. Booty, Natural Born Warrior, No Cover, Transmutation and strong CC package.

| Profile | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 18 | 0 | Rifle, Light Shotgun, Grenades, Pistol, AP CCW |
| 2 | 14 | 0 | Chain Rifle (+1B), Grenades, Pistol, AP CCW |

Explicit Wildcard; current chart comment `(Brawler)`.

### Warcors, War Correspondents

**Unit ID:** 50 · **Slug:** `warcors-war-correspondents` · **AVA:** 1 · **LI / Mercenary / Irregular**  
`MOV 10-10 | CC 11 | BS 9 | PH 11 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Journalist.

| Profile | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CCW (-3); 360º Visor |
| 2 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CCW (-3); Sixth Sense |

### Traktor Mul Unit

**Unit ID:** 257 · **Slug:** `traktor-mul` · **AVA:** 2 · **REM / Support / Regular**  
`MOV 10-10 | CC 13 | BS 10 | PH 9 | WIP 12 | ARM 2 | BTS 0 | STR 1 | S 4`. Baggage, ECM: Guided (-6), Remote Presence, Courage.

| Profile | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 5 | 0 | Deactivator; PARA CCW (-3) |
| 2 | 9 | 1 | Katyusha MRL; **BS Attack (Guided)** |
| 3 | 14 | 1 | Uragan MRL; **BS Attack (Guided), Total Reaction** |

### Fanous Remotes

**Unit ID:** 318 · **Slug:** `fanous-remotes` · **AVA:** 3 · **REM / Support / Regular**  
`MOV 15-15 | CC 13 | BS 8 | PH 11 | WIP 13 | ARM 0 | BTS 3 | STR 1 | S 3`. Repeater, Mimetism (-3), Remote Presence, Courage.

| Profile | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 7 | 0 | Flash Pulse, PARA CCW (-3) |

### Dozers, Field Engineers

**Unit ID:** 256 · **Slug:** `dozers-field-engineers` · **AVA:** 1 · **LI / Support / Regular**  
`MOV 10-10 | CC 14 | BS 11 | PH 11 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Engineer, Deactivator, GizmoKit, Courage.

| Profile | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 13 | 0 | Rifle, D-Charges |
| 3 | 14 | 0 | Rifle, Blitzen, D-Charges |
| 4 | 14 | 0 | Rifle, D-Charges; Deployable Cover |
| 5 | 15 | 0 | Rifle, D-Charges; Armed Turret (Rifle) |

### Authorized Bounty Hunters

**Unit ID:** 49 · **Slug:** `authorized-bounty-hunters` · **AVA:** 4 · **LI / Mercenary / Regular**  
`MOV 10-10 | CC 16 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Booty (ReRoll), Stealth.

| Profile | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 15 | 0 | Combi Rifle |
| 2 | 12 | 0 | Boarding Shotgun, Heavy Riotstopper |
| 3 | 19 | 0.5 | Sniper Rifle, Breaker Pistol (+1B) |
| 4 | 21 | 1 | Spitfire, Boarding Pistol |
| 5 | 12 | 0 | SMG, Akrylat-Kanone, Breaker Pistol |
| 6 | 20 | 0.5 | Red Fury |

Explicit Wildcard, maximum four in the chart.

### Kum Motorized Troops

**Unit ID:** 313 · **Slug:** `kum-motorized-troops` · **AVA:** 4 · **WB / Line / Irregular, Impetuous**  
`MOV 20-15 | CC 22 | BS 11 | PH 13 | WIP 14 | ARM 1 | BTS 0 | W 1 | S 4`. Motorcycle, Mimetism (-3), Dogged, No Cover, Dodge (+5); Smoke Grenade Launcher on chassis.

| Profile | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1123 | 6 | 0 | Chain Rifle, Smoke Grenades, Pistol, Shock CCW |
| 1124 | 7 | 0 | Light Shotgun, Smoke Grenades, Pistol, DA CCW |
| 1125 | 9 | 0 | Boarding Shotgun, Smoke Grenades, Pistol, E/M CCW |
| 1126 | 11 | 0 | Rifle, Light Shotgun, Smoke Grenades, Pistol, E/M CCW |

### Zellenkrieger

**Unit ID:** 1747 · **Slug:** `zellenkrieger` · **AVA:** 1 · **WB / Support / Irregular, Impetuous**  
`MOV 10-10 | CC 23 | BS 10 | PH 13 | WIP 12 | ARM 1 | BTS 3 | STR 1 | S 2`. Berserk, Natural Born Warrior, MetaChemistry (ReRoll), No Cover, strong CC/Dodge modifiers.

| Profile | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 8 | 0 | Light Shotgun, Smoke Grenades, Heavy Pistol, DA CCW |
| 2 | 8 | 0 | Pulzar, Smoke Grenades, Heavy Pistol (+1B), DA CCW |
| 3 | 8 | 0 | **FTO**; Pulzar (+1B), Heavy Pistol (+1B), DA CCW; **no Smoke** |

Only profile **3** may fill the Zellenkrieger FTO row in Brawlers Fireteams.

### Brawlers, Mercenary Enforcers

**Unit ID:** 987 · **Slug:** `brawlers-mercenary-enforcers` · **AVA:** 5 · **MI / Spec. Trained / Regular**  
`MOV 10-10 | CC 17 | BS 12 | PH 11 | WIP 12 | ARM 2 | BTS 3 | W 1 | S 2`. Sixth Sense.

| Profile | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 15 | 0 | Rifle, Light Shotgun (+1B) |
| 2 | 15 | 1.5 | Heavy Rocket Launcher, Assault Pistol; X-Visor |
| 3 | 25 | 1.5 | MULTI Sniper Rifle, AP Mine; **MSV2** |
| 5 | 16 | 0.5 | SMG, Cybermine; Hacking Device |
| 6 | 19 | 0 | Rifle, Light Shotgun (+1B), D-Charges; Engineer, GizmoKit/Deactivator |
| 7 | 19 | 0 | Rifle, Light Shotgun (+1B); Doctor, MediKit |
| 9 | 15 | 0 | Rifle, Light Shotgun (+1B); **Lieutenant** |

Native Brawlers Fireteams are Duo/Haris/Core.

### Zúyŏng Invincibles

**Unit ID:** 127 · **Slug:** `zuy-ng-invincibles` · **AVA:** 5 · **HI / Line / Regular**  
`MOV 15-5 | CC 17 | BS 13 | PH 12 | WIP 13 | ARM 3 | BTS 3 | W 2 | S 2`. Number 2, Dodge (+2.5).

| Profile | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 2 | 26 | 0 | MULTI Rifle, Breaker Pistol (+1B); TinBot Firewall (-6) |
| 3 | 30 | 1.5 | HMG, Breaker Pistol (+1B) |
| 4 | 22 | 0 | Boarding Shotgun, E/Mitter, Breaker Pistol (+1B) |
| 5 | 24 | 0 | MULTI Rifle, Breaker Pistol (+1B) |
| 6 | 31 | 1.5 | Missile Launcher, Light Shotgun, Breaker Pistol (+1B) |
| 8 | 27 | 0 | Combi Rifle, Breaker Pistol (+1B); **Tactical Awareness**, TinBot Firewall (-6) |
| 11 | 26 | 0 | MULTI Rifle, Breaker Pistol (+1B); Paramedic, MediKit |
| 12 | 33 | 1.5 | HMG, Breaker Pistol (+1B); **Tactical Awareness** |

Native Zúyŏng Fireteams are Haris/Core; Rui Shi may join according to the canonical chart.

### Father Lucien Sforza

**Unit ID:** 198 · **Slug:** `father-lucien-sforza` · **AVA:** 1 · **MI / Character / Regular**  
`MOV 10-10 | CC 19 | BS 13 | PH 11 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. X-Visor, Combat Instinct, Stealth, NCO, Dogged, Religious Troop, BS Attack (+1SD).

| Profile | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 26 | 0 | Viral Rifle, Adhesive Launcher Rifle, Nanopulser, Heavy Pistol, PARA CCW (-9); Holoprojector, Surprise Attack, Forward Deployment (+10) |
| 2 | 23 | 0 | **Sforza FTO**; same base weapons |
| 3 | 26 | 0 | **Sforza FTO**; same base weapons; Albedo (-6) |

Only profiles **2–3** use the explicit `SFORZA FTO` Wildcard row.

### Najjarun Engineer

**Unit ID:** 314 · **Slug:** `najjarun-engineers` · **AVA:** 1 · **LI / Support / Regular**  
`MOV 10-10 | CC 14 | BS 11 | PH 10 | WIP 14 | ARM 1 | BTS 0 | W 1 | S 2`. Engineer, Deactivator, GizmoKit, Courage.

| Profile | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 15 | 0 | Rifle, Light Shotgun, D-Charges |
| 2 | 16 | 0 | Same; Deployable Cover |
| 3 | 17 | 0 | Same; Armed Turret (Rifle) |

### Kameel Remotes

**Unit ID:** 334 · **Slug:** `kameel-remotes` · **AVA:** 2 · **REM / Support / Regular**  
`MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 2 | BTS 3 | STR 1 | S 4`. Baggage, Remote Presence, Courage.

| Profile | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 8 | 0 | Deactivator, Repeater |
| 2 | 14 | 0.5 | **EVO Hacking Device** |
| 3 | 16 | 0 | Rifle, Light Shotgun, Repeater; **Total Reaction** |

### Húláng Shocktroopers

**Unit ID:** 1257 · **Slug:** `hulang-shocktroopers` · **AVA:** 1 · **HI / Veteran / Regular**  
`MOV 15-5 | CC 22 | BS 12 | PH 12 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`. Martial Arts L2, Berserk, Mimetism (-6), Specialist Operative, Stealth, NWI, Combat Instinct.

| Profile | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 38 | 0.5 | **FTO-2**; Combi Rifle (+1B), Light Flamethrower, D-Charges, AP Mine, Monofilament CCW; FD +20, Minelayer |
| 2 | 38 | 0 | **FTO-2**; SMG (+1B), E/Mitter, D-Charges, CrazyKoala, Monofilament CCW; FD +20, Minelayer |
| 3 | 31 | 0 | **FTO**; SMG (+1B), E/Mitter, D-Charges, Disco Baller, Monofilament CCW |
| 4 | 33 | 0 | **FTO**; Combi Rifle (+1B), Light Flamethrower, D-Charges, Monofilament CCW |

The current Dahshat Fireteam chart has **no Húláng row** and Húláng is not a Wildcard. FTO/FTO-2 names alone therefore grant **no current Dahshat Fireteam access**.

### Al Fasid Regiment

**Unit ID:** 343 · **Slug:** `al-fasid-regiment` · **AVA:** 1 · **HI / Veteran / Regular**  
`MOV 10-10 | CC 17 | BS 13 | PH 14 | WIP 14 | ARM 5 | BTS 6 | W 2 | S 5`. Albedo (-3), Minelayer, Sixth Sense, Combat Instinct, Warhorse.

| Profile | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 50 | 1.5 | HMG, Grenade Launcher, Smoke Grenade Launcher, Shock Mine, Heavy Pistol; BS Attack (SR-1) |
| 2 | 44 | 1.5 | HRL, SMG, Shock Mine, Heavy Pistol; BS Attack (+1SD) |

Both current profiles may fill the Fasid row in Assault Fireteams.

### Ghulam Infantry

**Unit ID:** 301 · **Slug:** `ghulam-infantry` · **AVA:** 6 · **LI / Line / Regular**  
`MOV 10-10 | CC 14 | BS 11 | PH 10 | WIP 14 | ARM 1 | BTS 0 | W 1 | S 2`. Terrain (Desert).

| Profile | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 11 | 0 | Rifle, Light Shotgun |
| 2 | 20 | 1 | HMG |
| 4 | 17 | 1.5 | Missile Launcher |
| 7 | 16 | 0.5 | Rifle, Light Shotgun; Hacking Device |
| 8 | 15 | 0 | Rifle, Light Shotgun; Doctor (+3), MediKit |
| 9 | 12 | 0 | Rifle, Light Shotgun, Flash Pulse; Forward Observer |
| 10 | 13 | 0 | Rifle, Light Shotgun, E/M Mine; Deployable Repeater |
| 11 | 11 | 0 | Rifle, Light Shotgun; **Lieutenant** |
| 14 | 15 | 1 | Rifle, Grenade Launcher, Smoke Grenade Launcher; **NCO** |
| 18 | 12 | 0 | Rifle, Light Shotgun, Panzerfaust; Number 2 |
| 19 | 15 | 0 | Rifle, Light Shotgun; **Lieutenant (+1 Command Token)** |

Native Ghulam Fireteams are Haris/Core.

## Lieutenant and order-control index

| Unit/profile | Function |
|---|---|
| Ghulam profile 11 | Lieutenant, 11 pts / 0 SWC |
| Ghulam profile 19 | Lieutenant +1 Command Token, 15 pts / 0 SWC |
| Brawler profile 9 | Lieutenant, 15 pts / 0 SWC |
| Ghulam profile 14 | NCO; Smoke Grenade Launcher |
| Sforza | NCO on all current profiles |
| Maghariba Guard | Tactical Awareness on all current profiles |
| Triphammer | Tactical Awareness on all current profiles |
| Zúyŏng profiles 8 and 12 | Tactical Awareness |

The current standard Dahshat roster does not expose a normal Chain of Command profile in this snapshot.

## Hacking and network index

### Hackers

- **Hacking Device:** Ghulam profile 7; Brawler profile 5; Zhēnchá profile 4; Valerya Gromoz.
- **EVO Hacking Device:** Kameel profile 2.
- No standard Dahshat KHD profile is present in the current main roster snapshot.
- Optional Rumbler Spec-Ops can take a Hacking Device when that mode is enabled.

### Network / projection

- **Pitcher:** Valerya Gromoz.
- **Deployable Repeaters:** Ghulam profile 10; Hunzakut profiles 1 and 3; Zhēnchá profile 3.
- **Repeaters:** Rafiq; Rui Shi; Fanous; Kameel profiles 1 and 3.
- **Sensor:** Rafiq.
- **Guided:** Shaytaniyah profile 1; Traktor Mul profiles 2 and 3.
- **Disco Baller:** Odalisque profile 12; Húláng profile 3.
- **Cybermine:** Brawler Hacker.

## Deployment / marker-state index

- **Combat Jump / Parachutist:** Bashi Bazouks have Parachutist plus Holoprojector; no standard Combat Jump unit is present.
- **Hidden Deployment:** Saito Togan.
- **Camouflage / infiltration:** Hunzakuts; Zhēnchá; Saito; Libertos (1-use camouflage).
- **Forward Deployment:** Libertos (+20), Cateran profile 3 (+10), Húláng profiles 1–2 (+20), Sforza non-FTO profile (+10).
- **Holoprojector / Holomask:** Bashi Bazouks; Lù Duān; Sforza profile 1.
- **Fast attack:** Kum; Motorized Bounty Hunters; motorized 112; McMurrough; Maghariba; airborne Bashi.

## Vision-control and sensor index

- **Smoke:** McMurrough; Saito; Kum; 112 Motorized; Al Fasid profile 1 Smoke Grenade Launcher; Ghulam NCO profile 14 Smoke Grenade Launcher; Zellenkrieger profiles 1–2.
- **MSV2:** Rui Shi profile 1; Brawler MULTI Sniper profile 3.
- **MSV1:** Lù Duān; Rui Shi profile 2.
- **Sensor:** Rafiq.
- Zellenkrieger **FTO profile 3 has no Smoke**; do not project the smoke capability from profiles 1–2 onto the Fireteam profile.

## Canonical Fireteam definitions

Current chart limit: **1 Core, 1 Haris, unlimited Duos** (`DUO: 256` source sentinel).

### FT-01 — Ghulam Fireteams

**Types:** Haris, Core  
**Anchor:** Ghulam has source `min: 1`.

| Member | Unit ID | Required | Min | Max | Counts as / comment | Profile restriction |
|---|---:|---|---:|---:|---|---|
| Ghulam | 301 | no | 1 | 5 | — | all |
| Fiddler | 1564 | no | 0 | 1 | `FTO` | **profile 1 only** |
| Rumbler Spec-Ops | 1925 | no | 0 | 1 | `Spec-Ops` | optional mode only |

### FT-02 — Brawlers Fireteams

**Types:** Duo, Haris, Core  
**Anchor:** Brawler has source `min: 1`.

| Member | Unit ID | Required | Min | Max | Counts as / comment | Profile restriction |
|---|---:|---|---:|---:|---|---|
| Brawler | 987 | no | 1 | 5 | — | all |
| Monstrucker | 1333 | no | 0 | 2 | — | all |
| Zellenkrieger | 1747 | no | 0 | 1 | `FTO` | **profile 3 only** |
| Rumbler Spec-Ops | 1925 | no | 0 | 1 | `Spec-Ops` | optional mode only |

### FT-03 — Odalisques Fireteams

**Types:** Duo, Haris  
**Anchor:** Odalisque has source `min: 1`.

| Member | Unit ID | Required | Min | Max | Counts as / comment | Profile restriction |
|---|---:|---|---:|---:|---|---|
| Odalisque | 324 | no | 1 | 3 | — | all |

### FT-04 — Zúyŏng Fireteams

**Types:** Haris, Core  
**Anchor:** Zúyŏng has source `min: 1`.

| Member | Unit ID | Required | Min | Max | Counts as / comment | Profile restriction |
|---|---:|---|---:|---:|---|---|
| Zúyŏng | 127 | no | 1 | 5 | — | all |
| Rui Shi | 159 | no | 0 | 1 | — | all |

### FT-05 — Assault Fireteams

**Type:** Duo

The current source has unusual raw semantics: **every row is `required: true` while every row also has `min: 0`**. Preserve both fields exactly. Do not rewrite the chart into a guessed anchor requirement.

| Member | Unit ID | Required | Min | Max | Counts as / comment | Profile restriction |
|---|---:|---|---:|---:|---|---|
| Al Fasid | 343 | **yes** | 0 | 1 | — | all |
| Rafiq Remote | 315 | **yes** | 0 | 1 | `FTO` | **profile 3 only** |
| Maghariba Guard | 309 | **yes** | 0 | 1 | — | all |
| Triphammer | 1569 | **yes** | 0 | 1 | — | all |
| Motorized Bounty Hunter | 1565 | **yes** | 0 | 2 | — | all |

This table records Army’s source representation; normal Fireteam size/type rules still govern the actual Duo formed from eligible selections.

### Wildcards

| Unit | Unit ID | Counts as / comment | Max | Profile restriction | Notes |
|---|---:|---|---:|---|---|
| Authorized Bounty Hunter | 49 | — | 4 | all | explicit Wildcard row |
| Father Lucien Sforza | 198 | `FTO` | 1 | **profiles 2–3 only** | explicit Wildcard row |
| Miranda Ashcroft | 51 | `(Odalisque)` | 1 | all | explicit Wildcard row |
| Valerya Gromoz | 464 | — | 1 | all | explicit Wildcard row |
| Digger | 1568 | `(Brawler)` | 2 | all | explicit Wildcard row |

`Rumbler Spec-Ops` is **not** a global Wildcard in Dahshat. It is an optional-mode member explicitly listed only in the Ghulam and Brawlers Fireteam families.

Do not import additional Wildcards or Fireteam permissions from older Dahshat references, Haqqislam, Yu Jing, Ikari, Druze Bayram Security, or another NA2 sectorial.

## Unit → Fireteam access index

| Unit | Fireteam | Types | Access | Profile restriction | Min–max / notes |
|---|---|---|---|---|---|
| Ghulam | FT-01 | Haris/Core | native anchor | all | 1–5 |
| Fiddler | FT-01 | Haris/Core | FTO member | **profile 1** | 0–1 |
| Rumbler Spec-Ops | FT-01 | Haris/Core | optional member | Spec-Ops mode | 0–1 |
| Brawler | FT-02 | Duo/Haris/Core | native anchor | all | 1–5 |
| Monstrucker | FT-02 | Duo/Haris/Core | native member | all | 0–2 |
| Zellenkrieger | FT-02 | Duo/Haris/Core | FTO member | **profile 3** | 0–1 |
| Rumbler Spec-Ops | FT-02 | Duo/Haris/Core | optional member | Spec-Ops mode | 0–1 |
| Odalisque | FT-03 | Duo/Haris | native anchor | all | 1–3 |
| Zúyŏng | FT-04 | Haris/Core | native anchor | all | 1–5 |
| Rui Shi | FT-04 | Haris/Core | native member | all | 0–1 |
| Al Fasid | FT-05 | Duo | Assault row | all | raw required=true, min0, max1 |
| Rafiq | FT-05 | Duo | Assault FTO row | **profile 3** | raw required=true, min0, max1 |
| Maghariba | FT-05 | Duo | Assault row | all | raw required=true, min0, max1 |
| Triphammer | FT-05 | Duo | Assault row | all | raw required=true, min0, max1 |
| Motorized Bounty Hunter | FT-05 | Duo | Assault row | all | raw required=true, min0, max2 |
| Authorized Bounty Hunter | Wildcard | permitted teams | Wildcard | all | max 4 |
| Sforza | Wildcard | permitted teams | FTO Wildcard | **profiles 2–3** | max 1 |
| Miranda Ashcroft | Wildcard | permitted teams | Wildcard, counts as Odalisque | all | max 1 |
| Valerya Gromoz | Wildcard | permitted teams | Wildcard | all | max 1 |
| Digger | Wildcard | permitted teams | Wildcard, counts as Brawler | all | max 2 |

If this reverse index ever conflicts with the canonical Fireteam tables above, the canonical tables win.

## Explicit no-access FTO labels

The following source profiles are labelled FTO/FTO-2 but have no corresponding current Dahshat Fireteam-chart row and are not covered by an explicit Wildcard rule:

- `112 Emergency Service` profile 1 (`112 FTO`)
- `Húláng Shocktroopers` profiles 1–2 (`FTO-2`) and profiles 3–4 (`FTO`)

Do **not** infer Dahshat Fireteam access from those profile names alone.

## Optional-mode units

### Rumbler Spec-Ops

**Unit ID:** 1925 · **Slug:** `rumbler-spec-ops` · **Mode:** Infinity Spec-Ops · **Normal Dahshat status:** optional only.  
Unlike Ikari, Dahshat’s current chart does not make Rumbler a global Wildcard. When Spec-Ops mode is enabled, one Rumbler may join **Ghulam Fireteams** and one row is also available in **Brawlers Fireteams**; normal uniqueness/mode rules still apply.

| Profile | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 28 | 1 | HMG, D-Charges, Pistol, CCW |
| 2 | 28 | 1 | AP Spitfire, D-Charges, Pistol, CCW |
| 3 | 23 | 0 | MULTI Rifle, Pistol, CCW; Specialist Operative, GizmoKit |
| 4 | 26 | 0.5 | AP Combi Rifle, D-Charges, Pistol, CCW; Hacking Device |
| 5 | 23 | 0 | MULTI Rifle, Flash Pulse, D-Charges, Pistol, CCW; Forward Observer |
| 6 | 23 | 0 | AP Combi Rifle, D-Charges, Pistol, CCW; Paramedic, MediKit |

### NA2 Team-Ops

**Unit ID:** 1939 · **Slug:** `na2-team-ops` · **Mode:** Team-Ops · **Normal Dahshat status:** optional only.  
Contains Rumbler-1, Rumbler Heavy and Gort SpecBot Team-Ops profiles. It is not counted as an ordinary matched-play Dahshat roster entry and is not automatically substituted for Rumbler Spec-Ops in the Fireteam chart.

## Source relations and identity constraints

The current Dahshat snapshot has three top-level relation records:

1. **Grouped profile relation:** Traktor Mul profile 2 (`unit 257/profile 2`), Dozer profile 1 (`unit 256/profile 1`), and Kuryer profile 2 (`unit 1524/profile 2`), with source `min:1`, `max:2`, `group:true`.
   - Kuryer ID `1524` is **not present in the current `7.26246.159` Dahshat roster/resume** even though the relation remains.
   - Earlier source revisions identify ID 1524 as **Kuryer Unit**.
   - Treat this as a **partially dangling/stale source relation**, not as permission to select Kuryer. With the absent member excluded, it does not create a new roster entry or Fireteam permission.
2. **Sforza identity relation:** main Sforza ID `198` and Reinforcement Sforza ID `1692`, source max 1. Do not duplicate Sforza across Main/Reinforcement selections.
3. **Miranda identity relation:** main Miranda ID `51` and Reinforcement Miranda ID `1693`, source max 1. Do not duplicate Miranda across Main/Reinforcement selections.

IDs `1692` and `1693` are the Contracted Back-up / Reinforcement forms of Sforza and Miranda respectively; they are not extra Main roster entries.

## Reinforcements boundary

Army links Dahshat Company to Reinforcement roster ID **999**. Reinforcement-only profiles, AVA and Fireteam permissions remain outside this Main reference. Do not merge Reinforcement Fireteam permissions into the Main chart above.

The source identity relations for Sforza and Miranda explicitly cross this boundary and enforce character uniqueness; that does not otherwise merge the two rosters.

## Derived tactical index

This section is analytical and non-authoritative; source profile data and the canonical Fireteam chart above take precedence.

| Block / tag | Strong Dahshat candidates |
|---|---|
| Group 2 | Fanous; Warcor; Kameel EVO/TR; Traktor Mul; Shihab; Irregular Hunzakuts/Libertos/Bashi; cheap bikes |
| Long-range attack | Maghariba; Zúyŏng HMG/TacAware HMG; Rui Shi; Al Fasid HMG; Triphammer |
| Mid-range attack | Zúyŏng; Rui Shi; Lù Duān; Odalisques; Húláng; Sforza; Maghariba |
| Long-range ARO | Shaytaniyah; Traktor Mul Uragan TR/Guided; Shihab TR; Brawler MSV2 sniper/HRL; Cateran; Zúyŏng ML; Ghulam ML |
| Mid-range ARO | Al Fasid HRL; Lù Duān; Rafiq; Brawlers; Odalisques |
| Close assault | McMurrough; Saito; Húláng; Kum; Zellenkrieger; Diggers; Odalisques |
| Specialist | Ghulam HD/Doctor/FO; Brawler HD/Engineer/Doctor; Rafiq FO/Sensor; Hunzakut FO; Zhēnchá FO/HD; Valerya; 112; Fiddler; Dozer; Najjarun; Monstrucker; Odalisque Paramedic; Bashi specialists |
| Cheerleader | Ghulam; Fanous; Warcor; cheap Authorized Bounty Hunters; Kameel |
| TAG + support | Maghariba or Triphammer + Dozer/Najjarun/Monstrucker/Fiddler + Nasmat where applicable |
| REM + support | Rafiq/Rui Shi/Lù Duān/Shaytaniyah/Shihab/Fanous/Traktor/Kameel + Engineers |
| DZ defense | Shihab; Kameel TR; Traktor Uragan; Brawler ARO profiles; Ghulam/Zúyŏng missiles; Warcor |
| Midfield defense | Hunzakuts; Libertos; Zhēnchá; Saito; Húláng; Diggers |
| Midfield specialist | Hunzakut FO; Zhēnchá FO/HD; Húláng Specialist; Libertos pressure; Rafiq when advanced |
| Warband | McMurrough; Kum; Zellenkrieger; Diggers; Motorized Bounty Hunters |
| Airborne troops | Bashi Bazouks |
| Enemy-DZ attacker | Bashi; McMurrough; Saito; Húláng; Kum; fast MBH |
| Network projection | Valerya Pitcher; Ghulam/Hunzakut/Zhēnchá deployable repeaters; Fanous/Rafiq/Rui Shi/Kameel repeaters |
| Vision control | McMurrough/Saito/Kum/112M/Fasid/Ghulam/Zellen smoke; Rui Shi/Brawler MSV2 exploitation |
| Hacker | Ghulam; Brawler; Zhēnchá; Valerya; Kameel EVO |
| KHD | None in current standard Main roster |
| Tech-counter | Rafiq Sensor; Fiddler/Dozer/Najjarun/Monstrucker Engineers; Nasmat servant support |
| Guided package | Shaytaniyah profile 1 or Traktor Mul profiles 2–3 + FO/Spotlight network |
| Baggage support | Maghariba; Traktor Mul; Kameel — useful with disposable/deployable-heavy builds |

## Source-normalization and validation notes

- Standard roster count is **39 normal entries + 2 optional-mode entries**.
- Generic `merc-*` catalogue objects with empty `factions` arrays are excluded even though the aggregate dataset contains them. Explicit faction-`908` mercenary/guest entries are retained.
- Source `DUO: 256` is normalized as effectively unlimited Duos.
- Ghulam, Brawler, Odalisque and Zúyŏng anchors use positive source `min` values despite `required:false`; those minimums are preserved.
- Assault Fireteam rows all use the unusual combination `required:true, min:0`. Those raw facts are preserved rather than normalized into a guessed anchor rule.
- Fiddler Fireteam access is **profile 1 only**.
- Zellenkrieger Fireteam access is **profile 3 only**, and that FTO profile lacks Smoke.
- Rafiq Assault access is **profile 3 only**.
- Sforza Wildcard access is **profiles 2–3 only**; non-FTO profile 1 does not inherit it.
- Foot 112 and all current Húláng profiles carry FTO/FTO-2 names but have no Dahshat chart row; no Fireteam access is inferred.
- Rumbler Spec-Ops is not a global Dahshat Wildcard; it is an optional named member of Ghulam and Brawlers teams only.
- Shaytaniyah profile 1 is Guided; profile 3 has Missile Launcher (+1B) but no Guided skill.
- Disabled Jandab, Jackbot and TurtleMek subordinate entries are not counted as independent roster selections.
- The dangling Kuryer relation is recorded as source data but does not restore Kuryer to the current roster.
- Sforza and Miranda Main/Reinforcement identity relations are preserved.
- Main and Reinforcement roster `999` remain separate.

## Tactical research — Dahshat Company (reviewed 2026-10-23)

**This is tactical analysis, not a rules update.** Dedicated deep-dive episodes [W1/W2] and [R1] predate N5; [N1] is a transcript-reviewed N5 Dahshat battle report; [T1/H1/Y1] cover current shared TAG and REM mechanics. **The verified N5.3 Army 7.26246.159 tables above override every older claim about profiles, prices, skills, LT choices and Fireteams.** No long-form post-October-2025 Dahshat-only N5 faction focus was verified in the searched MCP catalogue, so the edition caveat matters.

### Winning concept: a good gun with numerous cheap second plans

| Plan / package | Why it wins Orders or objectives | Why it can fail |
|---|---|---|
| **8–9pt Libertos, 15–19pt Hunzakuts, 6pt Kum, 23pt McMurrough** | Multiple inexpensive Camo/smoke/close assault trades force enemy attention away from the primary gun. Dahshat can field these while still affording costly TAG/HI. [W1, R1, N1] | They are **Irregular**; the 15-trooper cap and limited Regular Orders can hurt more than points. Avoid paying for every excellent cheap attacker in one list. |
| **Zúyŏng + Rui Shi Core/Haris** | **33/1.5 Zúyŏng Tactical Awareness HMG**, **26/0 or 27/0 TinBot Firewall(-6)**, and **23/1 Rui Shi MSV2 Spitfire** generate reliable high-burst gunfighting, including through smoke. Rui Shi is legally joinable **only in the Zúyŏng family** here. [W1, R1, Y1] | Hackable HI and a **one-STR Rui Shi** put too many points/orders in one vulnerable formation. Consider a small Haris rather than automatically paying for a five-person Core. |
| **Ghulam LT/NCO/Valerya support** | **11/0 Ghulam LT**, **15/0 LT +1 Command Token**, **15/1 NCO smoke grenade launcher**, **16/0.5 Ghulam HD**, **15/0 Doctor(+3)** and **19/0.5 Valerya Wildcard HD/Pitcher** provide Regular Orders, smoke, protected missions and a projected hacking network. [W1, R1, N1] | These are mainly BS11 support troopers, not a premium frontline Core. Support the TAG, Rui Shi or midfield plan instead of pretending the Ghulam HMG replaces them. |
| **Brawler specialist defense** | **16/0.5 Sixth Sense hacker**, **25/1.5 MSV2 sniper**, **15/1.5 X-Visor HRL**, **14/0 Regular Digger** and **12–16pt Monstrucker Engineer** form complementary Brawler Duo/Haris/Core combinations. [W1, W2] | A WIP12 hacker/BS12 gun remains mediocre against dedicated opponents; Monstruckers are Irregular. Only one Core and one Haris total. |
| **Maghariba versus Triphammer** | **Maghariba 71–72/1.5, BS14/ARM8/TacAware** is a sustained ranged attack and lane-control center; **Triphammer 48/0** is a cheaper zero-SWC TAG with ancillary specialist. [T1, H1] | Maghariba is **Silhouette 8**, hard to conceal/manoeuvre on tight boards; Triphammer is lower-quality BS13/BTS3. Either costs troops and objectives. |

**Build-order check:** Have (1) main active shooter, (2) protected Lieutenant and useful Regular Orders, (3) an FO or infiltrating objective specialist, (4) long- and close-range armor answers, (5) smoke/MSV or hacking control if the list relies on it, and (6) a second attack lane after the primary piece is lost. [R1] argues **trooper slots are often scarcer than points**: do not add cheap troops merely because you can afford them.

### Individual unit value and opposing arguments

- **Libertos, AVA2:** **8/0** chain-colt/SMG is a cheap forward trade; **9/0 Mimetism(-3)** costs one point more and makes the Camo/Forward Deployment (+20) nuisance harder to remove. **9/1 Mimetism(-3) Minelayer** trades precious SWC for a prepared board-defense layer. [W1/R1] favor Mimetism almost universally; **counter:** at the 15-slot cap, a Regular specialist or cheaper 8pt profile can be more valuable than a second disposable Irregular.
- **McMurrough (23/0) and Kum (6–11/0):** Dog-Warrior's PH16, smoke, Super-Jump, Chain Rifle(+1B), Dogged and AP+DA CCW create a direct route to a valuable target and **smoke for the Rui Shi/Brawler MSV2**; bikes add fast smoke and cheap trades. [W1] calls him central to aggressive Dahshat. **Counter:** speculative charges spend Orders exposing the piece before it reaches the high-value target. Motorized Bounty Hunters (8–16) compete for Irregular slots; **motorized 112** instead buys a **Regular Doctor**, mobility and objectives.
- **Hunzakut vs Zhēnchá:** **15/0 Hunzakut FO** or **19/0 FO + deployable repeater**, WIP14/Infiltration/Camo, buys cheap prepositioned objectives and hacking projection **but is Irregular**. **30–34pt Zhēnchá** buys a **Regular**, NWI, BTS6 Camo/Infiltration specialist and stronger late-turn durability, with FO, deployable repeater, minelayer or HD. If the mission needs the specialist alive in round 3, Zhēnchá justifies the cost. [W1/N1]
- **Critical hacking edition change:** [R1]'s N4 statement **“no Trinity anywhere” is no longer true**. The current roster still contains **NO KHD profile**; however **Zhēnchá option 4 is a 34/0.5 Hacking Device with Trinity upgrade**. Ghulam, Brawler and Valerya have ordinary HD; Kameel can take EVO. An HD with Trinity is **not** a KHD, and a KHD is **not** needed to Spotlight. Flag the difference rather than preserving the old absolute claim. [N1]
- **Valerya (19/0.5):** WIP14 HD, Pitcher, Total Control(+1B), Wildcard: useful Hacking/Spotlight/repeater network at low cost. [W1] calls her the lynchpin; [R1] calls Dahshat's hacking *thin*, because most hackers are lightly protected and there is no native KHD. Both views hold conditionally: plan a **specific** repeater + FO/Spotlight + attack rather than buying guided artillery on autopilot.
- **Saito (33/0), Húláng (31–38):** Saito has Hidden Deployment, Infiltration, Mimetism(-6), smoke, T2 shotgun and EXP melee for assassination, **but no current specialist/FO skill**. Húláng brings Mimetism(-6), NWI, Specialist Operative, Monofilament and options for FD+20 mines or a cheaper Disco Baller. [W2] likes high-ceiling offense; **counter:** premium midfield tools compete with cheaper objective-taking Hunzakuts and resilient Zhēnchá. **No Húláng may enter Dahshat Fireteams despite its FTO labels**.
- **Fiddler (29–43):** **29/0 FTO Engineer with Super-Jump** can join **Ghulam Core/Haris only**, while **36/43 standalone Jackbot variants** are synchronized assault/repair packages but do **not** join Ghulam Fireteams. [R1] praises the Jackbots for breaking a position then exploiting it; **counter:** FTO at 29 can offer a protected 0-SWC specialist while keeping points for Libertos/REM backup. Peripherals are not independent Orders.
- **Brawlers + Diggers + Monstruckers:** Sixth Sense HD and smoke-shooting **MSV2 MULTI sniper** give quality support; **14pt Regular Digger Wildcard counts as Brawler** and handles corner CC/templates. Monstruckers can repair TAGs/REMs and join Brawler family, but their own order is Irregular. [W1/W2] praise role coverage; **counter:** a maximal Brawler Core has weaker active shooting than a Zúyŏng/Rui Shi list.
- **Miranda / Odalisques / Sforza:** **25–28pt Miranda Wildcard** has Mimetism(-6), Specialist Operative, Monofilament and counts as **Odalisque** in its family. **19–26pt Odalisques** offer NWI, Sixth Sense, combat-instinct tools, and 0-SWC Disco Baller/Paramedic/Viral Marksman profiles as Duo/Haris. **23/0 or 26/0 Sforza FTO Wildcard** brings NCO, Viral + adhesive, while **non-FTO option 1 (26/0)** is solo Holoprojector/FD/Surprise Attack. Useful tricks if their unique objectives beat an extra HI shooter; not mandatory filler. [W2/H1]
- **Ghulam LT, Sforza/NCO and Fireteams:** Ghulam LT **11/0** or **15/0 +1 Command Token** and Brawler LT **15/0** are current choices. **Ghulam smoke NCO 15/1** and **Sforza NCO** can exploit the LT Order. Unlike [W1/R1] N4 discussion, **the current Zúyŏng roster has NO Lieutenant loadout**. No standard Chain of Command; protect the LT and watch the 15-slot economy.
- **Al Fasid (44–50):** ARM5/BTS6, Warhorse, Sixth Sense, Minelayer and HMG+Smoke GL or HRL make a **self-sufficient solo/Assault Duo anchor**. **Counter:** its 1.5 SWC and inability to join Zúyŏng/Ghulam links can be an inefficient duplication of Maghariba or Zúyŏng HMG roles. [W2/H1]

### TAGs, REMs and Vehicle audit: exact N5.3 eligible units

| Unit | Why take it | Cautions / dissent |
|---|---|---|
| **Maghariba Guard (AVA1)** **72/1.5 E/M Carbine(+2B)**, **71/1.5 HRL+Grenade Launcher**, **71/1.5 HFT(+1B)+Shock Mine Dispenser**, all MULTI HMG | **BS14, ARM8, BTS6, STR3, S8, 360º, Baggage, TacAware, ECM Guided(-6)/Hacker(-3)**. [T1] N5 TAG panel especially favors **HFT + Mine Dispenser** for approach defense and Baggage reload; [N1] demonstrates Maghariba + Ghulam smoke/Valerya/Zhēnchá + cheap Libertos/Traktor support. Eligible **Assault Duo**. | [R1] says Dahshat's huge points discount elsewhere compensates for a TAG he sees as overpriced; [T1/H1] see 71pt as viable but warn **S8 and broad base expose it to shots and narrow routes**. Choose for suitable table terrain and sustained armor fighting, not automatically. |
| **Triphammer TAG (AVA1)** **48/0 HRL+shotgun+Panzerfaust**, **52/0 Thunderbolt+shotgun**, or **52–53/1.5 AP Spitfire** | ARM7/STR3, Tactical Awareness, Booty, transmutation and embedded **TurtleMek Specialist**. Cheaper zero-SWC TAG / eligible Assault Duo when SWC funds Rui Shi, snipers or guided. [T1/H1] | Contested: BS13/BTS3, large target and worse direct gun profile; not a premium TAG duelist. Often a real Maghariba or more specialist redundancy is preferable. |
| **Rui Shi REM (AVA1)** **23/1 MSV2 Spitfire**, **21/0.5 MSV1 Red Fury + Shock Mine Dispenser** | **Can join Zúyŏng Core/Haris**; MSV2 plus smoke and optional EVO Marksmanship becomes an inexpensive answer to Mimetism/ARO lanes, with linked shooting bonuses. [W1/R1/Y1] | Only STR1/ARM1, hackable, and needs repair/TinBot placement. Old videos quote different armor/points/Fireteam math: pinned profile above wins. |
| **Lù Duān REM (AVA1)** **24/0 Mk12+HFT+E/M Mine**, **20/0 Thunderbolt+E/M Carbine+E/M Mine** | Holoprojector, MSV1, Surprise(-3), BS Attack(+1B) provide deception, templates and anti-tech at **0 SWC**. [W2] likes it as the versatile Rui Shi alternative. | **Not linkable** here. **N4 Holomask/Minelayer/deployable-repeater tricks do not exist on its pinned N5 profile**. Rui Shi is better for linked direct shooting. |
| **Rafiq REM (AVA1)** **13/0 FO+Sensor**, **19/0.5 FTO Red Fury** | Fast Sensor/FO/Deactivator/Repeater can reveal markers and push objectives; **only profile 3 Red Fury** qualifies for the odd **Assault Duo** row. [W2] | BS11/ARM0/STR1. **13pt FO profile does not join Assault**. Sometimes Hunzakut FO or Zhēnchá gets to the objective safer. |
| **Shihab TR REM (AVA1)** **23/1 HMG**, **18/0 Thunderbolt(+1B)** | Total Reaction 360º deterrent. **18pt zero-SWC** fits lists already paying SWC for Maghariba/Rui Shi/Brawler sniper. Can use relevant EVO supportware. [W2/R1] | STR1/ARM0 and no Fireteam row; it delays, not withstands, serious attackers. |
| **Shaytaniyah REM (AVA1)** **16/1.5 Guided ML** or **19/1.5 ML(+1B), NOT Guided** | Guided profile threatens Targeted targets via Valerya/HD/FO repeaters; +1B variant is a **direct-attack** option. [W2] | Neither profile may link in Dahshat. **Do not merge Guided and +1B** into an illegal linked Guided missile. High SWC and setup Orders compete with 9pt Traktor artillery or direct attacks. |
| **Traktor Mul REM (AVA2)** **5/0 Baggage**, **9/1 Katyusha MRL Guided**, **14/1 Uragan MRL Guided+Total Reaction** | Very cheap Regular Baggage battery or Guided threat. [W2] favors 9pt/1SWC as an inexpensive artillery option; [N1] demonstrates a separate 5pt Baggage unit reloading near cover when Maghariba is forced elsewhere. | MRL damage/ranges **differ** from the Shaytaniyah missile launcher; still needs Targeted; no Fireteam row. Do not assume a free kill from a single Spotlight. |
| **Fanous REM (AVA3)** **7/0** | Cheap fast Regular Repeater/Flash Pulse with Mimetism(-3), spreads network and makes Irregular-heavy lists more order-stable. | Uses one of precious 15 slots; STR1, cannot link. |
| **Kameel REM (AVA2)** **8/0 Baggage+Repeater**, **14/0.5 EVO**, **16/0 Total Reaction combi** | Reload/network and EVO for a planned Rui Shi/Shihab REM package; alternative TR body. [W2/R1/H1] | EVO costs SWC and troop slot; optional, not auto-include. No Fireteam membership. |
| **Nasmat, Jandab, TurtleMek, Jackbot** | Servant/ancillary/synchronized helper reach for repair, objectives and attacks. | **Not separate Regular Orders**; obey parent profile and peripheral limitations. |

**Vehicle classification:** Dahshat's **39-unit Main roster has no VH-type troops**. Kum, motorized 112 and Motorized Bounty Hunters are **motorcycle WB/LI**, not VH. Maghariba and Triphammer are **TAGs**, not VH. Do **not** import Haqq-only Shakush or Scarface, other-faction Vehicles, or adjacent sectorial Fireteam rights. Jandab/TurtleMek/Jackbot are ancillary, not separate TAGs.

### Keep disagreement and legality visible

1. **Discount swarm vs expensive flagship:** [R1] calls Dahshat the discount army where **troop slots, not points**, are scarce, and considers Maghariba slightly overpriced; [N1/T1/H1] show Maghariba is still a very good heavy anchor because the other pieces leave enough points. Both are conditional on mission/terrain.
2. **Linked Rui Shi vs independent Maghariba:** [W1/R1] prefer efficient **MSV2 Spitfire + smoke/EVO**, while [T1] praises **Maghariba mine dispenser/defense**. Do not rank them as interchangeable: one wins negative-mod gunfights efficiently, one absorbs shots and controls wide lines.
3. **Traktor vs Shaytaniyah Guided:** [W2] values **9pt Katyusha/1 SWC**; full Guided ML **16/1.5** offers a different weapon at more cost. The Shaytaniyah **19/1.5 +1B profile is NOT Guided**. Neither gains any Dahshat link.
4. **Hacking strength:** [W1] sees strong enough network through Valerya/Ghulam and Repeaters, while [R1] points out **no native KHD and weak anti-hacker resilience**. **N5 Zhēnchá HD now includes Trinity upgrade**, a meaningful improvement, while remaining **not a KHD**.
5. **Roster-only rules, do not inherit prior Fireteams:** **Zúyŏng Core/Haris legally includes Rui Shi** (not Fanous/Rafiq/Maghariba); **Ghulam Core/Haris legally includes Fiddler option 1 only**; Brawlers can include Monstruckers and **Zellenkrieger FTO profile 3 only (no Smoke)**. **Húláng FTO/FTO-2 and foot 112 FTO have no Fireteam access**. The Assault Duo chart has peculiar **required=true/min=0 for every row**; do not invent a universal required anchor or unsupported combos. Check authoritative chart.
6. **Current Lieutenant reality:** Older [W1/R1] recommend a Zúyŏng Lieutenant HMG. That profile **does not exist** in the pinned roster. Ghulam/Brawler provide current LTs, while Ghulam NCO and Sforza use LT Orders. Do not copy an N4 list.

### Recommended videos/podcasts and MCP transcript coverage

**Dedicated Dahshat material — best first**
- **[N1] [Robert Shepherd — Infinity N5 Battle Report: Dashat vs PanOceania (Acquisition)](https://www.youtube.com/watch?v=cQCB9XONJvU)**. **YouTube MCP transcript reviewed**; practical current-edition play with Maghariba, Ghulam LT/NCO/Valerya Pitcher, Zhēnchá Trinity HD, 2 Libertos, Monstruckers, Traktor Baggage and Rui Shi. *A single game, not general win-rate proof.*
- **[W1] [WIP12 E165: Dashat Part 1](https://open.spotify.com/episode/5LyspedREmw1py5M8gLa1K)** (2024-07-23). **Podcast MCP transcript reviewed**; strongest detailed N4 faction philosophy: 15 slots vs cheap models, McMurrough/Libertos, Rui Shi/Zúyŏng, hacking and Ghulam support.
- **[W2] [WIP12 E166: Dashat Part 2](https://open.spotify.com/episode/4rONwGAmjRXakeybrBVeBA)** (2024-07-30). **Podcast MCP transcript reviewed**; best specialist, TAG, REM and Guided counterpoints, including Saito, Lù Duān, Rafiq, Traktor/ML, Shihab, Maghariba.
- **[R1] [Robert Shepherd — Infinity N4 Faction Focus: Dashat Company](https://www.youtube.com/watch?v=Aj9eai4crps)** (2024-09). **YouTube MCP transcript reviewed**; discount army, unit selection pressure, linked Rui Shi/EVO, Fiddler Jackbots and Maghariba. **Outdated N4 assertions about lack of Trinity and Zúyŏng LT are explicitly corrected above**.
- [Robert Shepherd — Dashat Company Faction Overview and Battle Reports](https://www.youtube.com/watch?v=BbyHVkAu-pk). **YouTube MCP transcript reviewed**; older general context, not authoritative for N5.
- **[WIP12 E82 Dahshat Part 1](https://open.spotify.com/episode/71CneWgRofMq5g0NRoZVFc)** and [E83 Part 2](https://open.spotify.com/episode/2dQjCY7e6i9S9eilwI00su) (2022). **Both Podcast MCP transcripts reviewed**; extra historical differences, not contemporary list legality.

**TAGs, combat/support REMs and neighboring Haqq/Yu Jing**
- **[T1] [Loss of Lieutenant E142 — N5 TAG Tier List](https://www.youtube.com/watch?v=dZo_gQWQYSY)** and [Spotify](https://open.spotify.com/episode/1h5CJfZC5zBPxdg66o7xIN). **YouTube MCP transcript reviewed**; discusses Maghariba's preferred HFT/mine dispenser and reloads, S8 footprint concern, Triphammer alternatives, and why Dahshat can afford a TAG more easily.
- **[H1] [Robert Shepherd — N5 Haqqislam Faction Focus](https://www.youtube.com/watch?v=Dmv4pfdTbc0)** (2025-11). **YouTube MCP transcript reviewed**; Maghariba/TAG footprint and updated Odalisque ideas. **Haqq-only Maghariba Duos, Hafza, Saladin and other TAGs are not Dahshat units**.
- **[Y1] [Robert Shepherd — N5 Yu Jing Faction Focus](https://www.youtube.com/watch?v=mn4yHSNxsnA)** (2025). **YouTube MCP transcript reviewed**; Tactical Awareness HI and EVO/combat-REM support. Do not import vanilla Yu Jing links.
- **[Infinity the Dante — N5 Qapu Khalqi Faction Focus](https://www.youtube.com/watch?v=z4kV-SFZ5Uw)**. **YouTube MCP transcript reviewed** for shared faction themes; QK Fireteam/TAG lineup differs.
- [Dahshat N5 source index, Bureau Aegis](https://www.bureau-aegis.org/forum/index.php?topic=18021.0); [N4 Dahshat discussion, Corvus Belli](https://forum.corvusbelli.com/threads/n4-recap-dahshat-company-tacticas.41552/). These catalog historical views and edition dates, not a substitute for the pinned Army source.

**Coverage limitation:** The MCP catalogue returned the excellent **2024 WIP12 shows**, but no **verified long-form late-2025/2026 N5 Dahshat-only faction review**. N5 conclusions here are based on the actual N5 battle transcript, cross-faction current sources and exact pinned Army data; transcribed unit names are often phonetically garbled.

## Provenance

Validated against the pinned N5.3 Army-derived source on **2026-10-16**. If future Army revisions change roster entries, AVA, profiles, Fireteam chart semantics, relation records, or Reinforcement linkage, update this file and its `army_source_version`/verification metadata together.

## Mission specialist choices — N5.3 cross-game evaluation

A balanced **Dahshat** mission list wants independent **Ghulam FO12/Doctor15** (where roster-legal), a midfield camouflaged/forward specialist, and a **real Engineer** to support its expensive tech when chosen. Don't mistake **Ghulam Lieutenant or NCO** role for generic button permission; a strong hired gun cannot score Specialist-only consoles by being a good combat profile. Protect one late Specialist while the aggressive package trades.

See [Mission Specialists / Button Pushers apex and value tiers](../../notes/list-building/mission-specialists-and-button-pushers-apex-value.md). This roster and its Fireteam chart are the final authority for exact options.

## N5.3 airborne / enemy-DZ profile and value choices (2026-10-23)

**Bashi Bazouk SMG12/0 or T2 BSG14/0** is a very cheap **Irregular ordinary Parachutist + Holoprojector** distraction; the current Dahshat list does **not** grant Bashi Combat Jump or Parachutist(DZ), unlike Druze's explicit Combat Jump profile. **Saito Tōgan33/0** has Hidden Deployment/Infiltration, excellent CC/EXP threat but does not deploy inside enemy DZ; **Hunzakuts/Zhencha** can threaten protected midfield lanes. With no standard Combat Jump profile, prefer reliably opened side routes over an imaginary sky drop. Preserve a scoring piece after the assault.

[Cross-game N5.3 airborne/rear-strike apex-value and landing-risk tiers](../../notes/list-building/airborne-and-enemy-dz-attackers-apex-value.md). **Use this roster and canonical Fireteam chart for exact legality.**

## TAG tactical cross-reference (2026-10-23)

**Maghariba Guard** buys a conventional heavy ARM8 ranged centerpiece but needs S8 lanes, screening and Engineer access; **Triphammer** is a cheaper, aggressive secondary weapon choice with TacAware and the required-assault partner opportunities. When Dahshat already has efficient HI and support guns, the cheaper TAG may give better scenario value than a second long-range elite.

For the two-tier **apex/points-value** comparison, TAG counterplay, matchup matrix and direct transcript sources: [N5.3 TAG field guide](../../notes/list-building/tags.md). Treat current profiles, points/SWC and canonical Fireteam data above as authoritative.

## Hacker and KHD tactical cross-reference (2026-10-23)

**Valerya Gromoz WIP14 HD + Pitcher/Total Control(+1B), 19/0.5**, is the clear value engine for hostile TAG/HI via projected Repeaters. **Brawler HD 16/0.5 (Sixth Sense)** and **Ghulam HD 16/0.5** are cheap general-coverage specialists; **Zhēnchá HD+Trinity 34/0.5** trades price for a hidden/camouflaged forward hacker assassin. **Important roster distinction:** the current **Dahshat standard Main roster lists no ordinary native KHD**. A Trinity-upgrade **HD** is *not* a KHD/Cybermask source unless specifically printed. **Why:** don't assume a hacker-heavy list automatically has lethal network defense; take suitable Camo/physical repeater-clearing or the hybrid profile and maintain TAG-support TinBots where actually legal.

See the [cross-game apex/value Hacker/KHD tier guide](../../notes/list-building/hackers-and-killer-hackers.md). **The sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative; device upgrades are profile-specific.**


## Cheerleader / Order-generation tactical cross-reference (2026-10-23)

See the N5.3 [cross-game apex/value rankings and transcript-backed competing assessments](../../notes/list-building/cheerleaders-and-order-generators.md). The current roster and official Fireteam definitions above remain authoritative; unit access/cost may differ from vanilla.

- Cheap Authorized/Motorized Bounty Hunter — usually a Regular trading body with Booty, not always a protected static S2 Order; exact bike/profile/Fireteam legality varies.
- 7pt Fanous — regular Flash/Repeater network Order when this mercenary/NA2 roster permits it.
- 8pt Kameel — Baggage/repeater utility where this NA2 roster permits it.
- 3pt Warcor — very useful Irregular Flash ARO/cheap screen, NOT an ordinary transferable Order.

**Selection rule:** Count deployed, transferable Regular Orders per Combat Group, not total models or restricted bonus Orders; choose the lowest-cost protected Regular profile that *also* contributes a relevant Repeater, Baggage, Fireteam, template, ARO or Specialist job. Check Group slots and DZ hiding space before buying a third large-base REM or replacing a needed scoring piece.


## ARO apex/value cross-reference (2026-10-23)

See [Best ARO Units in N5.3 — apex, cost-value, Hidden Deployment, reactive traps, opposed podcast views](../../notes/list-building/aro-units-apex-and-value.md). **Only the legal roster above** establishes options, exact costs/AVA, upgrades and Fireteam permissions in this army.

- **Authorized Bounty Hunter cheap body** — small-base template/Panzerfaust or close ARO if profile equipped, useful only in legal team/roster
- **Cateran camo T2/AP sniper** — 21pt Irregular long-range trade up, valuable despite not making generic pool Orders
- **Warcor 3pt Flash** — token defensive tax/late game stun, Irregular so not a generic Order

**List test:** a strong ARO consumes enemy Orders by forcing Smoke, rerouting, poor range, discoveries or risky trades. A robust list normally prefers *serial, different* defenders—a cheap visible or marker/template screen, a covered second gate, and a preserved attack/scoring unit—rather than two adjacent visible snipers. Plan for opponent pie-slicing, AD, anti-camo, hacking and recovery; evaluate whether extra SWC is better spent on mission attackers.
