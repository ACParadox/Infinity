---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 502
sectorial_slug: corregidor
sectorial_name: Corregidor
parent_faction: Nomads
rules_baseline: N5.3
army_source_version: "7.26246.158"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-15
coverage: "Standard Corregidor roster, standard loadouts, canonical Surface/Deepspace/Correctional Fireteam chart, and reverse Fireteam index. Vortex Spec-Ops and Nomads Team-Ops are optional-mode hooks rather than ordinary matched-play roster entries."
---

# Corregidor

## Overview and provenance

**Unit selection evidence (23 Oct 2026):** [Nomads source-backed four-roster must-have / go-to / avoid audit](#must-have--go-to--avoid--source-backed-recommendations-2026). Tactical opinion only; the roster and Fireteam chart in this file remain authoritative.


Repository-native reference for **Corregidor** roster, profiles, points/SWC, AVA, dependencies, and Fireteam access.

For concise, transcript-reviewed strategy, list-building modules, opinion disagreements and TAG/REM analysis, see [Corregidor — N5.3 Tactical and List-Building Guide](../../notes/factions/corregidor.md). This file remains authoritative for current profile legality and Fireteam charts.

Sources used:

- Army-derived Corregidor source revision `7.26246.158` from `massayoshi/infinity-army-backup` commit `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b`.
- InfinityDB Fireteam normalization/semantics at commit `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: N5.3 + N5 FAQ v0.1.

Coverage notes:

- Covers the **40-unit standard Corregidor roster** and the complete Corregidor `fireteamChart` in the pinned Army source.
- `Vortex Spec-Ops` and `Nomads Team-Ops` are optional game-mode content and are listed separately.
- Soldier of Fortune / generic mercenary-catalog entries whose source faction list is empty are excluded from the base roster.
- Surface and Deepspace Fireteams are separate legal team families and are not merged in this reference.
- Fireteam legality comes from the canonical chart below, not from an `FTO` loadout name by itself.
- Profile restrictions are preserved: Coyote joins the Surface team only through its FTO profiles; Vostok and Jazz are Wildcards only through their FTO profiles. Stempler is a Wildcard without a chart-level FTO restriction even though one Stempler profile is named FTO.
- The structured `required: true` rows in the Corregidor Surface, Correctional, Corregidor Deepspace, and armored team families are preserved as required-choice sets; this file does not reinterpret them as requiring every marked unit type simultaneously.
- Coyote/BambaDroid list dependency is preserved: a BambaDroid requires a Coyote in the same Combat Group, and the list cannot contain more BambaDroids than Coyotes.
- The Army source uses `coyotes-recon-and-maneuver-team` for the BambaDroid row in one Surface Armored entry while the actual unit slug is `coyotes`; this reference normalizes both to the same Coyotes/BambaDroid source unit.
- Linked Reinforcement army ID: **599**. Reinforcement Fireteam rows are not merged into the main chart here.

## Sectorial summary

| Field | Value |
|---|---|
| Sectorial | Corregidor |
| Parent faction | Nomads |
| Army ID | 502 |
| Rules baseline | N5.3 + FAQ v0.1 |
| Standard roster units | 40 |
| Optional-mode units | Vortex Spec-Ops; Nomads Team-Ops |
| Reinforcement roster | Army ID `599` |
| Fireteam limits | Core 1; Haris 1; Duo unlimited |
| Fireteam structure | Surface, Correctional, Deepspace, plus Surface/Deepspace armored and Gecko families |

## Roster index

| Unit | ID | AVA | Type | Order | Fireteam access |
|---|---:|---:|---|---|---|
| Valerya Gromoz | 464 | 1 | LI | Regular | Surface Wildcard; Deepspace Wildcard |
| Warcors | 50 | 1 | LI | Irregular | — |
| Diablos of D-Block | 1578 | 4 | HI | Irregular + Impetuous | Correctional |
| Gecko Squadron | 432 | 4 | TAG | Regular + Tactical Awareness | Gecko Surface; Gecko Deepspace; Deepspace Armored |
| Hellcats | 394 | 5 | MI | Regular | — |
| Corregidor Alguaciles | 296 | Total | LI | Regular | Corregidor Surface; Corregidor Deepspace |
| Tomcats | 415 | 4 | LI | Regular | — |
| Evaders | 1543 | 3 | HI | Regular | Corregidor Deepspace; Gecko Deepspace |
| Vigilantes | 1895 | 2 | MI | Regular | — |
| Jazz & Billie | 1551 | 1 | LI + REM | Regular | Surface/Deepspace Wildcard, Jazz FTO only |
| Reaktion Zonds | 409 | 1 | REM | Regular | — |
| Salyut Zonds | 426 | 2 | REM | Regular | — |
| Señor Massacre | 462 | 1 | MI | Regular | Surface Wildcard; Deepspace Wildcard |
| Intruders | 395 | 5 | MI | Regular | — |
| Meteor Zonds | 411 | 1 | REM | Regular | — |
| Bearcats | 1891 | 3 | HI | Regular | — |
| Kazurabā Ruby Monday | 1890 | 1 | HI | Irregular | — |
| Moran, Maasai Hunter | 421 | 2 | SK | Regular | — |
| Clockmakers | 406 | 1 | LI | Regular | — |
| Zondbots | 425 | 2 | REM | Peripheral | — |
| Lobos | 1579 | 4 | MI | Regular | Correctional; Corregidor Deepspace |
| Corregidor Bandits | 400 | 2 | SK | Irregular | — |
| Corregidor Jaguars | 404 | 5 | WB | Regular | Correctional |
| Coyotes / BambaDroids | 1896 | 3 / 3 | MI / REM | Regular | Corregidor Surface, Coyote FTO only; BambaDroid also Surface Armored |
| Daktaris | 405 | 2 | LI | Regular | Surface Wildcard; Deepspace Wildcard |
| Vertigo Zonds | 410 | 1 | REM | Regular | — |
| Transductor Zonds | 412 | 2 | REM | Regular | — |
| TAG-Treiber | 1853 | 1 | LI | Regular | Corregidor Deepspace |
| Wildcats | 430 | 5 | MI | Regular | Corregidor Surface; Gecko Surface; Surface Armored; Corregidor Deepspace; Deepspace Armored |
| Mobile Brigada | 382 | 6 | HI | Regular | Corregidor Surface; Corregidor Deepspace |
| Sombras | 1542 | 2 | MI | Regular | — |
| Shifta Insertion Group | 1902 | 2 | LI | Regular | Surface Wildcard only |
| Territorials | 1893 | 3 | MI | Regular + Tactical Awareness | Corregidor Surface |
| McMurrough | 283 | 1 | WB | Irregular + Impetuous | — |
| Stempler Zonds | 408 | 1 | REM | Regular | Surface Wildcard; Deepspace Wildcard |
| Vostok Sputniks | 1544 | 2 | REM | Regular | Surface/Deepspace Wildcard, FTO profiles only |
| Lupe Balboa | 433 | 1 | LI | Regular | Surface Wildcard; Deepspace Wildcard |
| Gator Squadron | 1580 | 2 | TAG | Regular + Tactical Awareness | Deepspace Armored |
| Carlota Kowalsky | 427 | 1 | LI | Regular | — |
| Iguana Squadron | 383 | 2 | TAG | Regular + Tactical Awareness | Surface Armored |

Optional-mode units:

| Unit | ID | Mode | Fireteam relevance |
|---|---:|---|---|
| Vortex Spec-Ops | 1917 | Spec-Ops | Corregidor Surface and Corregidor Deepspace, max 1 when Spec-Ops mode is in use |
| Nomads Team-Ops | 1931 | Team-Ops | No ordinary Corregidor Fireteam row |

## Unit details

### Valerya Gromoz, Mercenary Hacker

**ID 464 · AVA 1 · LI** — `MOV 10-10 | CC 15 | BS 11 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`. Hacking Device with Total Control (+1B) upgrade; Hacker.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 19 | 0.5 | Combi Rifle, Zapper, Pitcher, Pistol, CCW | Surface Wildcard max 1; Deepspace Wildcard max 1 |

### Warcors, War Correspondents

**ID 50 · AVA 1 · LI** — `MOV 10-10 | CC 11 | BS 9 | PH 11 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Journalist; Irregular.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CCW (-3); 360º Visor | — |
| 2 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CCW (-3); Sixth Sense | — |

### The Diablos of D-Block

**ID 1578 · AVA 4 · HI** — full-power profile `MOV 15-5 | CC 23 | BS 11 | PH 13 | WIP 12 | ARM 2 | BTS 0 | W 2 | S 2`; Battle-Ravaged profile `MOV 10-10 | CC 23 | BS 10 | PH 12 | WIP 12 | ARM 2 | BTS 0 | W 2 | S 2`. Berserk, Natural Born Warrior, Transmutation, Religious Troop, No Cover; Irregular + Impetuous.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 8 | 0 | Light Shotgun, Grenades, Boarding Pistol, Trench-Hammer, CCW | Correctional required-choice max 4 |
| 2 | 9 | 0 | SMG, Grenades, Boarding Pistol, Trench-Hammer, CCW | same |
| 4 | 9 | 0 | SMG, Flammenspeer, Boarding Pistol, Trench-Hammer, CCW | same |

### Gecko Squadron

**ID 432 · AVA 4 · TAG** — `MOV 15-5 | CC 15 | BS 13 | PH 14 | WIP 13 | ARM 6 | BTS 6 | W 3 | S 6`. ECM: Guided, ECM: Hacker, Tactical Awareness, Zero-G Terrain. Each profile includes a RobbyBot attendant.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 54 | 1 | MULTI Marksman Rifle, Chain Rifle, Panzerfaust, CCW | Gecko Surface 1–3; Gecko Deepspace 1–3; Deepspace Armored max 1 |
| 2 | 55 | 1 | Mk12, Chain Rifle, Blitzen, CCW | same |
| 3 | 49 | 0 | Vulkan Shotgun, Chain Rifle, Panzerfaust, CCW | same |

### Hellcats

**ID 394 · AVA 5 · MI** — `MOV 10-10 | CC 14 | BS 12 | PH 12 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. Courage, Parachutist, Combat Jump, Super-Jump, Terrain (Zero-G).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 3 | 19 | 0 | Boarding Shotgun, Adhesive Launcher Rifle, D-Charges, Pistol, CCW | — |
| 5 | 26 | 1.5 | Spitfire, Pistol, CCW | — |
| 6 | 22 | 0.5 | Boarding Shotgun, D-Charges, Pistol, CCW; Hacking Device, Hacker | — |
| 8 | 23 | 0 | Combi Rifle, Pistol, CCW; MediKit, Paramedic | — |

### Corregidor Alguaciles

**ID 296 · AVA Total · LI** — `MOV 10-10 | CC 14 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 10 | 0 | Combi Rifle, Pistol, CCW | Surface required-choice max 5; Deepspace required-choice max 5 |
| 2 | 18 | 1 | HMG, Pistol, CCW | same |
| 5 | 15 | 1.5 | Missile Launcher, Pistol, CCW | same |
| 6 | 15 | 0.5 | Combi Rifle, Pistol, CCW; Hacking Device, Hacker | same |
| 8 | 12 | 0 | Combi Rifle, Flash Pulse, Pistol, CCW; Deployable Repeater, Forward Observer | same |
| 9 | 12 | 0 | Combi Rifle, Pistol, CCW; MediKit, Paramedic | same |
| 10 | 10 | 0 | Combi Rifle, Pistol, CCW; Lieutenant | same |
| 11 | 12 | 0 | Combi Rifle, Pistol, CCW; Commlink (+1), Specialist Operative | same |
| 12 | 10 | 0 | **ALGUACIL GATTA**; SMG, Contender, Pistol, CCW; BTS 3 | same |
| 13 | 10 | 0 | **ALGUACIL GATTA**; SMG, E/Mitter, Pistol, CCW; BTS 3 | same |
| 14 | 10 | 0 | **ALGUACIL GATTA**; SMG, Adhesive Launcher Rifle, PARA Mine, Pistol, CCW; BTS 3 | same |

### Tomcats, Emergency and Rescue Special Team

**ID 415 · AVA 4 · LI** — `MOV 10-10 | CC 14 | BS 12 | PH 11 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Parachutist, Climbing Plus, Terrain (Zero-G), Deactivator.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 3 | 19 | 0.5 | Combi Rifle, Light Flamethrower, Pistol, CCW; Deployable Repeater | — |
| 4 | 22 | 0 | Combi Rifle, Light Flamethrower, D-Charges, Pistol, CCW; GizmoKit, Engineer | — |
| 5 | 25 | 0 | MULTI Rifle, Light Shotgun, D-Charges, Pistol, CCW; GizmoKit, Engineer | — |
| 6 | 26 | 0 | As Opt 4; includes Zondcat | — |
| 7 | 22 | 0 | Combi Rifle, Light Flamethrower, Pistol, CCW; MediKit, Doctor | — |
| 8 | 26 | 0 | As Opt 7; includes Zondcat | — |
| 9 | 17 | 0 | SMG, Panzerfaust, D-Charges, Pistol, CCW; MediKit, Paramedic | — |

### Evaders, EVA Tactical Group

**ID 1543 · AVA 3 · HI** — `MOV 10-10 | CC 15 | BS 13 | PH 12 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`. Courage, No Wound Incapacitation, Climbing Plus, Terrain (Zero-G), Deactivator.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 31 | 1 | AP Spitfire, D-Charges, Pistol, CCW; TinBot: Firewall (-3), Specialist Operative | Deepspace required-choice max 3; Gecko Deepspace max 1 |
| 4 | 23 | 0 | Boarding Shotgun (+1SD), D-Charges, AP Mine, Pistol, CCW; TinBot: Firewall (-3), Specialist Operative | same |
| 5 | 32 | 1.5 | Feuerbach, D-Charges, Pistol, CCW; TinBot: Firewall (-3), Specialist Operative | same |
| 6 | 29 | 0 | MULTI Rifle, Panzerfaust, D-Charges, Pistol, CCW; GizmoKit, Engineer | same |
| 7 | 24 | 0 | Boarding Shotgun, D-Charges, AP Mine, Pistol, CCW; GizmoKit, Engineer | same |
| 8 | 35 | 1.5 | AP Spitfire, D-Charges, Pistol, CCW; GizmoKit, TinBot: Firewall (-3), Engineer | same |

### Vigilantes, Tactical Support and Surveillance Special Group

**ID 1895 · AVA 2 · MI** — `MOV 10-10 | CC 16 | BS 12 | PH 11 | WIP 13 | ARM 3 | BTS 6 | W 1 | S 2`. Camouflage, Mimetism (-3), Surprise Attack (-3), Forward Deployment (+20), Counterintelligence, Stealth, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 25 | 0.5 | AP SMG, Flash Pulse, Cybermine, Pistol, CCW; Hacking Device, Hacker, Sensor | — |
| 2 | 28 | 0 | MULTI Rifle, Light Flamethrower, Pistol, CCW; Killer Hacking Device, Hacker | — |
| 3 | 28 | 0.5 | MULTI Rifle, Light Flamethrower, D-Charges, AP Mine, Pistol, CCW; Minelayer, Specialist Operative | — |
| 4 | 29 | 0 | MULTI Rifle, Light Flamethrower, D-Charges, Armed Turret (Combi Rifle), Pistol, CCW; Specialist Operative | — |
| 5 | 26 | 0 | Boarding Shotgun (+1B), E/Mitter, Flash Pulse, D-Charges, Pistol, CCW; Forward Observer | — |

### Jazz & Billie, Tactical Hacking Team

**Jazz** — `MOV 10-10 | CC 16 | BS 11 | PH 10 | WIP 14 | ARM 0 | BTS 6 | W 1 | S 2`; Hacking Device Plus with Trinity (SR-1), Hacker. **Billie** — `MOV 15-10 | CC 13 | BS 10 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 1`; Repeater, Remote Presence.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 25 | 0.5 | **JAZZ Hacker & BILLIE**, 2 minis / 2 Regular Orders. Jazz: SMG, Pitcher, Cybermine, Boarding Pistol, PARA CCW (-3). Billie: Flash Pulse, E/M Mine, Heavy Pistol, PARA CCW (-3) | — |
| 2 | 22 | 0.5 | **JAZZ FTO** only: Combi Rifle, Pitcher, Cybermine, Boarding Pistol, PARA CCW (-3); Number 2 | Surface Wildcard max 1; Deepspace Wildcard max 1 |

### Reaktion Zonds

**ID 409 · AVA 1 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. 360º Visor, Remote Presence, Courage, Total Reaction, Climbing Plus.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 24 | 1 | HMG, PARA CCW (-3) | — |
| 2 | 19 | 0 | Thunderbolt (+1B), PARA CCW (-3) | — |

### Salyut Zonds

**ID 426 · AVA 2 · REM** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 4`. Baggage, Remote Presence, Courage.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 8 | 0 | PARA CCW (-3); Deactivator, Repeater | — |
| 2 | 14 | 0.5 | PARA CCW (-3); EVO Hacking Device, Hacker | — |
| 3 | 17 | 0 | Combi Rifle, PARA CCW (-3); Repeater, Total Reaction | — |

### Señor Massacre

**ID 462 · AVA 1 · MI** — `MOV 10-10 | CC 24 | BS 12 | PH 13 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. Martial Arts L3, Natural Born Warrior, Courage, Stealth.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 27 | 0 | Breaker Combi Rifle, Eclipse Grenades, E/M Grenades, Boarding Pistol, Shock CCW, E/M CCW | Surface Wildcard max 1; Deepspace Wildcard max 1 |
| 2 | 25 | 0 | Boarding Shotgun (+1B), Eclipse Grenades, E/M Grenades, Boarding Pistol, Shock CCW, E/M CCW | same |

### Intruders, Corregidor Assault Commandos

**ID 395 · AVA 5 · MI** — `MOV 10-10 | CC 14 | BS 13 | PH 12 | WIP 14 | ARM 3 | BTS 3 | W 1 | S 2`. MSV2, Camouflage, Mimetism (-3), Surprise Attack (-3), Stealth, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 38 | 1.5 | HMG, Heavy Pistol, CCW | — |
| 4 | 33 | 0 | AP SMG (+1B), Pulzar (+1B), Grenades, D-Charges, Heavy Pistol, CCW; Killer Hacking Device, Hacker, Infiltration | — |
| 6 | 38 | 1.5 | MULTI Sniper Rifle (+1SD), Heavy Pistol, CCW | — |

### Meteor Zonds

**ID 411 · AVA 1 · REM** — `MOV 15-10 | CC 14 | BS 11 | PH 12 | WIP 13 | ARM 0 | BTS 6 | W 1 | S 3`. ECM: Hacker, Repeater, Remote Presence, Triangulated Fire, Forward Observer, Parachutist, Combat Jump, Sensor, Super-Jump.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 21 | 0 | Light Shotgun, E/M Carbine, Flash Pulse, PARA CCW (-6) | — |
| 2 | 19 | 0 | Boarding Shotgun, Flash Pulse, PARA CCW (-6) | — |

### Bearcats, Airborne Heavy Regiment

**ID 1891 · AVA 3 · HI** — `MOV 15-5 | CC 15 | BS 13 | PH 13 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`. Parachutist, Combat Jump, No Wound Incapacitation, Super-Jump, Warhorse.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 30 | 0 | Boarding Shotgun (+1B), D-Charges, Boarding Pistol (+1B), CCW; Killer Hacking Device with Firewall (-3) upgrade, Hacker | — |
| 2 | 29 | 0 | AP SMG, Adhesive Launcher Rifle, D-Charges, Boarding Pistol (+1B), CCW; Killer Hacking Device with Firewall (-3) upgrade, Hacker | — |
| 3 | 28 | 0 | AP SMG, D-Charges, Boarding Pistol (+1B), CCW; Deactivator, GizmoKit, Engineer | — |
| 4 | 35 | 1.5 | Spitfire, D-Charges, Boarding Pistol (+1B), CCW; Specialist Operative | — |
| 5 | 27 | 0 | AP SMG, Boarding Pistol (+1B), CCW; MediKit, Deployable Repeater, Paramedic | — |

### Kazurabā Ruby Monday

**ID 1890 · AVA 1 · HI** — `MOV 15-5 | CC 18 | BS 12 | PH 12 | WIP 13 | ARM 3 | BTS 6 | W 2 | S 2`. Technorganic, Climbing Plus, Specialist Operative, Terrain (Total); Irregular.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 19 | 0 | Adhesive Launcher Rifle, Flash Pulse, E/M Grenades, Stun Pistol, CCW | — |

### Moran, Maasai Hunter

**ID 421 · AVA 2 · SK** — `MOV 10-10 | CC 15 | BS 12 | PH 11 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Infiltration, Mimetism (-3), Minelayer, Forward Observer, Stealth, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 18 | 0.5 | Combi Rifle, Flash Pulse, D-Charges, CrazyKoala, Pistol, CCW; Camouflage (1 Use), Surprise Attack (-3) | — |
| 2 | 16 | 0.5 | Boarding Shotgun, Flash Pulse, CrazyKoala, Pistol, CCW; Camouflage (1 Use), Surprise Attack (-3) | — |
| 3 | 17 | 0.5 | Combi Rifle, Flash Pulse, D-Charges, CrazyKoala, Pistol, CCW; Repeater | — |
| 4 | 15 | 0.5 | Boarding Shotgun, Flash Pulse, CrazyKoala, Pistol, CCW; Repeater | — |

### Clockmakers

**ID 406 · AVA 1 · LI** — `MOV 10-10 | CC 14 | BS 11 | PH 10 | WIP 15 | ARM 1 | BTS 3 | W 1 | S 2`. Engineer, Deactivator, GizmoKit.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 18 | 0 | Combi Rifle, D-Charges, Pistol, CCW | — |
| 2 | 19 | 0 | Same; Deployable Cover | — |
| 3 | 21 | 0 | Combi Rifle, D-Charges, Armed Turret (Combi Rifle), Pistol, CCW | — |

### Zondbots

**ID 425 · AVA 2 · REM** — `MOV 15-10 | CC 11 | BS 8 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 1`. Peripheral (Servant), Courage, Mimetism (-3).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 3 | 0 | PARA CCW (-3); no Order contribution | — |

### Lobos, Correctional Response Group

**ID 1579 · AVA 4 · MI** — `MOV 10-10 | CC 19 | BS 13 | PH 11 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`. Biometric Visor, Deactivator, Berserk, Natural Born Warrior, Warhorse, Religious Troop, FT Master (Diablos).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 20 | 0 | Boarding Shotgun (+1B), Disco Baller, Breaker Pistol, PARA CCW (-9) | Correctional required-choice max 4; Deepspace max 4 |
| 2 | 22 | 0 | Boarding Shotgun (+1B), Adhesive Launcher Rifle, Disco Baller, Breaker Pistol, PARA CCW (-9) | same |
| 3 | 22 | 0 | Breaker Combi Rifle, Heavy Riotstopper, Disco Baller, Breaker Pistol, PARA CCW (-9); Specialist Operative | same |
| 4 | 24 | 0 | Breaker Combi Rifle, Light Flamethrower, Disco Baller, Breaker Pistol, PARA CCW (-9); Specialist Operative | same |
| 5 | 28 | 1 | Red Fury, Disco Baller, Breaker Pistol, PARA CCW (-9); NCO | same |

### Corregidor Bandits

**ID 400 · AVA 2 · SK** — `MOV 10-10 | CC 22 | BS 12 | PH 13 | WIP 12 | ARM 1 | BTS 3 | W 1 | S 2`. Martial Arts L2, Camouflage, Mimetism (-3), Surprise Attack (-3), Infiltration, Stealth, Terrain (Total), Bangbomb (+4); Irregular.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 3 | 23 | 0 | Light Shotgun, Adhesive Launcher Rifle, Boarding Pistol, DA CCW | — |
| 5 | 28 | 0.5 | Light Shotgun, Adhesive Launcher Rifle, D-Charges, Boarding Pistol, DA CCW; Hacking Device, Hacker | — |
| 6 | 26 | 0 | Light Shotgun, Adhesive Launcher Rifle, D-Charges, Boarding Pistol, DA CCW; Killer Hacking Device, Hacker | — |
| 7 | 25 | 0.5 | SMG, Shock Mine, Boarding Pistol, DA CCW; Deployable Repeater, Minelayer | — |
| 8 | 24 | 0 | Light Shotgun, Adhesive Launcher Rifle, Flash Pulse, Boarding Pistol, DA CCW; Forward Observer | — |

### Corregidor Jaguars

**ID 404 · AVA 5 · WB** — `MOV 10-10 | CC 22 | BS 11 | PH 13 | WIP 12 | ARM 1 | BTS 0 | W 1 | S 2`. Martial Arts L1, Courage, Dogged, Frenzy.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 10 | 0 | Chain Rifle, Smoke Grenades, Kobra Pistol, DA CCW | Correctional required-choice max 4 |
| 2 | 11 | 0 | Light Shotgun, Smoke Grenades, Kobra Pistol, E/M CCW | same |
| 3 | 11 | 0 | Adhesive Launcher Rifle, Panzerfaust, Smoke Grenades, Kobra Pistol, DA CCW | same |

### Coyotes, Recon and Maneuver Team

**ID 1896 · Coyote AVA 3 · MI** — `MOV 10-10 | CC 15 | BS 13 | PH 11 | WIP 13 | ARM 2 | BTS 6 | W 1 | S 2`. MSV1, X-Visor, Forward Observer, Terrain (Total), Warhorse.

A BambaDroid can only be fielded if a Coyote is in the list; both must be in the same Combat Group, and BambaDroids cannot outnumber Coyotes.

#### Coyote loadouts

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 27 | 0 | Boarding Shotgun, Flash Pulse, D-Charges, Boarding Pistol, CCW; Forward Deployment (+10); BambaBot-1 | — |
| 2 | 27 | 0 | Same; BambaBot-2 | — |
| 3 | 33 | 0 | MULTI Marksman Rifle, D-Charges, Boarding Pistol, CCW; Forward Deployment (+10); BambaBot-1 | — |
| 4 | 33 | 0 | Same; BambaBot-2 | — |
| 5 | 28 | 0 | SMG, Flash Pulse, Boarding Pistol, CCW; Killer Hacking Device with Carbonite upgrade, Hacker, Forward Deployment (+10); BambaBot-1 | — |
| 6 | 28 | 0 | Same; BambaBot-2 | — |
| 7 | 19 | 0 | **COYOTE FTO**; Boarding Shotgun, Flash Pulse, D-Charges, Boarding Pistol, CCW | Surface required-choice max 2 |
| 8 | 26 | 0 | **COYOTE FTO**; MULTI Marksman Rifle, D-Charges, Boarding Pistol, CCW | same |
| 9 | 23 | 0 | **COYOTE FTO**; SMG, E/Mitter, D-Charges, Boarding Pistol, CCW; Killer Hacking Device with Carbonite upgrade, Hacker | same |

#### BambaDroid loadouts

**AVA 3 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 12 | ARM 0 | BTS 3 | W 1 | S 2`. ECM: Hacker, 360º Visor, Remote Presence, Mimetism (-3), Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 16 | 0 | AP Marksman Rifle, Chain Rifle, Mine Dispenser (AP), Pistol, PARA CCW (-3) | Surface max 2; Surface Armored max 1 |
| 2 | 13 | 0 | Thunderbolt, Chain Rifle, Mine Dispenser (AP), Pistol, PARA CCW (-3) | same |
| 3 | 13 | 0 | Thunderbolt, Chain Rifle, Flash Pulse, D-Charges, Pistol, PARA CCW (-3); Deployable Repeater, Forward Observer | same |

BambaBot-1 and BambaBot-2 are Coyote-attached Peripheral profiles rather than independent roster entries.

### Daktaris

**ID 405 · AVA 2 · LI** — `MOV 10-10 | CC 14 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Doctor, MediKit.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 14 | 0 | Combi Rifle, Pistol, CCW | Surface Wildcard max 1; Deepspace Wildcard max 2 |

### Vertigo Zonds

**ID 410 · AVA 1 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Remote Presence, Courage, Guided.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 16 | 1.5 | Missile Launcher, PARA CCW (-3) | — |

### Transductor Zonds

**ID 412 · AVA 2 · REM** — `MOV 15-15 | CC 13 | BS 8 | PH 11 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Repeater, Remote Presence, Courage, Mimetism (-3).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 7 | 0 | Flash Pulse, PARA CCW (-3) | — |

### TAG-Treiber, NMF TAG Squadrons Support Pilots

**ID 1853 · AVA 1 · LI** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Specialist Operative, TAGCom.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 12 | 0 | **GECKO PILOT**; Combi Rifle, Assault Pistol (+1B), CCW; GizmoKit, Terrain (Zero-G) | Deepspace max 1 |
| 4 | 11 | 0 | **GATOR PILOT**; Boarding Shotgun, D-Charges, Kobra Pistol, PARA CCW (-6) | same |

### Wildcats, Polyvalent Tactical Unit

**ID 430 · AVA 5 · MI** — `MOV 10-10 | CC 16 | BS 13 | PH 11 | WIP 13 | ARM 2 | BTS 6 | W 1 | S 2`. MSV1, Courage, Number 2, Combat Instinct, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 21 | 0 | Combi Rifle, Light Flamethrower, D-Charges, Pistol, CCW | Surface required-choice max 5; Gecko Surface max 1; Surface Armored max 1; Deepspace required-choice max 5; Deepspace Armored max 1 |
| 3 | 21 | 1.5 | Heavy Rocket Launcher, Light Shotgun, Pistol, CCW | same |
| 4 | 27 | 0.5 | Combi Rifle, Light Flamethrower, D-Charges, Pistol, CCW; Hacking Device with Zero Pain upgrade, Deployable Repeater, Hacker | same |
| 5 | 26 | 0 | Combi Rifle, Light Flamethrower, Jammer, D-Charges, Pistol, CCW; Killer Hacking Device, Hacker | same |
| 6 | 25 | 0 | Combi Rifle, Light Flamethrower, D-Charges, Pistol, CCW; Deactivator, GizmoKit, Engineer | same |
| 7 | 28 | 1.5 | Spitfire, Pistol, CCW; NCO | same |
| 8 | 25 | 0 | Combi Rifle, Light Flamethrower, D-Charges, Pistol, CCW; Lieutenant (+1 Order) | same |
| 10 | 22 | 0 | Boarding Shotgun, Flammenspeer, D-Charges, Pistol, CCW; Deactivator, GizmoKit, Engineer | same |

### Mobile Brigada

**ID 382 · AVA 6 · HI** — `MOV 15-5 | CC 18 | BS 13 | PH 13 | WIP 13 | ARM 5 | BTS 3 | W 2 | S 2`. 360º Visor, Courage, Jump (+7.5).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 33 | 0 | MULTI Rifle, Boarding Pistol (+1B), CCW; TinBot: Firewall (-6) | Surface required-choice max 5; Deepspace required-choice max 5 |
| 2 | 38 | 1.5 | HMG, Boarding Pistol (+1B), CCW | same |
| 3 | 27 | 0 | Boarding Shotgun, Boarding Pistol (+1B), CCW | same |
| 5 | 35 | 1.5 | Missile Launcher, Boarding Pistol (+1B), CCW | same |
| 9 | 36 | 0.5 | Combi Rifle, D-Charges, Boarding Pistol (+1B), CCW; Hacking Device, TinBot: Firewall (-6), Hacker | same |
| 10 | 33 | 0 | MULTI Rifle, Boarding Pistol (+1B), CCW; TinBot: Firewall (-6), Lieutenant | same |
| 11 | 27 | 0 | Boarding Shotgun, Boarding Pistol (+1B), CCW; Lieutenant | same |
| 12 | 38 | 1 | HMG, Boarding Pistol (+1B), CCW; Lieutenant | same |

### Sombras, Forward Interdiction Team

**ID 1542 · AVA 2 · MI** — `MOV 10-10 | CC 15 | BS 12 | PH 11 | WIP 13 | ARM 3 | BTS 6 | W 1 | S 2`. Camouflage, Mimetism (-3), Surprise Attack (-3), Forward Deployment (+20), No Wound Incapacitation, Stealth, Climbing Plus, Terrain (Zero-G).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 36 | 1 | Red Fury, Boarding Pistol, CCW | — |
| 2 | 40 | 0.5 | MULTI Rifle, Light Shotgun, Boarding Pistol, CCW; Hacking Device with Carbonite upgrade, Hacker | — |
| 3 | 33 | 0 | AP SMG, D-Charges, AP Mine, Boarding Pistol, CCW; Killer Hacking Device, Hacker | — |
| 4 | 36 | 0 | MULTI Rifle, Light Shotgun, D-Charges, Boarding Pistol, CCW; Specialist Operative | — |
| 5 | 29 | 0 | AP SMG, Flash Pulse, D-Charges, AP Mine, Boarding Pistol, CCW; Forward Observer | — |

### Shifta Insertion Group

**ID 1902 · AVA 2 · LI** — `MOV 10-10 | CC 16 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Triangulated Fire, Strategic Deployment, Specialist Operative, Stealth, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 21 | 0 | Light Shotgun (+1B), E/Marat, Flash Pulse, Disco Baller, Breaker Pistol, CCW; Chain of Command | Surface Wildcard max 2 |
| 3 | 17 | 0 | SMG, E/Marat, Flash Pulse, E/M Mine, Breaker Pistol, CCW; Minelayer | same |
| 4 | 22 | 0 | Thunderbolt (+1B), E/M Mine, Breaker Pistol, CCW; Minelayer | same |
| 5 | 21 | 0 | Thunderbolt (+1B), Breaker Pistol, CCW; MediKit, Paramedic | same |

### Territorials, Territorial Domination Unit

**ID 1893 · AVA 3 · MI** — `MOV 10-10 | CC 14 | BS 13 | PH 11 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`. Combat Instinct, Marksmanship, Terrain (Total), Tactical Awareness. All profiles provide Regular + Tactical Awareness Orders.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 28 | 0 | AP SMG, E/Mitter, Panzerfaust, D-Charges, AP Heavy Pistol, CCW; Deactivator, GizmoKit, Engineer | Surface required-choice max 3 |
| 2 | 26 | 0 | Boarding Shotgun (+1B), Panzerfaust, D-Charges, AP Heavy Pistol, CCW; GizmoKit, Specialist Operative | same |
| 3 | 32 | 1.5 | AP Red Fury, D-Charges, AP Heavy Pistol, CCW; Specialist Operative | same |
| 4 | 29 | 0 | AP Marksman Rifle, AP Heavy Pistol, CCW; X-Visor | same |
| 5 | 32 | 1.5 | AP Red Fury, D-Charges, AP Heavy Pistol, CCW; Lieutenant, Specialist Operative | same |
| 6 | 28 | 0 | As Opt 1; Lieutenant, Engineer | same |

### McMurrough, Mercenary Dog-Warrior

**ID 283 · AVA 1 · WB** — `MOV 15-10 | CC 23 | BS 11 | PH 16 | WIP 14 | ARM 4 | BTS 3 | W 2 | S 6`. Martial Arts L2, Berserk, Courage, Dodge (+5), Immunity (ARM), No Cover, Super-Jump, Dogged; Irregular + Impetuous.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 0 | Chain Rifle (+1B), Grenades, Smoke Grenades, AP + DA CCW | — |

### Stempler Zonds

**ID 408 · AVA 1 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Deactivator, Repeater, Remote Presence, Triangulated Fire, Courage, Forward Observer, Sensor, Climbing Plus.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 15 | 0 | Combi Rifle, Flash Pulse, PARA CCW (-3) | Surface Wildcard max 1; Deepspace Wildcard max 1 |
| 2 | 18 | 0 | Same; Tactical Awareness | same |
| 3 | 17 | 0 | **STEMPLER ZOND FTO**; same weapons; Super-Jump | same; chart itself does not restrict wildcard access to FTO |
| 4 | 22 | 0 | Thunderbolt (+1B), Flash Pulse, PARA CCW (-3); BS 12, Tactical Awareness | same |

### Vostok Sputniks

**ID 1544 · AVA 2 · REM** — `MOV 15-10 | CC 14 | BS 12 | PH 10 | WIP 13 | ARM 3 | BTS 6 | W 2 | S 4`. Remote Presence, Courage, Mimetism (-6), Climbing Plus, Immunity (AP).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 4 | 38 | 0 | Mk12, Light Shotgun, PARA CCW (-3); Repeater | — |
| 5 | 35 | 0 | **VOSTOK FTO**; Mk12, Light Shotgun, PARA CCW (-3) | Surface Wildcard max 1; Deepspace Wildcard max 1 |
| 6 | 37 | 1 | Spitfire, PARA CCW (-3); Repeater | — |
| 7 | 34 | 1 | **VOSTOK FTO**; Spitfire, PARA CCW (-3) | Surface Wildcard max 1; Deepspace Wildcard max 1 |

### Alguacil Vortex Lupe Balboa

**ID 433 · AVA 1 · LI** — `MOV 10-10 | CC 14 | BS 12 | PH 11 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. Mimetism (-3), Immunity (Shock).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 0 | AP SMG, E/Mitter, Panzerfaust, Smoke Grenades, Boarding Pistol, CCW; Chain of Command | Surface Wildcard max 1; Deepspace Wildcard max 1 |
| 2 | 19 | 0 | Same weapons; Specialist Operative | same |

### Gator Squadron

**ID 1580 · AVA 2 · TAG** — `MOV 15-10 | CC 21 | BS 14 | PH 15 | WIP 13 | ARM 8 | BTS 6 | W 3 | S 7`. ECM: Guided, ECM: Hacker, Tactical Awareness, NCO. Includes a RobbyBot attendant.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 73 | 1.5 | MULTI HMG, Chain Rifle (+1B), Mine Dispenser, E/M CCW | Deepspace Armored required-choice max 2 |

### Carlota Kowalsky, Tomcats Sergeant

**ID 427 · AVA 1 · LI** — `MOV 10-10 | CC 15 | BS 13 | PH 11 | WIP 14 | ARM 2 | BTS 0 | W 1 | S 2`. Engineer, Parachutist (Deployment Zone), Climbing Plus, Terrain (Zero-G), Deactivator, GizmoKit.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 28 | 0 | Breaker Combi Rifle, Light Flamethrower, Adhesive Launcher Rifle, D-Charges, Pistol, CCW | — |
| 2 | 32 | 0 | Same; includes Moriarty the Zondcat | — |

### Iguana Squadron

**ID 383 · AVA 2 · TAG** — full TAG `MOV 15-10 | CC 17 | BS 14 | PH 16 | WIP 13 | ARM 6 | BTS 6 | W 4 | S 7`. ECM: Guided, ECM: Hacker, Repeater, Tactical Awareness, Transmutation (Escape System), No Wound Incapacitation. Transmutes into an Iguana Operator.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 64 | 1.5 | AP HMG, Heavy Flamethrower (+1B), Mine Dispenser, CCW | Surface Armored required-choice max 2 |
| 2 | 68 | 1.5 | AP HMG, Heavy Flamethrower (+1B), CCW | same |

## Canonical Fireteam chart

Fireteam limits in the pinned source: **Core 1; Haris 1; Duo unlimited** (`DUO: 256` sentinel).

### Corregidor Surface Fireteams

**Types:** Haris, Core, Duo

| Entry | Min | Max | Required-choice | Counts as / note |
|---|---:|---:|---|---|
| ALGUACIL | 0 | 5 | yes | Corregidor |
| WILDCAT | 0 | 5 | yes | Corregidor |
| MOBILE BRIGADA | 0 | 5 | yes | Corregidor |
| TERRITORIAL | 0 | 3 | yes | Corregidor |
| COYOTE FTO | 0 | 2 | yes | Corregidor; FTO profiles only |
| BAMBADROID | 0 | 2 | no | Corregidor; Coyote dependency applies |
| VORTEX | 0 | 1 | no | Spec-Ops mode only |

The five `required-choice` rows are a required-choice set from the Army chart; they are not interpreted here as requiring one of every row simultaneously.

### Geckos Surface Fireteams

**Types:** Duo, Haris

| Entry | Min | Max | Required-choice | Note |
|---|---:|---:|---|---|
| GECKO | 1 | 3 | no | — |
| WILDCAT | 0 | 1 | no | — |

### Surface Armored Fireteams

**Types:** Duo

| Entry | Min | Max | Required-choice | Note |
|---|---:|---:|---|---|
| IGUANA | 0 | 2 | yes | — |
| WILDCAT | 0 | 1 | no | — |
| BAMBADROID | 0 | 1 | no | Coyote dependency applies |

### Wildcards Surface

These entries can join legal Surface Fireteams according to the chart.

| Entry | Max | Profile restriction / note |
|---|---:|---|
| VOSTOK | 1 | FTO profiles only |
| DAKTARI | 1 | — |
| STEMPLER ZOND | 1 | No chart-level FTO restriction |
| SHIFTA | 2 | Surface only |
| SEÑOR MASSACRE | 1 | Correctional tag in source comment |
| VALERYA GROMOZ | 1 | — |
| LUPE BALBOA | 1 | Corregidor tag in source comment |
| JAZZ | 1 | FTO profile only |

### Correctional Fireteams

**Types:** Duo, Haris, Core

| Entry | Min | Max | Required-choice | Note |
|---|---:|---:|---|---|
| LOBO | 0 | 4 | yes | Correctional |
| DIABLO | 0 | 4 | yes | Correctional |
| JAGUAR | 0 | 4 | yes | Correctional |

The three `required-choice` rows are a required-choice set from the Army chart; they are not interpreted here as requiring one of every row simultaneously.

### Corregidor Deepspace Fireteams

**Types:** Haris, Core, Duo

| Entry | Min | Max | Required-choice | Counts as / note |
|---|---:|---:|---|---|
| ALGUACIL | 0 | 5 | yes | Corregidor |
| WILDCAT | 0 | 5 | yes | Corregidor |
| MOBILE BRIGADA | 0 | 5 | yes | Corregidor |
| EVADER | 0 | 3 | yes | Corregidor |
| LOBO | 0 | 4 | no | Corregidor |
| TAG-TREIBER | 0 | 1 | no | — |
| VORTEX | 0 | 1 | no | Spec-Ops mode only |

The four `required-choice` rows are a required-choice set from the Army chart; they are not interpreted here as requiring one of every row simultaneously.

### Geckos Deepspace Fireteams

**Types:** Duo, Haris

| Entry | Min | Max | Required-choice | Note |
|---|---:|---:|---|---|
| GECKO | 1 | 3 | no | — |
| EVADER | 0 | 1 | no | Geckos |

### Deepspace Armored Fireteams

**Types:** Duo

| Entry | Min | Max | Required-choice | Note |
|---|---:|---:|---|---|
| GATOR | 0 | 2 | yes | — |
| GECKO | 0 | 1 | no | — |
| WILDCAT | 0 | 1 | no | — |

### Wildcards Deepspace

These entries can join legal Deepspace Fireteams according to the chart.

| Entry | Max | Profile restriction / note |
|---|---:|---|
| VOSTOK | 1 | FTO profiles only |
| DAKTARI | 2 | — |
| STEMPLER ZOND | 1 | No chart-level FTO restriction |
| SEÑOR MASSACRE | 1 | Correctional tag in source comment |
| VALERYA GROMOZ | 1 | — |
| LUPE BALBOA | 1 | Corregidor tag in source comment |
| JAZZ | 1 | FTO profile only |

## Reverse Fireteam index

| Unit | Fireteam access |
|---|---|
| Alguacil | Corregidor Surface Core/Haris/Duo; Corregidor Deepspace Core/Haris/Duo |
| BambaDroid | Corregidor Surface Core/Haris/Duo max 2; Surface Armored Duo max 1; Coyote dependency applies |
| Coyote FTO | Corregidor Surface Core/Haris/Duo max 2; FTO profiles only |
| Daktari | Surface Wildcard max 1; Deepspace Wildcard max 2 |
| Diablo | Correctional Core/Haris/Duo max 4 |
| Evader | Corregidor Deepspace Core/Haris/Duo max 3; Gecko Deepspace Haris/Duo max 1 |
| Gator | Deepspace Armored Duo max 2 |
| Gecko | Gecko Surface Haris/Duo 1–3; Gecko Deepspace Haris/Duo 1–3; Deepspace Armored Duo max 1 |
| Iguana | Surface Armored Duo max 2 |
| Jaguar | Correctional Core/Haris/Duo max 4 |
| Jazz FTO | Surface Wildcard max 1; Deepspace Wildcard max 1 |
| Lobo | Correctional Core/Haris/Duo max 4; Corregidor Deepspace Core/Haris/Duo max 4 |
| Lupe Balboa | Surface Wildcard max 1; Deepspace Wildcard max 1 |
| Mobile Brigada | Corregidor Surface Core/Haris/Duo max 5; Corregidor Deepspace Core/Haris/Duo max 5 |
| Señor Massacre | Surface Wildcard max 1; Deepspace Wildcard max 1 |
| Shifta | Surface Wildcard max 2 only |
| Stempler Zond | Surface Wildcard max 1; Deepspace Wildcard max 1 |
| TAG-Treiber | Corregidor Deepspace Core/Haris/Duo max 1 |
| Territorial | Corregidor Surface Core/Haris/Duo max 3 |
| Valerya Gromoz | Surface Wildcard max 1; Deepspace Wildcard max 1 |
| Vortex Spec-Ops | Corregidor Surface and Deepspace main teams max 1 in Spec-Ops mode |
| Vostok FTO | Surface Wildcard max 1; Deepspace Wildcard max 1; FTO profiles only |
| Wildcat | Corregidor Surface Core/Haris/Duo max 5; Gecko Surface Haris/Duo max 1; Surface Armored Duo max 1; Corregidor Deepspace Core/Haris/Duo max 5; Deepspace Armored Duo max 1 |

## Reinforcement linkage

The pinned Corregidor Army data links Reinforcement roster **599**. This reference deliberately keeps Reinforcement roster entries and Reinforcement-specific Fireteams separate from the standard Corregidor chart.

## Source pinning

- Army source version: `7.26246.158`
- Army backup commit: `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b`
- Corregidor source blob: `c8f7d9ced663b907e61e35694d7207b78b7c9d77`
- InfinityDB semantics commit: `4e2662be3f43387fbae42b3790a711b3e98570c4`
- Rules baseline: N5.3 + N5 FAQ v0.1
- Verified: 2026-10-15

## Mission specialist / button-pusher choices (N5.3)

**Moran FO15–18/.5** is an exceptional midfield button/repeater/CrazyKoala package with Infiltration and Mimetism(-3); a Repeater profile and 1-use Camo profile are *different*. **Jazz FTO HD+22/.5** or **Jazz+Billie25/.5** provides Hacking Device Plus/Pitcher and related Order infrastructure; two different selections. **Evader Engineer24–29** repairs while climbing/fighting, but **AP Spitfire Specialist Operative** is *not* simultaneously Engineer. **Coyote FO27–33** has MSV1/Warhorse and BambaBot when actual profile permits.

[Cross-game apex and value specialist tier guide](../../notes/list-building/mission-specialists-and-button-pushers-apex-value.md). The unit profiles/Fireteams above control exact legality.

## Airborne and enemy-DZ attack choices — N5.3 (2026-10-23)

**Deepspace**: **Hellcat BSG+Adhesive19, Hacker22, Paramedic23** trades via Combat Jump or standard Parachutist; **Tomcat Paramedic17/Engineer22** supplies reliable *side-edge* objective/repair; **Carlota28/32 Parachutist(DZ)** is direct enemy-edge Engineer/short-range attack. **Surface**: **Bearcat KHD29–30, Engineer28, Paramedic27** is NWI/Warhorse/BS13 dual-role aerial pressure. **Meteor Zond19/21** drops FO/Sensor/Repeater for the *hacking network*, not mainly kills. **These Surface vs Deepspace access pools differ**; current roster's Fireteam and segment restrictions apply. The 2026 Dante video claims PH12+3 Hellcat jump but this abbreviated pinned roster does **not** list +3; verify modifier before planning numeric odds.

See [current cross-game apex/value, landing odds and expected-trade tiers](../../notes/list-building/airborne-and-enemy-dz-attackers-apex-value.md). **This roster and Fireteam chart control exact loadout/availability.**

## Active-turn gunfighter cross-reference (2026-10-23)

**Active-turn shooting choices:** **Intruder HMG38/1.5** uses Camo/MSV2 with faction smoke to win otherwise poor vision FtF; the sniper(+1SD) variant serves longer reactive lanes. **Vostok Mk12/Spitfire34–38** uses Mimetism(-6) and Climbing, with only roster-legal division-specific FTO permissions. **Surface Territorial AP MMR29/0 TacAware + Marksmanship** is often superior repeated midrange value to 32pt/1.5SWC Red Fury; division differences matter. **Gecko54–55** is a compact **TAG**, while **Deepspace Gator** buys the larger assault package. [Gunfighter tiers with TAGs separately classified](../../notes/list-building/active-turn-gunfighters-apex-and-value.md).

## Warbands and inexpensive trading roles — N5.3

**Diablo Light Shotgun/Trench-Hammer8/0 or SMG9/0** is one of the best cheap **Berserk CC23** anti-HI options when **Lobo FT Master/Correctional required-choice** enables its route; it has printed **Irregular+Impetuous**, 2W/Transmutation and NO self Smoke. **Jaguar Chain+Smoke10/0** is **Regular**, adds Dogged and enables **Intruder MSV2 smoke-shooting**; 11pt Adhesive+Panzerfaust version trades at range against heavy units. **McMurrough23/0** is better at sustained solo crashing but consumes Irregular/personal Orders. After one successful CC kill, prefer preserve Jaguar Smoke/scoring paths to chasing a 10pt second target.

[Cross-game warband/cheap-trader apex and value tiers, targets and command packages](../../notes/list-building/warbands-and-cheap-trading-units-apex-value.md). Profile-specific sectorial legality/Fireteams above control all selections.

## DZ assault via airborne entry — video-tested interpretation (2026-10-28)

[Infinity the Dante: *Deployment Zone Assault — Drop Troop Tactics*](https://www.youtube.com/watch?v=fzvUQPWBQKM) compares **Deepspace Hellcat, Carlota+Moriarty and Tomcat** with **Surface Bearcat** against a Svalarheima DZ guarded by Pilot-X/RacerBots and a RemDriver-supported TR bot. Use the **landing pocket → network/Hacker disruption → key ARO/Disco removal → stop or score** sequence. An off-table **Tomcat can wait** if both entry edges are guarded. **Narration errors versus these authoritative profiles:** **Hellcat Paramedic Opt8 (23/0) has no Deployable Repeater**; **Bearcat Paramedic Opt5 (27/0) has Deployable Repeater but no Adhesive Launcher Rifle** (Adhesive belongs to **Bearcat KHD Opt2 29/0**). **Tomcat DR Opt3 (19/.5)** is separate from **Tomcat Paramedic Opt9 (17/0)**; **Meteor Zond** has native Repeater. This source compares mutually exclusive **Surface and Deepspace** division options, not one legal list. The [fully transcript-checked tactical breakdown](../../notes/factions/corregidor.md#airborne-dz-assault-workshop--infinity-the-dante-28-october-2026-transcript-audit) contains entry lanes, unit-specific uses, and risks. **No canonical roster/profile/Fireteam values are changed by this video.**

## TAG tactical cross-reference (2026-10-23)

**Gator (73)** wins the straightforward armor/gun plus NCO/TacAware/mine role. **Gecko (49–55)** is superior when legal Gecko links and a second active piece create useful Orders at low cost. **Iguana (64–68)** has AP HMG, Repeater and a post-shell operator plan, but its survivability/failure state is disputed. The 2025 podcast's '2 wounds' argument is **not the current reference**: this file specifies the TAG state **W4**.

Cross-faction **apex vs points-value** comparisons, matchup table, and direct MCP-reviewed podcast/video sources: [N5.3 TAG field guide](../../notes/list-building/tags.md). Current profile and Fireteam legality above remain authoritative.

## Hacker and KHD tactical cross-reference (2026-10-23)

**Jazz + Billie HD+ with Trinity, 25/0.5**, or **Jazz FTO 22/0.5**, is the first serious network controller: Pitcher/White Noise/Trinity interact well with **Moran Repeaters**. **Wildcat HD 27/0.5 Zero Pain + Combat Instinct** adds resilient defensive HD inside a legal Fireteam, while **Coyote KHD+Carbonite 23/0 FTO or 28/0 with BambaBot** and **Bearcat Combat Jump KHD+Firewall 29–30/0** create different anti-Hacker attacks. **Valerya HD 19/0.5 Total Control(+1B)** is affordable TAG control; **Alguacil HD 15/0.5** is a minimalist alternative. **Counterpoint (WIP12 E208, June 2026):** Moran/Jazz + Guided missile bot can consume substantial SWC before buying a main gun; don't force Guided into every list.

See the [cross-game apex/value Hacker/KHD tier guide](../../notes/list-building/hackers-and-killer-hackers.md). **The sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative; device upgrades are profile-specific.**


## Cheerleader / Order-generation tactical cross-reference (2026-10-23)

See the N5.3 [cross-game apex/value rankings and transcript-backed competing assessments](../../notes/list-building/cheerleaders-and-order-generators.md). The current roster and official Fireteam definitions above remain authoritative; unit access/cost may differ from vanilla.

- 7pt Transductor — cheap Regular Repeater/Flash REM (not a dedicated gunfighter); its S3 footprint and AVA constrain spam.
- 8pt Salyut — Baggage/Repeater Regular Order; reload support and deployment-zone density determine marginal value.
- 10pt Alguacil — inexpensive S2 Regular and Fireteam/LT material; upgrade only for a credible second job.
- 3pt Warcor — very useful Irregular Flash ARO/cheap screen, NOT an ordinary transferable Order.

**Selection rule:** Count deployed, transferable Regular Orders per Combat Group, not total models or restricted bonus Orders; choose the lowest-cost protected Regular profile that *also* contributes a relevant Repeater, Baggage, Fireteam, template, ARO or Specialist job. Check Group slots and DZ hiding space before buying a third large-base REM or replacing a needed scoring piece.


## ARO apex/value cross-reference (2026-10-23)

See [Best ARO Units — N5.3 apex and cost-value tiers](../../notes/list-building/aro-units-apex-and-value.md) for gunfighter vs hidden-trap vs cheap Order-tax comparisons, when each wins, transcript disagreements and counterplay. **The roster, prices/AVA and canonical Fireteam chart above remain authoritative**; a shared unit's permissions do not transfer between armies.

- **Reaktion Thunderbolt TR** — 19pt/0SWC recoverable guard; complement mines/repeaters, not a sole primary defence
- **Moran Koalas/Repeater** — mission-route mine/perimeter and hacking-area denial, not just a gunfight
- **Warcor Flash Pulse** — 3pt Irregular zero-SWC Order-tax ARO; never count as a generic Regular Order

**Deployment choice:** put the disposable/tax ARO on the approach, preserve a separate hidden/mission-denial gate where legal, and avoid leaving an expensive active-turn gun as your only exposed defence. Test pie-slicing, Smoke/Eclipse/White Noise, hacking, AD entry, recovery access and specialist survival before paying more SWC for a second sniper.

## N5.3 midfield area denial / speed bumps (tactical synthesis)

**Best passive network piece:** **Moran BSG Repeater+CrazyKoala Minelayer 15/.5**, AVA2: infiltrated Regular FO, perimeter tripwire and immediate hacker ARO access. **The Camo(1 use) BSG 16/.5 is a *different profile* with no Repeater.** **Bandit 25/.5** can Minelayer a Shock Mine or Deployable Repeater but is Irregular; **Shifta E/M Minelayer 17/0** adds Surface Strategic Deployment/FT utility, not true Infiltration. **Counterpoint:** two Morans/Jazz/Vertigo already commit substantial SWC, so choose Guided only when the mission/network justifies it; enemy Sensor/Deactivator or non-Hackable scouts may sweep them.

[Cross-game apex/value, matchups, and video/podcast disagreements](../../notes/list-building/midfield-area-denial-and-speed-bumps-apex-value.md). Qualitative tactics; the unit profile tables above remain authoritative.

## Doctor / Engineer / Recovery cross-reference (2026-10-23)

**Clockmaker18 + Zondbot3** is the cheap safe home repair network; **Tomcat Engineer22/26 incl. Zondcat** or **Carlota28/32 incl. Moriarty** reaches a downed **Gecko/Gator/REM** on a distant flank by Parachutist/Climbing. **Evader Engineer24/29/35** is durable combined assault/repair, while a **Wildcat Engineer25** can pay too much for mismatched combat/tools (Toolbox video dispute). **Daktari14** is the inexpensive VITA Doctor. [Doctor/Engineer apex/value, odds and media disagreement](../../notes/list-building/doctors-engineers-and-recovery-apex-value.md).

## N5.3 DZ defense / anti-alpha-strike tactical choices

**Moran Repeater+CrazyKoala Minelayer 15/.5 (AVA2)** is the cheapest *outer* Repeater/physical network; two can deter flank rushes while Jazz waits safely behind. **Important anti-IMP limit:** Boost is not triggered by IMP-1/IMP-2 or Camo markers, so Morans alone do not secure Jazz/Clockmaker/cheap Alguaciles from Fiday/Speculo. **Warcor 360º3/0** is a cheap edge alarm; **Transductor7/0 Flash/Repeater** is a Regular support body; **Salyut8/0 Deactivator/Baggage/Repeater** doubles as logistic support. **Opponent view:** WIP12 post-Mazebreaker warns that two Morans + Jazz + Vertigo consumes SWC; retain real active gun and two independent scoring paths instead of buying only defensive hacking.

[Whole-game DZ-defender apex/value guide, counters and transcripts](../../notes/list-building/dz-defenders-alpha-strike-and-impersonation-apex-value.md).

## Close-combat assassins and counter-CC — N5.3 (2026-10-23)

**Diablo8/0** (CC23 Berserk/NBW, Trench-Hammer, nominal 2W/Transmutation) is an outstanding **cheap conditional high-end melee trade**, especially when a legal **Lobo Correctional Fireteam** delivers it; **Irregular/Impetuous** and No Cover make a naked turn-1 charge expensive. **Jaguar10/0** is Regular Smoke/DA team/support value at CC22 MA1; **Lobo20** has NBW/Berserk but often better as **PARA (-9) control** than raw damage. Do not call Berserk a free Normal-roll guaranteed trade under current N5. [Dedicated CC assassin apex/value, delivery and counter-CC](../../notes/list-building/dedicated-close-combat-assassins-apex-value.md).

## N5.3 network projection — Pitchers, Repeaters, TinBots and disposable delivery

**Two Moran BSG Repeater15/.5 (AVA2)** start **two free infiltrated hacking zones** with Koalas and FO; current best Turn-0 network benchmark. **Jazz+Billie25/.5** provides HD+/Trinity/Pitcher and **2 Regular Orders** (Billie native Repeater), while **Jazz FTO22/.5** is separate, link-compatible but no Billie. **Bandit Deployable Repeater Minelayer25/.5** puts a third midfield *node* down during deployment; **Meteor19/0** is airborne native Repeater; **Stempler15/0** follows with FO/Sensor/Climbing. **Opposing WIP12 2026 view:** Moran+Jazz is strong, but Vertigo Guided + links cost SWC; one Hacker with firearms or a gun-first list may outscore full Guided. Koalas do not Boost at IMP/Camo markers.

[Cross-game apex/value guide, exact delivery cost and transcript disagreements](../../notes/list-building/network-projection-repeaters-pitchers-apex-value.md). Profile and Fireteam tables above remain authoritative.

## Tactical cross-reference — toolbox units (2026-10-23)

**Evader AP Spitfire Engineer35/1.5** combines real midrange AP gun, WIP13 Engineer/GizmoKit, NWI/Climbing+, Deactivator, and TinBot(-3). **Evader AP Spitfire31/1 is Specialist Operative, NOT Engineer**. **Evader BSG Engineer24/0** usually maximizes support value; the **Gecko+Evader+Stempler** legal Deepspace module is high-ceiling shared gun/repair/scoring/repeater but costs all three troopers and proper Fireteam access. **Coyote FTO KHD+Carbonite23** is Surface-only and is a different toolbox plan. [N5.3 toolbox tiers](../../notes/list-building/jack-of-all-trades-toolbox-units-apex-value.md).

## N5.3 rare abilities & unusual combinations — tactical synthesis

**Coyote FO27/0 with BambaBot-1/2** gets a **Forward Observer controller plus synchronized combat peripheral** in an FD(+10), MSV1, X-Visor, Warhorse package. **BambaDroid FO13/0** is *another selectable dependent REM* with a **Coyote in the same Combat Group**, not that BambaBot: **Coyote27 + BambaDroid FO13 =40/0** gives two FO-capable *troopers*, not a synchronized double-FO skill. Additional BambaDroids limited by Coyote count/group. **Opposing WIP12:** useful MSV/BambaDroid utility/mission flex, but a fragile multi-body setup can cost Orders and unnecessarily crowd a Moran/Jazz/Gecko plan. **Señor Massacre25–27/0 Eclipse+E/M grenades+CC** gives separate rare linkable close-approach control.

[Whole-game rare capability apex/value, rules, matchups and opposing MCP transcripts](../../notes/list-building/rare-capabilities-and-unique-combinations-apex-value.md). Use current profile and Fireteam chart above.

## Anti-TAG / Anti-HI without hacking — N5.3 (2026-10-23)

**Jaguar11 Adhesive Launcher Rifle+Panzerfaust+Smoke** is one of the cheapest dual answers (**IMM-A** versus damage). **Shifta17 E/Marat+E/M Mine**, **Tomcat Paramedic17 Panzerfaust/Parachutist**, and **Vigilante26 E/Mitter/Camo/FD+20** attack close or flank routes. **Territorial Engineer28/0 AP SMG+E/Mitter+Panzerfaust + Tactical Awareness** supplies **three modes and technical scoring**; **Evader32 Feuerbach** offers ranged AP+DA. **Diablo8 Trench-Hammer** is **not Disposable(3)** under N5.3, but still needs a safe CC/short throwing angle. **Choose by engagement:** Jaguar/Shifta in short TAG routes, **Vigilante/Territorial E/Mitter** when a ranged disabling shot is feasible, **Evader Feuerbach** for repeated long-lane damage. [WIP12 E208](https://open.spotify.com/episode/342lz18SRGSZ8QWf1Zg3Z9) contrasts linked E/Mitter versus conventional guns; its older Trench-Hammer charge discussion predates N5.3. [Anti-TAG/HI non-hacking apex/value rankings](../../notes/list-building/anti-tag-anti-heavy-infantry-non-hacking-apex-value.md).

## Tactical cross-reference — indirect fire (2026-10-23)

**Guided network verdict:** **Vertigo Guided16/1.5** behind **Moran Repeater FO15/.5 ×2 + Jazz HD+22–25/.5** is high ceiling, but uses **3 SWC before the primary gun**. Tactical Awareness values saturation and indirect threat; **WIP12 E208 (June 2026)** and a TA co-host warn that Spotlight/Save/Reset/Dodge rolls, spread defenders and newer Surface/Deepspace direct guns make the launcher *optional*, not mandatory. **Vanilla Nomads has Moran AVA1**, not Corregidor AVA2. [Whole-game Guided vs Spec tiers and transcripts](../../notes/list-building/indirect-fire-speculative-guided-apex-value.md).

## N5.3 objective holding, zone domination & carried-objective choices

**Gecko Vulkan49/0** is exceptional **49VP of 3STR/ARM6** with Tactical Awareness and 0SWC, 54–55/1 gives stronger range; **Gator73/1.5** 3STR/ARM8 is premium central counterattack/zone but not ordinary box Specialist. **Sombra FO29/0** Camo/FD+20/NWI/Climbing+ is excellent *box retrieval/vertical escape*, but **cannot re-enter marker state carrying Supplies**. **Mobile Brigada HD36/.5** W2/ARM5 360º/Firewall is tougher specialist carrier where source-legal link works; **Moran FO/Repeater15/.5** is superb 0-Order zone guard and eligible FO but W1/ARM0 **not your exposed final carrier**. **Coyote FO27/0 + BambaBot** defends two angles, whereas **independent BambaDroid FO13/0** requires Coyote same combat group. **Opposing:** better 2 independent scoring pieces than 2 expensive Gecko if mission is picking boxes rather than raw zone points.

[Whole-game objective holding/zone apex/value, scenario scoring and opposing media](../../notes/list-building/objective-holding-zone-domination-and-carriers-apex-value.md). Actual sectorial profiles and Fireteam chart remain authoritative.

## Anti-Tech — enemy visors, Mimetism, markers and Impersonation (2026-10-23)

**Jazz FTO HD+22/.5 / Jazz+Billie25/.5** plus Moran Repeaters projects **White Noise** to blind MSV and Marksmanship across a real approach, rather than pay a premium to outshoot the visor. **Intruder MSV2 HMG38/1.5 + Jaguar Smoke10/0** is the complementary *kill the Mimetism gun* attack; **Stempler Sensor/FO REM** hunts Camo/Hidden once within ZoC, and **Lobo Biometric** guards against Impersonators in actual Correctional/Deepspace legal configurations. **Counter:** do not buy a White Noise plan when the enemy ARO is non-MSV; do not import a Surface-only link into Deepspace.

[Anti-Tech N5.3 apex/value tiers, matchup rules and opposing MCP viewpoints](../../notes/list-building/anti-tech-msv-mimetism-camo-impersonation-apex-value.md).

## Force multipliers — N5.3 role/value cross-reference (2026-10-23)

**Mobile Brigada TinBot Firewall(-6)33/0** supports legal heavy hacker/HI teams, whereas **Evader Firewall(-3)23/0** is cheaper Deepspace protection and Specialist; choose based on enemy Comms MOD. **Shifta Strategic Deployment17/0** grants legal Surface Fireteam FD(+4″), valuable if the mission rewards it but not if it exposes an entire expensive link. **Vigilante Counterintelligence25–29** is disputed versus Moran15/.5 Turn-0 Repeaters; **TAG-Treiber11–12 TAGCom** applies only to same-group TAG using actual printed bracket MODs. **Salyut8 Baggage vs14/.5 EVO** depends on expected REM Supportware. [Transcripts and tiers](../../notes/list-building/force-multipliers-special-abilities-apex-value.md).

## N5.3 peripheral / synchronized / multi-body apex-value update

**Coyote27/0 BSG+attached BambaBot** puts **FO/MSV1, FD(+10)** and one synchronized bot through two firing lanes on one Order; **Coyote28/0 KHD+bot** changes job, **MMR+bot33/0** increases attack reach. A **BambaDroid FO13/0** with 360º/Mim(-3)/Deployable Repeater is a **separate dependent REM** (Coyote present, same group, cannot outnumber Coyotes); BambaBot is **NOT** this unit and does **not** inherit FO. **Coyote FTO19/0 BSG** instead has NO BambaBot and team rights. **Moran Minelayer/Repeater15/.5** is great passive board gate but CrazyKoala is deployable equipment, not synchronized live attacker. **WIP12 E208 counterviews:** attached bot+MMR gives double-origin pressure; the 13pt AP/FO Droid buys genuinely independent active response, costs an actual 13pt and consumes own group slot/orders. **Anaconda-style Ancillary nuance:** Gecko/Gator RobbyBots not deployed free; must Place Deployable and can affect Fireteam/integrity.

[Whole-game N5.3 Peripheral & Multi-Body Apex/Value guide](../../notes/list-building/peripheral-synchronized-multibody-apex-value.md). Source profiles, dependency and Fireteam tables above remain authoritative; media are opinions.

## Battle-report effectiveness and combinations (qualitative, 2026-11-01)

**Observed packages:** **Jazz/Billie + Moran Repeaters/Koalas + an Evader/Engineer or Fireteam gun**, backed by **Wildcat/Mobile Brigada/Vostok, Iguana/Gator/Gecko** depending on the mission, establishes both electronic and template defenses (#071, #078, #080). In #186, **two Gecko TAGs + Jazz + Intruder lane + Jaguars** beat a double-heavy Druze force in Cutthroat, partly through Flash Pulse/Stunned Order denial rather than winning every TAG roll. [#071–#080](../../notes/battle-reports/071-080-n5-battle-report-tactical-analysis.md) · [#186](../../notes/battle-reports/181-190-n5-battle-report-tactical-analysis.md).

**Counterplay / risk:** #238 saw **ISS Pitcher → Deva KHD Trinity** remove **Jazz**, opening Adil's route despite Corregidor's forward network. That match also showed **Iguana/McMurrough** attacks failing to accomplish the mission while independent ISS Taowu remained to score. [#238](../../notes/battle-reports/231-240-n5-battle-report-tactical-analysis.md).

**Practical lesson:** Distributed Morans/Koalas work only with a **protected hacker and actual objective runner**; consider counter-pitcher angles, protect edge/rear corridors, and keep an attack plan if Jazz is neutralized. Validate distinct Corregidor Surface vs Deep Space rosters in the current reference.

[Cross-report synthesis and evidence cautions](../../notes/battle-reports/cross-report-unit-effectiveness-and-combinations.md).

## Mission performance — battle-report evidence (2026-11-01)

| Mission(s) | Tested composition / scoring mechanism | Evidence |
|---|---|---|
| **Cutthroat** | Double Gecko + Jazz/Intruder/Jaguar screen controlled heavy opposition and finished 6–3 against Druze. | [#186](../../notes/battle-reports/181-190-n5-battle-report-tactical-analysis.md) |
| **Evacuation / Neutralization** | Moran repeaters/Koalas + Jazz, Wildcat/Evader Engineer and Bearcat/other mobile specialist variants for objective delivery, not only heavy guns. | [#078](../../notes/battle-reports/071-080-n5-battle-report-tactical-analysis.md), [#080](../../notes/battle-reports/071-080-n5-battle-report-tactical-analysis.md) |
| **Hardlock counterexample** | Iguana/McMurrough guns and Moran/Jazz network were bypassed after ISS Pitcher/Deva KHD removed Jazz; Taowu finished a 4–1 ISS win. | [#238](../../notes/battle-reports/231-240-n5-battle-report-tactical-analysis.md) |

**Limits:** Printed Surface vs Deep Space eligibility and scenario version must be checked. A single hacker's loss can collapse the network plan. Game-era qualitative evidence, not a win-rate or current Fireteam claim. [Full mission evidence audit](../../notes/battle-reports/cross-report-mission-performance-by-sectorial.md).

## Counterplay — observed N5 battle-report responses (2026-11-02)

| Threat / target | Observed response and limitation | Battle reports |
|---|---|---|
| **Vs heavy TAG / Fireteam** | Jazz/Moran Koalas and Repeaters + Vertigo Guided attacked Starmada linked units; double Gecko, Intruder and Flash/Jaguar screens defeated Druze Scarface/Anaconda 6–3. | [#078](../../notes/battle-reports/071-080-n5-battle-report-tactical-analysis.md), [#186](../../notes/battle-reports/181-190-n5-battle-report-tactical-analysis.md) |
| **Counter enemy hacker** | Moran/Jazz network is **vulnerable to counter-Pitcher**: ISS Zhanying/Wu Ming Pitcher enabled Deva KHD Trinity to kill Jazz and bypass front network (4–1). | [#238](../../notes/battle-reports/231-240-n5-battle-report-tactical-analysis.md) |
| **Vs hidden/endgame attacker** | McMurrough Smoke/Jaguar flanking plus Wildcat/Evader engineer and Vostok recovery are alternatives, but a failed McMurrough late LT strike did not flip Decapitation vs ALEPH. | [#126](../../notes/battle-reports/121-130-n5-battle-report-tactical-analysis.md), [#211](../../notes/battle-reports/211-220-n5-battle-report-tactical-analysis.md) |

**Limit:** #078 Iguana received a card granting temporary Specialist; this is **not** baseline Iguana. Distinguish Surface versus Deep Space historical rosters. These are historical qualitative interactions, not current N5.3 profile/Fireteam or faction win-rate claims. [Full cross-report counterplay analysis](../../notes/battle-reports/n5-cross-report-counterplay-tags-hi-hacking-camo-impersonators-fireteams.md).

---

## Must-have / Go-to / Avoid — source-backed recommendations (2026)

Dated source-backed tactical preferences and miniature purchasing priorities; opinions do not override N5.3 roster, profile or Fireteam data above.

**Original audit title:** Nomads — Vanilla, Corregidor, Bakunin, Tunguska: Must-have / Go-to / Avoid

*Source-backed list-building audit — 23 October 2026. Applies to the canonical [Vanilla Nomads](nomads.md), [Corregidor](corregidor.md), [Bakunin](bakunin.md), and [Tunguska](tunguska.md) N5.3 rosters, pinned to the **3 September 2026 Army data**. These are named-player tactical opinions and tested constructions, **not measured global tournament pick rates**. Latest main's profile/AVA/Fireteam source controls over any 2024–2026 video. Full tactical companions: [Vanilla](../../notes/factions/vanilla-nomads.md), [CJC](../../notes/factions/corregidor.md), [Bakunin](../../notes/factions/bakunin.md), [Tunguska](../../notes/factions/tunguska.md).*

### Classification standard

- **Must-have / near-must:** a recorded presenter explicitly says “every list”, “always” or “auto-include”; or independently supported recurrent list core. Only “near-must” when credible examples omit it. The *job* can be essential without a particular unit being compulsory.
- **Go-to:** outstanding reliable value for its **actual job**, but list architecture, mission, terrain or overlapping tools can make it unnecessary. Do not assume all go-tos go into one 300-point list.
- **Never take / strong avoid:** direct recorded critique **of the named profile**, preferably comparing a same-faction replacement. Mark **contested/conditional** where a different speaker defends it, a current changed roster undermines the critique, or it has a real special use. None of the four armies has a supported universal ban covering every profile of an entire multi-role unit.
- Evidence marks: **explicit** = reviewer states the near-auto/negative claim; **repeat** = published list examples, not population statistics; **reasoned** = synthesis of reviewer observations + current roster, and therefore *not* pretended to be a direct podcast verdict.

### 2. Corregidor (Army 502, **Surface OR Deepspace**)

**Near-must/default**

| Unit | Why and qualification | Evidence |
|---|---|---|
| **Moran Repeater BSG15/.5**, usually **two** (AVA2) | Excellent Turn-0 midfield Repeater/CrazyKoala board control; two separately cover approaches to give the hacker real projection. 0.5 SWC each can squeeze direct-fire SWC, and some mission-specific non-Guide lists replace one. | **[WIP12 E208 — Post-Mazebreaker CJC (June 2026)](https://open.spotify.com/episode/342lz18SRGSZ8QWf1Zg3Z9)** repeatedly builds two Moran network shells; [Tactical Awareness CJC](https://open.spotify.com/episode/1ngCemrrDVMMDgvWjNBMYY). **High-confidence archetype default**, not verbatim "all lists" statistical claim. |
| **Jazz & Billie25/.5 or Jazz FTO22/.5** | HD+/Pitcher/Trinity makes forward Morans dangerous. Billie = **two Regular Orders** and autonomous utility; **FTO-only** = Fireteam/TinBot option (not Billie). **Very compelling backbone if paying for two Repeaters**, not mandated in a smoke/straight-gun mission. | [WIP12 E208](https://open.spotify.com/episode/342lz18SRGSZ8QWf1Zg3Z9); [Tactical Awareness CJC](https://open.spotify.com/episode/1ngCemrrDVMMDgvWjNBMYY). |

**Go-to**

| Unit | Why and matchup | Evidence |
|---|---|---|
| **Intruder MULTI Sniper38/1.5 (+1 Special Die, MSV2/Camo)** | Reliable reactive **and** active long lane, combines especially well with Jaguar/McMurrough Smoke; use HMG when long/active range and no sniper lane. | [WIP12 E208](https://open.spotify.com/episode/342lz18SRGSZ8QWf1Zg3Z9) at ~82 and 121m explicitly calls the *MULTI Sniper* auto-include in its own builds; comments on opposing Orders spent routing around it. *One host's list style, not all CJC.* |
| **Deepspace Gecko MMR54/1 + Evader Engineer + Stempler TacAware18** | Paired independent extra orders and direct shooting, Engineer recovery, third specialist and Sensor/repeater. **Do not import into Surface**: Surface Gecko team uses **Wildcat** in place of Evader. | [WIP12 E208](https://open.spotify.com/episode/342lz18SRGSZ8QWf1Zg3Z9) ~41–55m, ~121–124m worked team example. |
| **Vostok FTO34–35**, with relevant legal Fireteam | Mimetism(-6)/2W attack REM gets meaningful link/Engineer backstop. **FTO variant loses Repeater**; use separate standalone 37–38 version to project network. | [WIP12 E208](https://open.spotify.com/episode/342lz18SRGSZ8QWf1Zg3Z9) ~43–46m says its original N5 weakness was overturned by **2026 team changes**. |
| **Intruder smoke escort: Jaguar**, **Wildcat hacker/Engineer**, **Transductor7**, **Salyut8**, **Stempler Sensor/TacAware**, **Bandit minelayer** | Jobs include enabling MSV2 smoke fights, Combat Instinct/Stealth defense, cheap Orders, extra midfield mine/deployable network. Bandit is **Irregular**, despite forward-control quality. | [WIP12 E208](https://open.spotify.com/episode/342lz18SRGSZ8QWf1Zg3Z9) ~75m explicitly calls Wildcat hacker a staple and ~122m includes Bandit minelayer as an auto in *sample* list; [Dante Corregidor after split](https://www.youtube.com/watch?v=dNoJI8nPnIU). |
| **Surface: Coyote+BambaBot, Territorial29 AP MMR+TacAware, Shifta Strategic Deployment, Bearcat AD**; **Deepspace: Gator, Evader, Hellcat/Tomcat/Carlota** | Strong **division-dependent**, not interchangeable. Surface pressure uses peripherals/TA/AD, Deepspace better heavy engineering and traditional airborne scoring. | [WIP12 E208](https://open.spotify.com/episode/342lz18SRGSZ8QWf1Zg3Z9); [Shepherd + Ollie 2026 faction update](https://www.youtube.com/watch?v=NRRP4Fects8) was a preview and may have superseded details. |

**Strong avoids (profile + job, not blanket unit bans)**

| Profile | Verdict / same-army alternative | Recorded basis and exception |
|---|---|---|
| **Surface Territorial AP Red Fury32/1.5** as all-purpose gun | **Prefer 29/0 AP Marksman Rifle with X-Visor + same TacAware** when long/mixed ranges or SWC pressure dominate; **Red Fury's higher Burst** has a real active-turn payoff and its 32pt LT option is separate. | [WIP12 E208](https://open.spotify.com/episode/342lz18SRGSZ8QWf1Zg3Z9) favors MMR cost/value; **not strict outclassing** because of Burst/range. |
| **Costlier generic Tomcat** bought merely to attack rear with a gun | **19/0 Hellcat BSG/Adhesive Combat Jump** often attacks cheaper; **17pt Tomcat Paramedic**, Engineer22–26, Doctor22–26, Carlota each solve real missions. Not a ban on Tomcats. | [WIP12 E208](https://open.spotify.com/episode/342lz18SRGSZ8QWf1Zg3Z9) ~123–128m *self-corrects* an earlier “never Tomcat profile” claim after discussing a mission which makes one valuable. **This is an explicit counterexample to literal “never”.** |
| **Gecko Vulkan Shotgun49/0** as your **sole range opener** | Shotgun short-band cannot force a 24–32in defensive ARO; use **Gecko MMR54/1**, Intruder, another long gun when the actual first lane requires it. Vulkan can dominate dense rooms. | [WIP12 E208](https://open.spotify.com/episode/342lz18SRGSZ8QWf1Zg3Z9) panel split: one tested a Vulkan and found Evader did the fighting, other sees close-table utility. **Contested, not never.** |

**Strict legality:** choose **Surface or Deepspace**. **Gator and Evader** are the Deepspace plan; **Coyote, Territorial, Shifta, Bearcat** are Surface. The joint canonical roster alone does not make those formations legal together. **Jazz FTO/Vostok FTO** link only as permitted by division chart.

### Fast starting template (not a fixed shopping list)

| Army | **Near-default consideration** | Add **one** game plan | First cuts when over budget |
|---|---|---|---|
| **Vanilla** | Morlock ×1–2; Moran Repeater ×1; a hacker (Interventor/Jazz) and cheap Regular support | Szalamandra/Gator/Gecko gun, Guided network, or solo assisted Vostok + mission specialists | Unlinked Grenzer sniper; Go-Pod if acting as first ARO gun; duplicate high-price hackers |
| **Corregidor** | Moran Repeater ×1–2, Jazz, a real long gun (Intruder sniper often) | Deepspace Gecko/Evader/Stempler **or** Surface Territorial/Coyote/Bearcat; smoke/MSV | Territorial AP Red Fury when 0SWC MMR suffices; unnecessary Tomcat vs Hellcat overlap; Guided without targets |
| **Bakunin** | Morlock ×1, one path-control/CC threat, a real gun and a specialist | Chimera/Cenobite zone assault; Riot/Uhahu protected network; Vostok/Clockmaker or Lizard/Stigmata gun/denial | Generic Zellen as duplicate Morlock role; Moderator Spitfire; unplanned Go-Pod |
| **Tunguska** | Puppet Master11, Interventor HD+, cheap Transductors/warband screen | Hollow Men/Perseus team; Kriza/Szalamandra gun; Pitcher/Heckler/Meteor program | 40+pt Triggermen with no distinct role; unlinked Grenzer costly gun; Go-Pod before safer first attacker |

### Primary evidence queue — directly checked with connected video/podcast transcripts

| Priority | Recording | Most important directly grounded point |
|---|---|---|
| 1 | **[Robert Shepherd — Vanilla Nomads, 2026](https://www.youtube.com/watch?v=dOtvw5FKOfo)** | Explicit **two Morlocks**, Moran baseline; explicit Grenzer-sniper skepticism; network versus real guns |
| 2 | **[WIP12 E208 — Corregidor Post-Mazebreaker, June 2026](https://open.spotify.com/episode/342lz18SRGSZ8QWf1Zg3Z9)** | Intruder MULTI Sniper near-auto speaker's list; 2026 Vostok reappraisal; Gecko-Evader-Stempler; Surface Territorial MMR; **self-corrected “never Tomcat”** |
| 3 | **[Shepherd — Bakunin N5](https://www.youtube.com/watch?v=firJVr1eDWg)** | Morlock-over-Zellenkrieger explicit; Moderator Spitfire explicit avoid; Chimera strong but high-skill; Vostok teams |
| 4 | **[MetaChemistry #132 — Bakunin tournament winner](https://open.spotify.com/episode/1S2sIe6nlefj4TZlZuII9g)** | **No Stigmata/Go-Pod/Guided**, minimal hacking, Orphan MSV2 anti-smoke; third-party Go-Pod auto-include claim **and** winner's own nonuse |
| 5 | **[Shepherd — Tunguska N5](https://www.youtube.com/watch?v=A2eKdenbcsw)** | Explicit Puppet Master **basically always**; Interventor/Hollow Men; Go-Pod low-floor and Triggermen criticism |
| 6 | **[MetaChemistry #129 — Tunguska Takedown](https://open.spotify.com/episode/6XSTLXqQUFcjv9lYcDTZ6g)** | Elite Interventor hacking, expensive guns, **Denma/Zellen nearly every list**, opponents beat hacking/CC exposure |
| 7 | **[Tactical Awareness Tunguska](https://www.youtube.com/watch?v=PFAewbgodZc)** | Competing ambitious Go-Pod, Puppet-Red-Fury, Kriza and Triggermen ideas |
| 8 | **[Tactical Awareness Nomad Prime](https://open.spotify.com/episode/2PpxuDu2WlxipiqpVzHTdv)** | Gecko gun, mass hacking/Guided, EVO REM as three valid but mutually competing Vanila approaches |
| 9 | **[Dante Vanilla N5](https://www.youtube.com/watch?v=hJKOZF1Je_g)** · **[Dante Bakunin](https://www.youtube.com/watch?v=DVOHynBsg6o)** | Older opposing views on nomad hacker/REM utility and Riot-versus-Reverend efficiency |
| 10 | **[Tactical Awareness CJC](https://open.spotify.com/episode/1ngCemrrDVMMDgvWjNBMYY)** · **[Loss of Lieutenant TAG debate](https://open.spotify.com/episode/1h5CJfZC5zBPxdg66o7xIN)** | Mixed TAG and infrastructure builds; premium gun opportunity costs |

#### N5.3 guardrails

- **Do not transplant list legality across ships**. Corregidor **Surface and Deepspace are different selectable divisions**; Vostok/Jazz **FTO** variants are not always the same as their independent profile. Vanilla has **0 Core / 1 Haris / 2 Duo**; no general Fireteam privilege follows from the string `FTO`.
- **Lunokhod** footage in older Nomad analyses does **not** describe a unit in the pinned ordinary rosters; don't suggest the removed model as current go-to. **Bakunin Zoe standalone 23pt** in older footage is not current ordinary roster access: pinned Bakunin has paired Zoe+Π-Well FTO instead.
- **Go-Pod** and premium hackers have real, explicit opposing opinions. **Do not flatten** them into unambiguous auto-include or never-purchase verdicts.
- An interviewer calling a piece "auto-include" in **their personal event list** is **not** proof it is on every successful list. A unit absent from one tournament winner is likewise **not proof it is bad**.

### Whole-unit purchasing audit — skip the model, not one loadout (2026-10-30)

**No uncontested full-unit never-buy** is established for any of these four rosters. The following **model-level deferrals** are useful when choosing what to *purchase first*, but the stated niche or dissent prevents a categorical ban.

| Army | Entire model/unit to defer | Why / when to buy instead |
|---|---|---|
| **Vanilla Nomads** | **No supported whole-unit skip** | Grenzer **unlinked sniper** competes poorly with Intruder; Grenzer's other profiles/sectorial links remain different. Go-Pod as first-turn linebreaker is risky, but late mobility is a real role. |
| **Corregidor** | **No supported whole-unit skip** | Territorial AP Red Fury versus MMR, Tomcat versus Hellcat and Gecko Vulkan versus MMR are **loadout/role** comparisons, not reasons to avoid the whole unit. |
| **Bakunin — Zellenkrieger** | **Defer generic Zellenkrieger purchase** if you already use **Morlocks** for smoke/trades | [Shepherd Bakunin](https://www.youtube.com/watch?v=firJVr1eDWg) directly favors 6pt Morlock to generic 8pt Zellen. **Do not label all Zellenkrieger forbidden:** the FTO's Taskmaster/Riot synergies and Natural Born Warrior/other attributes create genuine choices. **Extreme Zellenkrieger** is *a different unit* and not covered by this verdict. |
| **Tunguska — Triggermen** | **Defer as a first premium gun/ARO miniature; disputed** | [Shepherd Tunguska](https://www.youtube.com/watch?v=A2eKdenbcsw) prefers Kriza HMG or much cheaper Reaktion for common roles; **K1 Decoy/Forward Deploy** and Tactical Awareness sniper experiments provide special uses. |
| **Tunguska — Go-Pod** | **Defer if you need a Turn-1 main attacker** | No Cover/S7/hackability is a bad ARO-breaking floor, but fast late flanking/Go-Bot tricks are unique; [Tactical Awareness](https://www.youtube.com/watch?v=PFAewbgodZc) offers an opposing positive interpretation. |

**Not model-level:** Moderator Spitfire and Grenzer Sniper are weapon/profile negatives; don't skip the whole Moderator/Grenzer miniature family. [Cross-faction shortlist](../../notes/factions/model-purchase-avoid-summary-2026.md).

### Worst-value, rarely necessary and proxy-first miniature purchases by army (2026-10-30)

**Question answered:** which entire Nomads *miniatures* are a low-priority buy, which profiles should usually be avoided even though their unit has good options, and which **perfectly useful** miniatures or extra copies can be **proxied before buying**? This is a *shopping order*, not a new “never take” consensus or a claim about measured tournament frequency. **“Rare / circumstantial” here means not needed for ordinary first-choice list architectures in the recorded commentary**; the source videos/podcasts do not provide a reliable pick-rate survey. Latest [N5.3 army/sectorial data]() is the authority for profiles, availability, silhouette and Fireteam memberships.

**Strength of the verdict:** **Skip by default; proxy if needed** is a genuine *whole-model purchasing* deferral grounded in a speaker’s negative everyday-role comparison. **Proxy/test before buying** is an *inference* from credible niches and opportunity cost, **not** a speaker's assertion of overall weakness. **Avoid profile only** means the *other loadouts/sculpts of the unit remain worthwhile*. **Proxy another copy** refers to duplicate physical models or weapon sculpts, not a ban on a legal simultaneous AVA. **Contested** keeps materially opposing speaker/tournament evidence visible.

#### 2. Corregidor — Surface versus Deepspace purchases must be separate

The two current Corregidor divisions have **different roster/chart permissions** even though the repository's index aggregates the unit families. **Surface**: Coyotes, Territorials, Shifta and the relevant Iguana team routes. **Deepspace**: Evaders, Gator and its distinct Gecko/Evader team, and traditional mobile recovery/airborne plans. Do **not** buy a unit solely for a team that belongs to the *other* division. [Corregidor current roster](corregidor.md); [WIP12 E208, post-Mazebreaker June 2026](https://open.spotify.com/episode/342lz18SRGSZ8QWf1Zg3Z9).

**Surface-specific weaker/rare buying cases**

| Unit / role | Weak point or competing purchase | Verdict |
|---|---|---|
| **Territorial AP Red Fury 32/1.5 as generic all-range gun** | **Direct — WIP12 E208** strongly prefers **29pt/0SWC AP Marksman Rifle + X-Visor / TacAware** for range and SWC efficiency. Red Fury’s higher Burst / aggressive shorter range is a *real* reason to take it, not strict dominance. | **Avoid *Red Fury profile* by default; proxy its sculpt/loadout** using a distinct Territorial. **Do not skip Territorials**; the MMR/Engineer/command roles can be excellent. |
| **Coyote purchased without its BambaDroid/BambaBot payload plan** | **Reasoned:** Coyote FO/MSV1 + mine/repeater peripheral is a strong Surface fork but often depends on *both* main operator and extra physical unit. The **23pt Coyote FTO KHD** for a link is *not* the same body-count configuration as the independent peripheral build. | **Proxy/test exact package before buying extra Coyote and BambaDroids**. Buy when that **forward fork / linked specialist** is repeatedly used. Do not treat the first Coyote as weak. |
| **Second Iguana or Gecko TAG in a list already buying a Territorial/Coyote main attack** | **Contestable:** 2026 reworked **Iguana** gained a better attack/survival case than outdated 2025 ratings; Gecko MMR/utility also have normal uses. TAG/Tactical Awareness can be a central plan, but three competing expensive shooters strain objectives and support. | **Proxy another TAG**; buy only after a **legal Surface Armored or Gecko** concept repeatedly works. **Do not apply old pre-buff “Iguana bad” verdict.** |
| **Large Surface-linked Mobile Brigada/Wildcat gun brick with redundant heavy guns** | **Reasoned — [CJC guide](../../notes/factions/corregidor.md):** Wildcats have MSV1/Combat Instinct and Engineers, Mobile Brigada can provide TinBot defense; a full expensive team *just to give one fighter more guns* often costs too many Orders. Cheap Alguaciles/Morans/Transductors remain useful. | **Proxy extra HI/MI gun sculpts**, not the first required/missing support member. Buy the exact **legal** team once the useful member count is known. |

**Deepspace-specific weaker/rare buying cases**

| Unit / role | Source critique and valid exception | Verdict |
|---|---|---|
| **Gecko Vulkan Shotgun49/0 as the only ARO opener** | **Direct and contested — WIP12 E208**: a short-range gun struggles to open 24–32in lanes; **MMR54/1** usually handles long fire better. On dense/close tables the Vulkan can be excellent. | **Avoid the *Vulkan-as-long-range-opener profile*, not Gecko**; **proxy alternate weapon option** on the same appropriate TAG model. |
| **Generic costly Tomcat gun where a Hellcat attack is the objective** | **Direct with reviewer's self-correction — WIP12 E208** prefers **19pt Hellcat BSG Combat Jump** for economical rear-entry attack; but **Tomcat Paramedic17, Engineer/Doctor22–26 or Carlota** can rescue/scoring from different access lanes. **Tomcat is not Combat Jump.** | **Proxy-test a gun-only Tomcat**, not “never buy Tomcat.” A dedicated **Engineer, Doctor, Paramedic or Carlota** model is useful if your scenario needs its skill or deployment. |
| **Sombra as a routine second midfield skirmisher instead of Moran/Bandit** | **Recorded skeptical comparison in [CJC guide](../../notes/factions/corregidor.md):** expensive ~29–40pt one-model midfield NWI/FO/KHD often unnecessary after Morans project the network, cheap Bandit mines/FO and other scoring cover. **Durable independent specialist is a genuine niche.** | **Proxy first**, especially if buying a second Sombra. Buy for a specific **survivable infiltrating/scoring** plan; **not** a mathematically bad unit. |
| **Second premium Gator, Gecko or Evader body when the Deepspace repair/attack team is already complete** | **Reasoned:** a **Gecko MMR + Evader Engineer + Stempler TacAware** is an evidenced package; spare large guns/Engineers without a distinct mission role inflate cost. Gator and additional Evaders can be valid in different teams. | **Proxy the *additional* expensive body/chassis**. Do **not** skip a first **Evader** if it is the repair/Fireteam piece that makes your chosen TAG work. |

**Shared Corregidor choices across both division plans**

| Model or scheme | Main downside | Shopping action |
|---|---|---|
| **Third/fourth Intruder long-gun sculpt; sniper/HMG variants in the same list** | **Inferred:** [WIP12 E208](https://open.spotify.com/episode/342lz18SRGSZ8QWf1Zg3Z9) **loves the MULTI Sniper** as a real threat, often taking one. Buying many high-cost MSV2 guns just because **Intruders AVA5** may neglect scoring and leave few attacking Orders. | **Proxy extra Intruders and profile variants first**; **do not skip the first strong MSV2 MULTI Sniper**. |
| **Jazz FTO and Jazz+Billie purchased as though one model does both** | **Legality/body count:** Jazz FTO gets specific Fireteam access **without Billie**; Jazz+Billie is a distinct two-model **two-Regular-Order** selection with no automatic link. Both use similar lead Jazz sculpts. | **Buy one Jazz representation before duplicates**; proxy loadout. If choosing Jazz+Billie, **physically supply Billie**; do not purchase Billie for an FTO list. |
| **Vostok FTO versus unlinked Vostok; separate second Vostok chassis** | **Current N5.3:** FTO gives legal CJC Wildcard/team utility but **does not have the standalone Repeater**. WIP12's earlier skepticism was updated after 2026 team improvements. | **Do not skip Vostok for obsolete ratings**. **Proxy the second chassis / gun loadout** if never used simultaneously; buy for a specific link or independent repeater. |
| **Vertigo Guided without a maintained Moran/Jazz/FO Targeted plan** | **Reasoned:** good hacking pressure if the whole network and Order sequence are present, but **1.5SWC** directly competes with the Intruder sniper's SWC. | **Avoid unsupported Guided strategy**, not the Vertigo model in all possible lists; proxy/test before buying another missile REM. |
| **Ruby Monday, extra Bearcat/Carlota/other named off-table attackers without a planned second approach** | **Lower-confidence inference:** very specialized drop/mission/payload packages; [newer DZ-attack discussion](../../notes/factions/corregidor.md#airborne-dz-assault-workshop--infinity-the-dante-28-october-2026-transcript-audit) explains entry-angle and opponent DZ screens. Their simultaneous inclusion is not routine. | **Proxy individual unusual sculpt before buying**, with correct body size and team/peripheral count. **Do not call Bearcat/Hellcat inherently bad or confuse Combat Jump vs Parachutist.** |

**Preserve positive evidence:** first **Moran Repeater (often two in CJC)**, **Jazz chosen mode**, **Intruder MULTI Sniper**, **Gecko MMR**, **Vostok FTO**, **Wildcat/Engineer** and **Surface Territorial MMR/Coyote** each have strongly evidenced uses; the weak verdicts above target **role, *extra copies* or an unsuitable division**, not the unit family.

#### Across the four Nomads armies — additional proxy-first miniatures, even when good

**There is no checked-in Nomads physical inventory** under the obvious \`inventory/nomads.md\`, \`inventory/corregidor.md\`, \`inventory/bakunin.md\` or \`inventory/tunguska.md\` paths. **No claimed Nomads owned counts** are used here. A missing inventory file does not mean that you own none.

| Miniature somebody might buy | Better initial proxy/test option | Buy a separate model when… |
|---|---|---|
| **Named infantry/hackers** (Mary Problems, Jelena Kovač, Uhahu, Valerya Gromoz, Raoul Spector, Lupe Balboa, Perseus, Wolfgang, Cassandra Kusanagi, Agatha, Sforza) | An unused **correct-base/silhouette Corvus Belli infantry figure**, visibly distinct from the rest of your list, with the declared role written down. Do not assume two named AVA1 characters can be represented simultaneously by the same model. | The named capability is recurrent, *or* two similar-sized named characters are used concurrently and need unambiguous identities. A highly useful character can still be an excellent purchase even when testing by proxy is cheaper. |
| **Alternate hacker/gun sculpts** (Interventor HD+/KHD, Riot Grrl TinBot, Grenzer gun, Wildcats, Territorials, Evader, Moderator, Hollow Men, Stempler, Vostok) | Use one **same-unit/same-compatible-size miniature** and explicitly declare the chosen current N5.3 **profile/loadout**. FTO, Repeater, TacAware, TinBot and Counterintelligence are **profile-specific**. | You repeatedly field *two physically different bodies simultaneously*, or your event's proxy rules/readability demand dedicated representation. |
| **Morlocks/Zellen/Jaguars/Denma/Überfallkommando** | Borrow spare warband/CC sculpts when silhouette and unit count match; **Bakunin Morlock can initially represent generic Bakunin Zellen if allowed** but this does **not** make the Zellen unit or its rules identical. **Chimera requires three separately represented Pupniks**. | Your list has simultaneous multiple CC models beyond the available distinct pool, or a specific FTO body matters. **Do not proxy a solo Chimera as a complete squad.** |
| **Puppetactica Master + PuppetBots; Jazz + Billie; Zoe + Π-Well; Fiddler + Jackbots; Coyote + BambaDroids** | Test the whole **controller + required subordinate body count** with appropriately sized/scaled spare models; physical servants are not Regular Orders unless the chosen profile explicitly grants an independent Order. Check versions with/without extras. | You often field a two-or-more-body selection, or cannot meet separate body/silhouette count with spare proxies. **Jazz FTO has no Billie**; **Fiddler FTO has no Jackbots**; **Bakunin Zoe + Π-Well is paired in current standard roster**. |
| **Alternative Reaktion/Vertigo/Stempler/Salyut/Transductor/Meteor/Tsyklon/Vostok REMs** | Temporarily use an unused **correctly sized REM chassis**, with visible assignment to a specific trooper type. **S1 PuppetBots, S2 support remotes and larger combat REMs cannot be assumed interchangeable**; validate actual base and Silhouette. | Need distinct REM bodies in the **same list** (e.g., two Transductors, Stempler plus Vertigo), or the proposed chassis cannot reproduce the required footprint. |
| **TAG alternatives** (Gecko, Gator, Szalamandra, Stigmata, Lizard, Iguana, Anaconda) | Before purchasing a large kit, **borrow/proxy one correctly based/silhouetted TAG** and play several legal lists. Match gun/Engineer support concept; **not every TAG belongs to each sectorial**. | The specific armoured platform repeatedly earns the main-gun slot; buy extra *only* if multi-TAG/dual-Gecko lists are routine. |
| **Go-Pod aerial VH / Zondnautica / other mounted units** | Use a matching **Vehicle/appropriate motorcycle or composite-body** stand-in; these are **not** ordinary S2 troopers or generic TAGs. Respect **Zondnautica's transformation/body rules** and Go-Pod's applicable Go-Bot. | You choose the mobility strategy repeatedly and have proper physical forms/companions for that profile. |
| **Corregidor division-specific miniatures** | Proxy Surface **Coyote/Territorial/Shifta** and Deepspace **Gator/Evader** *from different lists*, never from the same made-up Surface+Deepspace blend. | You have actually selected one **current legal division and team**; only then fill any simultaneous physical gaps. |
| **Additional AVA copies for rare tools** (Triggermen, Sin-Eater, Grenzer, Sombra, Switcher, expensive second Hacker/Engineer) | Use the first suitable model or a distinct appropriately sized proxy. AVA is a legal maximum, *not a model-shopping goal*. | Multiple copies have already appeared **simultaneously and often** in your mission-driven lists. |

**Event/ownership caveats:** Reveal proxy substitutions and check current **Silhouette, base diameter, required partners, counts, and organized-play/organizer policy**. Ordinary infantry, heavy infantry, remotes, TAGs and S7 Vehicles **cannot automatically stand in for one another**. No separate plastic miniature is needed for a profile option **unless simultaneous distinct bodies or a stricter event rule calls for it**. Older ITS-season proxy language is not proof of current seasonal policy. **A proxy cannot grant a unit permission to join a Fireteam or a division in which it is not legal.**

**Practical buying shortlist:** **Strongest direct whole-model deferrals** are **Bakunin generic Zellenkrieger if Morlocks already do its only job**; **Tunguska Triggermen if bought as a generic first premium shooter**; and **Go-Pod in any army if bought solely as a Turn-1 ARO breaker** (contested by positive flank uses). **Strongest *profile-only* avoids** are **Vanilla unlinked Grenzer MULTI Sniper**, **Bakunin Moderator Spitfire**, **Corregidor Surface Territorial AP Red Fury where MMR is better**, **Deepspace Gecko Vulkan as a long-lane opener**, and **unsupported Vertigo Guided builds**. **Generally best proxy-first *good* purchases:** second TAG/alternate TAG chassis, extra Vostok/Tsyklon/REM, extra PuppetBot/Chimera/Coyote package beyond owned body counts, second/third premium character and fourth/fifth Fireteam gun sculpt. Keep the original positive/dissenting media opinions above when making an actual list.
