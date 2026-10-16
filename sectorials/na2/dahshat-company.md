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

## Provenance

Validated against the pinned N5.3 Army-derived source on **2026-10-16**. If future Army revisions change roster entries, AVA, profiles, Fireteam chart semantics, relation records, or Reinforcement linkage, update this file and its `army_source_version`/verification metadata together.
