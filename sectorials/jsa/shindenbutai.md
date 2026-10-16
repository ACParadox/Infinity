---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 1102
sectorial_slug: shindenbutai
sectorial_name: Shindenbutai
parent_faction: JSA
parent_faction_id: 1101
rules_baseline: N5.3
army_source_version: "7.26246.159"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-16
coverage: "Complete current Shindenbutai main roster, exact standard loadouts and AVA, current Fireteam chart and reverse access index, optional Spec-Ops/Team-Ops boundary, linked Reinforcements boundary, source character-relation constraints, and derived tactical indexes."
---

# Shindenbutai — N5.3 sectorial reference

## Overview and provenance

Repository-native reference for **Shindenbutai** (Army sectorial ID `1102`), a JSA sectorial. It is intended to answer roster, profile, AVA, points/SWC, Lieutenant, specialist, hacking/network, deployment, peripheral and Fireteam questions without reopening Army.

Sources used:

- Corvus Belli Army-derived revision `7.26246.159` from `massayoshi/infinity-army-backup` commit `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b` (`army: N5.3 + ITS18`, 2026-09-03).
- Versioned source: `n5/shindenbutai/7.26246.159.json`, blob `3b48c5df4a55cb9cb54bf1053e00e77e939cf12b`.
- Aggregate source: `n5/shindenbutai/shindenbutai.json`, blob `75662995dc103c81c41a2d076bea0ef89b2c6e1d` at the pinned source commit.
- InfinityDB normalization/semantics: commit `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: N5.3 + N5 FAQ v0.1.

Coverage notes:

- Covers **36 standard Shindenbutai roster entries** explicitly assigned to faction `1102` by the current Army source.
- `Kaizoku Spec-Ops` (ID `1924`) and `JSA Team-Ops` (ID `1938`) are optional-mode entries and are kept separate from the standard roster.
- Generic Soldiers-of-Fortune / mercenary-catalogue objects with an empty `factions` array are excluded. Explicit Shindenbutai entries such as Monstruckers, Triphammer, Warcor, Sāchā, Ioann Bann and Ruby Monday are retained.
- Linked Reinforcement army ID: **1199**. Reinforcement-only profiles and Fireteams remain separate from this Main reference.
- Army raw Fireteam `DUO: 256` is the source sentinel for effectively unlimited Duo formations, not a literal limit of 256.
- Disabled subordinate forms/peripherals such as the Mechazoid's Kobaruto and the Triphammer's TurtleMek are documented with their parent unit and are not counted as independent roster entries.
- `FTO` and specific profile restrictions are preserved wherever the Fireteam chart relies on them.

## Sectorial summary

| Field | Value |
|---|---|
| Sectorial | Shindenbutai |
| Parent faction | JSA (`1101`) |
| Army ID | `1102` |
| Rules baseline | N5.3 + FAQ v0.1 |
| Standard Main roster entries | 36 |
| Optional-mode entries | Kaizoku Spec-Ops; JSA Team-Ops |
| Reinforcement roster | Army ID `1199` |
| Core | up to 1 |
| Haris | up to 1 |
| Duo | unlimited/source `256` sentinel |
| Fireteam families | Senku; Bushi-tai; Sayō (Action); Yamabushi; Mechazoid |
| Explicit Wildcards | Shurayuki; Yuriko Oda FTO |

## Fireteam chart limits and sectorial-level restrictions

| Constraint | Current source value / normalized meaning |
|---|---|
| Core | `1` |
| Haris | `1` |
| Duo | `256` — normalized as unlimited Duos |
| Main/Reinforcement mixing | Main roster and Reinforcement roster `1199` remain separate |
| Wildcards | Only the explicit Wildcard rows listed below |
| Profile restrictions | Preserve `FTO`, `(Strategic Deployment)`, `Spec-Ops`, counts-as and source-required semantics exactly |

The chart contains five named Fireteam families plus a separate Wildcard list. A profile merely being labelled `FTO` elsewhere in Army does **not** grant Fireteam access unless the Shindenbutai chart actually includes it.

## Standard roster index

| Unit | Unit ID | AVA | Type | Classification | Regularity | Primary hooks |
|---|---:|---:|---|---|---|---|
| Tokusetsu Butai | 158 | 2 | LI | Support | Regular | Doctor/Engineer |
| Senku Troops | 1817 | 5 | LI | Line Troops | Regular | cheap orders, Lt, FO, Paramedic, Commlink |
| Nokizaru Unit | 1826 | 2 | SK | Spec. Trained | Regular | MSV1, KHD/FO, mobile skirmisher |
| Shurayuki | 1829 | 1 | MI | Veteran | Regular | elite CC, NWI, Wildcard `(Senku)` |
| Kurayami Ninjas | 1825 | 2 | SK | Spec. Trained | Regular | Hidden Deployment, HD, mines |
| Mechazoid Sōkōrentai | 1788 | 2 | TAG | Mechanized | Regular | TacAware TAG, Lt, Kobaruto, Duo |
| Robio Aibōt | 1833 | 1 | REM | Support | Regular | cheap Repeater |
| Hatamoto Imperial Guard | 1823 | 2 | HI | Headquarters | Regular | NCO, specialist, Lt +1 Order/+1 SWC |
| Warcors | 50 | 1 | LI | Mercenary | Irregular | Flash Pulse ARO |
| Metsuke Officers | 1818 | 1 | LI | Headquarters | Regular | Strategos Lt / Lt +1 Order, Counterintelligence |
| Yáoxiè Rui Shi | 159 | 2 | REM | Support | Regular | MSV attack REM, Sayō member |
| Monstruckers | 1333 | 1 | LI | Mercenary | Irregular | Engineer, Drop Bears/turret |
| Uran Aibōt | 1832 | 1 | REM | Support | Regular | Guided Missile Launcher |
| Yamabushi | 1824 | 2 | WB | Mercenary | Regular | FTO or camo assault profiles |
| Shizoku Kōgeki-tai | 1822 | 2 | HI | Veteran | Regular | heavy attack; FTO or Strategic Deployment |
| Kaizoku Yuriko Oda | 1019 | 1 | LI | Character | Regular | Engineer, mines, Wildcard FTO |
| Yojimbo, Motorized Sword for Hire | 224 | 1* | WB | Character | Irregular + Impetuous | smoke, Koalas, fast CC |
| Saito Togan | 668 | 1 | SK | Character | Regular | HD/camo, smoke, elite CC |
| Yojimbo, Sword for Hire | 1834 | 1* | WB | Character | Irregular + Impetuous | smoke, Koalas, CC |
| Garon Aibōt | 1831 | 1 | REM | Support | Regular | Total Reaction, HMG/Mk12/smoke GL |
| Triphammer | 1569 | 1 | TAG | Mercenary | Regular | TacAware TAG, TurtleMek |
| Teishin Guntai | 1820 | 2 | MI | Spec. Trained | Regular | Combat Jump, HD/KHD/FO |
| Taguraidā TAG Support Pilots | 1828 | 1 | LI | Support | Regular | TAG support specialist; Senku FT |
| Yáoxiè Lù Duān | 160 | 2 | REM | Support | Regular | Holoprojector, MSV1, E/M |
| Jizamurai Hanryodan | 1821 | 5 | MI | Elite | Regular | primary Bushi-tai body, flexible assault |
| Atom Aibōt | 1830 | 1 | REM | Support | Regular | Sensor, FO, Repeater; Mechazoid Duo |
| Aïda Swanson | 1160 | 1 | LI | Character | Regular | FTO/mines or solo FD profile |
| S.T.R.S. Tanuki Team | 1819 | 5 | MI | Veteran | Regular | CoC, Eng, hacker, MSV2 weapons, Lt |
| Yáopú Pangguling | 162 | 1 | REM | Support | Regular | Baggage/EVO/Repeater/TR |
| Kyojin Killers | 1827 | 2 | SK | Spec. Trained | Irregular | forward assault, templates |
| Yáozăo | 161 | 3 | REM | Support | Peripheral | Servant |
| Raiden Seibutai | 167 | 3 | MI | Elite | Regular | Hidden Deployment, Minelayer, HRL/ML |
| Ninjas | 135 | 1 | SK | Spec. Trained | Regular | Hidden Deployment, HD/KHD/FO |
| Sāchā, Xenotech Hunters | 1874 | 1 | LI | Mercenary | Irregular | cheap specialist, E/M grenades |
| Ioann Bann | 1940 | 1 | WB | Character | Irregular | Dog-Warrior, Sayō/Yamabushi FT |
| Kazurabā Ruby Monday | 1890 | 1 | HI | Character | Irregular | durable specialist, Adhesive/E/M |

`*` The two Yojimbo entries are alternate identities of the same character and are mutually exclusive; see **Character/relation constraints**.

## Unit details

### Tokusetsu Butai

**Unit ID:** 158  
**Slug:** `tokusetsu-butai`  
**AVA:** 2  
**Type:** LI · Support Troops · Regular

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 15 | 11 | 10 | 13 | 1 | 0 | 1 | 2 |

**Common:** Courage.

| Profile ID | Pts | SWC | Loadout / profile-specific rules |
|---:|---:|---:|---|
| 1 | 14 | 0 | **EISEI Doctor**; Combi Rifle, Pistol, CCW; MediKit |
| 2 | 14 | 0 | **KOHEI Engineer**; Combi Rifle, D-Charges, Pistol, CCW; Deactivator, GizmoKit |
| 3 | 15 | 0 | KOHEI Engineer as above + Deployable Cover |
| 4 | 17 | 0 | KOHEI Engineer as above + Armed Turret (Combi Rifle) |

### Senku Troops

**Unit ID:** 1817 · **Slug:** `senku-troops` · **AVA:** 5 · **LI / Line Troops / Regular**  
`MOV 10-10 | CC 15 | BS 11 | PH 10 | WIP 12 | ARM 0 | BTS 3 | W 1 | S 2`. Courage.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 9 | 0 | Combi Rifle, Pistol, CCW |
| 2 | 17 | 1 | HMG, Pistol, CCW |
| 3 | 11 | 0 | Shock Marksman Rifle, Pistol, CCW |
| 4 | 11 | 0 | Combi Rifle, Pistol, CCW; **Commlink, Specialist Operative** |
| 6 | 10 | 0 | Combi Rifle, Flash Pulse, Pistol, CCW; **Forward Observer** |
| 7 | 11 | 0 | Combi Rifle, Pistol, CCW; **Paramedic, MediKit** |
| 8 | 9 | 0.5 | Combi Rifle, Pistol, CCW; **Lieutenant** |

### Nokizaru Unit

**Unit ID:** 1826 · **Slug:** `nokizaru-unit` · **AVA:** 2 · **SK / Spec. Trained / Regular**  
`MOV 10-10 | CC 23 | BS 12 | PH 12 | WIP 13 | ARM 0 | BTS 6 | W 1 | S 2`. MSV1; Martial Arts L3, Mimetism (-3), Stealth, Climbing Plus, Terrain (Zero-G), Courage and mobility/defence modifiers as encoded by source.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 30 | 0 | MULTI Marksman Rifle, Silenced Pistol, Shock CCW |
| 2 | 27 | 0 | SMG, Shock Mine, D-Charges, Silenced Pistol, Shock CCW; **KHD** |
| 3 | 25 | 0 | SMG, Flash Pulse, Shock Mine, D-Charges, Silenced Pistol, Shock CCW; **FO** |

### Shurayuki

**Unit ID:** 1829 · **Slug:** `shurayuki` · **AVA:** 1 · **MI / Veteran / Regular**  
`MOV 10-10 | CC 23 | BS 12 | PH 12 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. Holomask, X-Visor; Martial Arts L4, NWI, Stealth, Immunity (Shock), Religious Troop.

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 30 | 0 | MULTI Rifle, Nanopulser, Pistol, Viral CCW |

**Fireteam:** explicit Wildcard, counts as **Senku**.

### Kurayami Ninjas

**Unit ID:** 1825 · **Slug:** `kurayami-ninjas` · **AVA:** 2 · **SK / Spec. Trained / Regular**  
`MOV 10-10 | CC 22 | BS 11 | PH 13 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 2`. Bangbomb (+4); Martial Arts L2, Hidden Deployment, Infiltration, Mimetism (-3), Surprise Attack (-3), Stealth, Super-Jump, Terrain (Zero-G).

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 22 | 0 | SMG, Viral Mine, Pistol, DA CCW |
| 2 | 26 | 0.5 | Light Shotgun, Viral Mine, D-Charges, Pistol, DA CCW; **Hacking Device** |
| 3 | 23 | 0.5 | SMG, Viral Mine, Pistol, DA CCW; **Minelayer** |

### Mechazoid Sōkōrentai

**Unit ID:** 1788 · **Slug:** `mechazoid-sokorentai` · **AVA:** 2 · **TAG / Mechanized / Regular**  
`MOV 15-10 | CC 23 | BS 13 | PH 15 | WIP 13 | ARM 6 | BTS 6 | STR 3 | S 6`. Hackable; ECM: Guided (-6); Martial Arts L2, BS Attack (SR-1), Tactical Awareness, Combat Instinct, Stealth, Climbing Plus, Religious Troop.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 66 | 1.5 | AP HMG, Pulzar, Panzerfaust, EXP CCW; **Tactical Awareness**; Kobaruto |
| 2 | 69 | 1.5 | Spitfire MULTI, Pulzar, Panzerfaust, EXP CCW; **Tactical Awareness**; Kobaruto |
| 3 | 69 | 1.5 | Profile 2; **Lieutenant + Tactical Awareness**; Kobaruto |

**Kobaruto Hojo-Bot:** disabled subordinate/Ancillary peripheral, `MOV 10-10 | PH 10 | WIP 13 | ARM 0 | BTS 3 | STR 1 | S 1`; Specialist Operative and Peripheral (Ancillary). It is not a separate roster selection.

### Robio Aibōt

**Unit ID:** 1833 · **Slug:** `robio-aib-t` · **AVA:** 1 · **REM / Support / Regular**  
`MOV 15-15 | CC 13 | BS 8 | PH 11 | WIP 13 | ARM 0 | BTS 3 | STR 1 | S 3`. Repeater, Remote Presence, Mimetism (-3), Courage.

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 7 | 0 | Flash Pulse, PARA CCW (-3) |

### Hatamoto Imperial Guard

**Unit ID:** 1823 · **Slug:** `hatamoto-imperial-guard` · **AVA:** 2 · **HI / Headquarters / Regular**  
`MOV 15-5 | CC 23 | BS 13 | PH 13 | WIP 13 | ARM 2 | BTS 6 | W 2 | S 2`. Hackable; Nanoscreen, X-Visor; Martial Arts L4, Natural Born Warrior, Combat Instinct, Mimetism (-3), Specialist Operative, Stealth, Frenzy. **Every current loadout has NCO.**

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 34 | 0 | Plasma Carbine, Heavy Pistol, Monofilament CCW, E/M CCW; **NCO** |
| 2 | 40 | 1 | Red Fury, Heavy Pistol, Monofilament CCW, E/M CCW; **NCO** |
| 3 | 41 | 1.5 | Spitfire, Heavy Pistol, Monofilament CCW, E/M CCW; **NCO** |
| 4 | 36 | **+1** | Profile 1; **Lieutenant (+1 Order), NCO** |
| 5 | 38 | **+1** | Profile 2; **Lieutenant (+1 Order), NCO** |
| 6 | 39 | **+1** | Profile 3; **Lieutenant (+1 Order), NCO** |

### Warcors

**Unit ID:** 50 · **Slug:** `warcors-war-correspondents` · **AVA:** 1 · **LI / Mercenary / Irregular**  
`MOV 10-10 | CC 11 | BS 9 | PH 11 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Journalist.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CCW (-3); **360º Visor** |
| 2 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CCW (-3); **Sixth Sense** |

### Metsuke Officers

**Unit ID:** 1818 · **Slug:** `metsuke-officers` · **AVA:** 1 · **LI / Headquarters / Regular**  
`MOV 10-10 | CC 21 | BS 12 | PH 12 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Holoprojector; Martial Arts L2, Counterintelligence, Surprise Attack (-3), Stealth, Immunity (Shock).

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 22 | 0 | MULTI Rifle, Flash Pulse, Heavy Pistol, Shock CCW; **Lieutenant, Strategos L1** |
| 2 | 23 | 0 | Same weapons; **Lieutenant (+1 Order)** |

### Yáoxiè Rui Shi

**Unit ID:** 159 · **Slug:** `yaoxie-rui-shi` · **AVA:** 2 · **REM / Support / Regular**  
`MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 6 | STR 1 | S 4`. Remote Presence, Courage.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 23 | 1 | Spitfire, PARA CCW (-3); **MSV2** |
| 2 | 21 | 0.5 | Red Fury, Mine Dispenser, PARA CCW (-3); **MSV1** |

### Monstruckers

**Unit ID:** 1333 · **Slug:** `monstruckers` · **AVA:** 1 · **LI / Mercenary / Irregular**  
`MOV 10-10 | CC 16 | BS 11 | PH 12 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Engineer, Climbing Plus; Deactivator, GizmoKit.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 15 | 0 | Boarding Shotgun, Adhesive Launcher Rifle, E/M Grenades, Pistol, CCW |
| 2 | 12 | 0 | SMG, Chain Rifle, Drop Bears, Pistol, CCW |
| 3 | 15 | 0 | SMG, Chain Rifle, Drop Bears, Armed Turret (AP Rifle), Pistol, CCW |
| 4 | 16 | 0 | Rifle, Light Shotgun, Akrylat-Kanone, D-Charges, Pistol, CCW; **360º Visor** |

### Uran Aibōt

**Unit ID:** 1832 · **Slug:** `uran-aib-t` · **AVA:** 1 · **REM / Support / Regular**  
`MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 0 | BTS 3 | STR 1 | S 3`. Remote Presence, Courage, BS Attack (Guided).

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 16 | 1.5 | Missile Launcher, PARA CCW (-3) |

### Yamabushi

**Unit ID:** 1824 · **Slug:** `yamabushi` · **AVA:** 2 · **WB / Mercenary / Regular**  
`MOV 15-5 | CC 23 | BS 11 | PH 13 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Martial Arts L3, Forward Deployment (+10), Mimetism (-3), Stealth, Frenzy, Dogged, Religious Troop, CC Attack (Shock).

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 15 | 0 | **FTO**; Chain Rifle, Panzerfaust, Heavy Pistol, DA CCW |
| 2 | 16 | 0 | **FTO**; Chain Rifle, Tactical Bow, Heavy Pistol, DA CCW; **Paramedic, MediKit** |
| 3 | 16 | 0 | Chain Rifle, Panzerfaust, Heavy Pistol, DA CCW; **Camouflage (1 Use)** |
| 4 | 16 | 0 | Chain Rifle, Tactical Bow, Shock Mine, Heavy Pistol, DA CCW; **Camouflage (1 Use)** |
| 5 | 17 | 0 | Chain Rifle, Tactical Bow (+1B), Panzerfaust, Heavy Pistol, DA CCW; **Camouflage (1 Use)** |

### Shizoku Kōgeki-tai

**Unit ID:** 1822 · **Slug:** `shizoku-kogeki-tai` · **AVA:** 2 · **HI / Veteran / Regular**  
`MOV 15-5 | CC 22 | BS 13 | PH 14 | WIP 13 | ARM 5 | BTS 6 | W 2 | S 2`. Hackable; Martial Arts L3, Berserk, Mimetism (-3), Stealth, Frenzy.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 43 | 1.5 | **FTO**; AP HMG, Chain Rifle, Pistol, AP+DA CCW |
| 2 | 33 | 1.5 | **FTO**; Heavy Rocket Launcher (+1B), Assault Pistol, AP+DA CCW |
| 3 | 38 | 1.5 | Heavy Rocket Launcher (+1B), Assault Pistol, AP+DA CCW; **Strategic Deployment** |

### Kaizoku Yuriko Oda

**Unit ID:** 1019 · **Slug:** `keisotsu-kaizoku-yuriko-oda` · **AVA:** 1 · **LI / Character / Regular**  
`MOV 10-10 | CC 15 | BS 12 | PH 11 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Engineer, Mimetism (-3), Minelayer; Deactivator, GizmoKit.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 25 | 0 | **FTO**; Combi Rifle, E/Mitter, D-Charges, Shock Mine, Pistol, CCW |
| 2 | 23 | 0 | **FTO**; Combi Rifle, Panzerfaust, D-Charges, Shock Mine, Pistol, CCW |
| 3 | 28 | 0.5 | Profile 1 weapons; **Forward Deployment (+20)**; non-FTO |

**Wildcard:** only FTO profiles; source counts-as `(Senku, Sayō)`.

### Yojimbo, Motorized Sword for Hire

**Unit ID:** 224 · **Slug:** `yojimbo-motorized-sword-for-hire` · **AVA:** 1 shared by identity · **WB / Character / Irregular + Impetuous**  
`MOV 20-15 | CC 24 | BS 12 | PH 14 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 4`. Motorcycle; Martial Arts L4, Limited Cover, Minelayer, NWI.

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 741 | 20 | 0 | Contender (+1B), Nanopulser, Smoke Grenades, CrazyKoala, Pistol, DA CCW |

Only one Yojimbo identity may appear in an Army List.

### Saito Togan

**Unit ID:** 668 · **Slug:** `saito-togan` · **AVA:** 1 · **SK / Character / Regular**  
`MOV 10-10 | CC 24 | BS 11 | PH 13 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Bangbomb (+4); Martial Arts L4, Camouflage, Hidden Deployment, Infiltration, Mimetism (-6), Surprise Attack (-3), Stealth.

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 33 | 0 | T2 Boarding Shotgun, Smoke Grenades, Pistol, EXP CCW |

### Yojimbo, Sword for Hire

**Unit ID:** 1834 · **Slug:** `yojimbo-sword-for-hire` · **AVA:** 1 shared by identity · **WB / Character / Irregular + Impetuous**  
`MOV 15-5 | CC 24 | BS 12 | PH 14 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Martial Arts L4, Minelayer, Stealth, No Cover, NWI.

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 19 | 0 | Contender (+1B), Nanopulser, Smoke Grenades, CrazyKoala, Pistol, DA CCW |

Mutually exclusive with Motorized Yojimbo and linked Reinforcement identities.

### Garon Aibōt

**Unit ID:** 1831 · **Slug:** `garon-aib-t` · **AVA:** 1 · **REM / Support / Regular**  
`MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | STR 1 | S 3`. 360º Visor, Remote Presence, Total Reaction, Courage.

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 23 | 1 | HMG, PARA CCW (-3) |
| 2 | 21 | 0 | Mk12, PARA CCW (-3) |
| 3 | 16 | 0 | Thunderbolt, Smoke Grenade Launcher, PARA CCW (-3) |

### Triphammer, Repurposed Industrial TAG

**Unit ID:** 1569 · **Slug:** `triphammers-repurposed-industrial-tags` · **AVA:** 1 · **TAG / Mercenary / Regular**

| State | MOV | CC | BS | PH | WIP | ARM | BTS | STR | S |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Full Power | 15-10 | 17 | 13 | 16 | 12 | 7 | 3 | 3 | 7 |
| Battle-Ravaged | 10-10 | 15 | 12 | 14 | 12 | 4 | 0 | 3 | 7 |

Transmutation; Tactical Awareness; each current profile includes a **TurtleMek Ancillary Remote Unit**.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 2 | 53 | 1.5 | AP Spitfire, Heavy Flamethrower, AP CCW; **Tactical Awareness** |
| 3 | 52 | 1.5 | AP Spitfire, Chain-colt (+1B), AP CCW; **Tactical Awareness** |
| 4 | 52 | 0 | Heavy Shotgun, Thunderbolt (+1B), AP CCW; **Tactical Awareness** |
| 5 | 48 | 0 | Heavy Shotgun, Heavy Rocket Launcher, Panzerfaust (+1B), AP CCW; **Tactical Awareness** |

**TurtleMek:** disabled subordinate/Ancillary peripheral (`MOV 15-10 | PH 10 | WIP 12 | ARM 0 | BTS 3 | STR 1 | S 1`), Specialist Operative; not an independent roster choice.

### Teishin Guntai

**Unit ID:** 1820 · **Slug:** `teishin-guntai` · **AVA:** 2 · **MI / Spec. Trained / Regular**  
`MOV 10-10 | CC 21 | BS 11 | PH 12 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. Martial Arts L1, Combat Jump, Parachutist, Stealth, Super-Jump (Jet Propulsion).

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 19 | 0 | Boarding Shotgun, D-Charges, Shock Mine, Pistol, Shock CCW |
| 2 | 23 | 0.5 | Boarding Shotgun, D-Charges, Pistol, Shock CCW; **Hacking Device** |
| 3 | 21 | 0 | Boarding Shotgun, D-Charges, Pistol, Shock CCW; **KHD** |
| 4 | 19 | 0 | SMG, Flash Pulse, D-Charges, Shock Mine, Pistol, Shock CCW; **FO** |

### Taguraidā, JSA TAG Support Pilots

**Unit ID:** 1828 · **Slug:** `taguraida-jsa-tag-support-pilots` · **AVA:** 1 · **LI / Support / Regular**  
`MOV 10-10 | CC 21 | BS 12 | PH 12 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Martial Arts L1, Stealth, TAGCom (`Dodge PH+3`, `GizmoKit PH+1`).

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 12 | 0 | `MECHAZOID PILOT`; Light Shotgun, Pistol, DA CCW; **Specialist Operative**, GizmoKit |

### Yáoxiè Lù Duān

**Unit ID:** 160 · **Slug:** `yaoxie-lu-duan` · **AVA:** 2 · **REM / Support / Regular**  
`MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 6 | STR 1 | S 4`. Holoprojector, MSV1; Remote Presence, Surprise Attack (-3), Courage.

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 24 | 0 | Mk12, Heavy Flamethrower, E/M Mine, PARA CCW (-3) |
| 2 | 20 | 0 | Thunderbolt, E/M Carbine, E/M Mine, PARA CCW (-3) |

### Jizamurai Hanryodan

**Unit ID:** 1821 · **Slug:** `jizamurai-hanryodan` · **AVA:** 5 · **MI / Elite / Regular**  
`MOV 15-5 | CC 23 | BS 12 | PH 13 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`. Martial Arts L3, Combat Instinct, Mimetism (-3), Stealth, Climbing Plus, Immunity (Shock), Courage.

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 21 | 0 | Light Shotgun, Pistol, DA CCW |
| 2 | 21 | 0 | Light Shotgun, Pistol, E/M CCW |
| 3 | 24 | 0 | Light Shotgun, E/Mitter, Pistol, DA CCW |
| 4 | 24 | 0 | Light Shotgun, Thunderbolt, Pistol, DA CCW |
| 5 | 22 | 0 | SMG, Pistol, DA CCW |

### Atom Aibōt

**Unit ID:** 1830 · **Slug:** `atom-aib-t` · **AVA:** 1 · **REM / Support / Regular**  
`MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | STR 1 | S 3`. Repeater, Deactivator; Triangulated Fire, Forward Observer, Remote Presence, Courage.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 15 | 0 | Combi Rifle, Flash Pulse, PARA CCW (-3); **Sensor** |
| 2 | 17 | 0 | Combi Rifle, Flash Pulse (+1B), PARA CCW (-3) |

### Aïda Swanson

**Unit ID:** 1160 · **Slug:** `aida-swanson` · **AVA:** 1 · **LI / Character / Regular**  
`MOV 10-10 | CC 19 | BS 12 | PH 11 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Martial Arts L2, Forward Deployment (+10), Mimetism (-3), Stealth.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 24 | 0.5 | SMG (+1B), Viral Mine, Viral Pistol, Shock CCW; **Minelayer**, Decoy; non-FTO |
| 2 | 21 | 0 | **FTO**; SMG, Viral Mine, Viral Pistol, Shock CCW; **Minelayer** |

### S.T.R.S. Tanuki Team

**Unit ID:** 1819 · **Slug:** `s-t-r-s-tanuki-team` · **AVA:** 5 · **MI / Veteran / Regular**  
`MOV 10-10 | CC 17 | BS 13 | PH 11 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. Warhorse, Number 2, Immunity (Shock), Terrain (Total).

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 18 | 0 | Boarding Shotgun, Chain-colt, Flash Pulse, Pistol, CCW; **Chain of Command** |
| 2 | 19 | 0 | MULTI Rifle, D-Charges, Pistol, CCW; **Engineer**, Deactivator, GizmoKit |
| 3 | 20 | 0.5 | SMG, Pitcher, Disco Baller, Pistol, CCW; **Hacking Device** |
| 4 | 20 | 0 | Boarding Shotgun, Contender, Pistol, CCW; **Paramedic, MediKit** |
| 5 | 29 | 1.5 | HMG, Pistol, CCW; **MSV2** |
| 6 | 27 | 1.5 | MULTI Sniper Rifle, Pistol, CCW; **MSV2** |
| 7 | 29 | 1 | HMG, Pistol, CCW; **MSV2, Lieutenant** |

### Yáopú Pangguling

**Unit ID:** 162 · **Slug:** `yaopu-pangguling` · **AVA:** 1 · **REM / Support / Regular**  
`MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 2 | BTS 3 | STR 1 | S 4`. Baggage, Remote Presence, Courage.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 8 | 0 | PARA CCW (-3); **Repeater, Deactivator** |
| 2 | 14 | 0.5 | PARA CCW (-3); **EVO Hacking Device** |
| 3 | 17 | 0 | Combi Rifle, PARA CCW (-3); **Repeater, Total Reaction** |
| 4 | 12 | 0 | **FTO label in profile**; Light Shotgun, PARA CCW (-3); Repeater |

**Important:** the current Shindenbutai Fireteam chart does not include Pangguling. Its FTO profile label alone does not create Fireteam access here.

### Kyojin Killers

**Unit ID:** 1827 · **Slug:** `kyojin-killers` · **AVA:** 2 · **SK / Spec. Trained / Irregular**  
`MOV 10-10 | CC 21 | BS 11 | PH 13 | WIP 12 | ARM 0 | BTS 0 | W 1 | S 2`. Forward Deployment (+20), Mimetism (-3), Surprise Attack (-3), Stealth, Super-Jump, Religious Troop.

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 18 | 0 | Light Flamethrower, Contender, Pistol, DA CCW |
| 2 | 15 | 0 | Heavy Flamethrower, Flammenspeer, Pistol, DA CCW |

### Yáozăo

**Unit ID:** 161 · **Slug:** `yaozao` · **AVA:** 3 · **REM / Support / Peripheral**  
`MOV 15-10 | CC 11 | BS 8 | PH 10 | WIP 13 | ARM 0 | BTS 3 | STR 1 | S 1`. Peripheral (Servant), Mimetism (-3), Courage.

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 3 | 0 | PARA CCW (-3); Servant |

### Raiden Seibutai

**Unit ID:** 167 · **Slug:** `raiden-seibutai` · **AVA:** 3 · **MI / Elite / Regular**  
`MOV 10-10 | CC 16 | BS 13 | PH 11 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`. X-Visor; Hidden Deployment, Minelayer, Mimetism (-3), Surprise Attack (-3), Immunity (Shock), Courage.

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 2 | 25 | 1.5 | Heavy Rocket Launcher, Shock Mine, Breaker Pistol, CCW |
| 3 | 33 | 2 | Missile Launcher, Shock Mine, Breaker Pistol, CCW |

### Ninjas

**Unit ID:** 135 · **Slug:** `ninjas` · **AVA:** 1 · **SK / Spec. Trained / Regular**  
`MOV 10-10 | CC 23 | BS 11 | PH 12 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Martial Arts L3, Camouflage, Hidden Deployment, Infiltration, Mimetism (-6), Surprise Attack (-3), Stealth, Climbing Plus.

| Profile ID | Pts | SWC | Loadout / flags |
|---:|---:|---:|---|
| 1 | 24 | 0 | Tactical Bow (+1SD), Shock Mine, Pistol, DA CCW |
| 4 | 27 | 0 | SMG, Pistol, DA CCW |
| 5 | 31 | 1.5 | MULTI Sniper Rifle, Pistol, DA CCW |
| 6 | 33 | 0.5 | SMG, Pistol, DA CCW; **Hacking Device** |
| 7 | 26 | 0 | Tactical Bow (+1SD), Shock Mine, Pistol, DA CCW; **KHD** |
| 9 | 30 | 0.5 | Boarding Shotgun, Flash Pulse, Pistol, DA CCW; **FO** |

### Sāchā, Xenotech Hunters

**Unit ID:** 1874 · **Slug:** `sacha-xenotech-hunters` · **AVA:** 1 · **LI / Mercenary / Irregular**  
`MOV 10-10 | CC 17 | BS 11 | PH 12 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 2`. Forward Deployment (+10), Booty, Specialist Operative, Climbing Plus, Terrain.

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 6 | 0 | Flash Pulse, E/M Grenades (+1B), Stun Pistol (+1B), CCW |

### Ioann Bann, Varangian Dog-Warrior

**Unit ID:** 1940 · **Slug:** `ioann-bann-varangian-dog-warrior` · **AVA:** 1 · **WB / Character / Irregular**

| State | MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Dogface | 15-10 | 22 | 11 | 14 | 13 | 2 | 3 | 3 | 2 |
| Dog-Warrior | 15-10 | 23 | 11 | 16 | 13 | 4 | 6 | 3 | 6 |

Martial Arts L3, Berserk, Super-Jump and transformation-related rules as encoded by source.

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 2 | 30 | 0 | Chain Rifle (+1B), Viral Tactical Bow (+1SD), Grenades, AP Heavy Pistol (+1B), AP+T2 CCW |

### Kazurabā Ruby Monday

**Unit ID:** 1890 · **Slug:** `kazuraba-ruby-monday` · **AVA:** 1 · **HI / Character / Irregular**  
`MOV 15-5 | CC 18 | BS 12 | PH 12 | WIP 13 | ARM 3 | BTS 6 | STR 2 | S 2`. Hackable; Technorganic, Specialist Operative, Climbing Plus, Terrain, Immunity (IMM-B).

| Profile ID | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 19 | 0 | Adhesive Launcher Rifle, Flash Pulse, E/M Grenades, Stun Pistol, CCW |

## Lieutenant and order-control index

| Unit/profile | Function |
|---|---|
| Senku profile 8 | cheap Lieutenant, 9 pts / 0.5 SWC |
| Mechazoid profile 3 | TAG Lieutenant plus Tactical Awareness, 69/1.5 |
| Hatamoto profiles 4–6 | Lieutenant **+1 Order**, **+1 SWC rebate**, and NCO; 36–39 pts |
| Metsuke profile 1 | Lieutenant + Strategos L1, 22/0 |
| Metsuke profile 2 | Lieutenant +1 Order, 23/0 |
| Tanuki profile 7 | HMG MSV2 Lieutenant, 29/1 |
| Tanuki profile 1 | Chain of Command |
| Hatamoto | NCO on every current profile |
| Mechazoid | Tactical Awareness on every current profile |
| Triphammer | Tactical Awareness on every current profile |
| Metsuke | Counterintelligence on chassis |

## Hacking and network index

### Hackers

- **Hacking Device:** Kurayami profile 2; Teishin profile 2; Tanuki profile 3; Ninja profile 6.
- **Killer Hacking Device:** Nokizaru profile 2; Teishin profile 3; Ninja profile 7.
- **EVO Hacking Device:** Pangguling profile 2.

### Network / projection

- **Pitcher:** Tanuki Hacker.
- **Repeaters:** Robio; Atom; Pangguling profiles 1, 3 and 4.
- **Sensor:** Atom profile 1.
- **Disco Baller:** Tanuki Hacker.
- **Guided weapon:** Uran Missile Launcher chassis is explicitly BS Attack (Guided).
- Shindenbutai does **not** have a broad Pitcher-heavy network: its main network is a small number of Repeaters plus the Tanuki Pitcher.

## Deployment / marker-state index

- **Combat Jump / Parachutist:** Teishin Guntai.
- **Hidden Deployment:** Kurayami Ninjas; Ninjas; Raiden.
- **Camouflage / marker pressure:** Yamabushi non-FTO profiles; Ninjas; Kurayami; Saito; Kyojin source package; Aïda solo profile via forward/minelayer tools.
- **Infiltration:** Kurayami, Ninjas, Saito.
- **Forward Deployment:** Yamabushi; Aïda; Sāchā; Yuriko non-FTO profile.
- **Holoprojector / Holomask:** Lù Duān; Metsuke; Shurayuki.

## Vision-control and sensor index

- **Smoke:** Yojimbo (both identities); Saito Togan; Garon profile 3 has Smoke Grenade Launcher; Ioann Bann's current source package provides aggressive visibility control through its warband kit.
- **MSV2:** Rui Shi profile 1; Tanuki HMG/sniper/Lt profiles.
- **MSV1:** Nokizaru; Rui Shi profile 2; Lù Duān.
- **Sensor:** Atom profile 1.

## Canonical Fireteam definitions

Current chart limit: **1 Core, 1 Haris, unlimited Duos** (`DUO: 256` source sentinel).

### FT-01 — Senku Fireteams

**Types:** Haris, Core  
**Anchor:** Senku has source `min: 1`; no row has `required: true`.

| Member | Unit ID | Required | Min | Max | Counts as / comment | Profile restriction |
|---|---:|---|---:|---:|---|---|
| Senku | 1817 | no | 1 | 5 | — | all |
| Jizamurai | 1821 | no | 0 | 2 | — | all |
| Hatamoto | 1823 | no | 0 | 1 | — | all |
| Taguraidā | 1828 | no | 0 | 1 | — | all |
| Kaizoku Spec-Ops | 1924 | no | 0 | 1 | `Spec-Ops` | optional mode only |

### FT-02 — Bushi-tai Fireteams

**Types:** Duo, Haris, Core  
**Anchor:** Jizamurai has source `min: 1`.

| Member | Unit ID | Required | Min | Max | Counts as / comment | Profile restriction |
|---|---:|---|---:|---:|---|---|
| Jizamurai | 1821 | no | 1 | 5 | `(Bushi-tai)` | all |
| Hatamoto | 1823 | no | 0 | 2 | `(Bushi-tai)` | all |
| Shizoku | 1822 | no | 0 | 1 | `(Bushi-tai)` | **FTO profiles 1–2 only** |
| Yamabushi | 1824 | no | 0 | 1 | — | **FTO profiles 1–2 only** |

### FT-03 — Sayō (Action) Fireteams

**Types:** Duo, Haris

The source marks **Tanuki `required: true` while leaving its raw `min` at `0`**. Preserve both facts: the required-member semantic is authoritative and must not be discarded merely because the numeric minimum is zero.

| Member | Unit ID | Required | Min | Max | Counts as / comment | Profile restriction |
|---|---:|---|---:|---:|---|---|
| Tanuki | 1819 | **yes** | 0 | 3 | `(Sayó)` | all |
| Jizamurai | 1821 | no | 0 | 2 | — | all |
| Yamabushi | 1824 | no | 0 | 1 | `(Sayó)` | **FTO profiles 1–2 only** |
| Rui Shi | 159 | no | 0 | 1 | `(Sayó)` | all current profiles |
| Shizoku | 1822 | no | 0 | 1 | `(Strategic Deployment)` | **profile 3 only** |
| Aïda Swanson | 1160 | no | 0 | 1 | `FTO` | **profile 2 only** |
| Ioann Bann | 1940 | no | 0 | 1 | — | all |

### FT-04 — Yamabushi Fireteams

**Type:** Duo

| Member | Unit ID | Required | Min | Max | Counts as / comment | Profile restriction |
|---|---:|---|---:|---:|---|---|
| Yamabushi | 1824 | no | 1 | 2 | — | **FTO profiles 1–2 only** |
| Ioann Bann | 1940 | no | 0 | 1 | `(Yamabushi)` | all |

### FT-05 — Mechazoid Fireteams

**Type:** Duo

| Member | Unit ID | Required | Min | Max | Counts as / comment | Profile restriction |
|---|---:|---|---:|---:|---|---|
| Mechazoid | 1788 | no | 1 | 2 | — | all |
| Tanuki | 1819 | no | 0 | 1 | — | all |
| Atom Aibōt | 1830 | no | 0 | 1 | — | all |

### Wildcards

| Unit | Unit ID | Counts as | Profile restriction | Notes |
|---|---:|---|---|---|
| Shurayuki | 1829 | `(Senku)` | all | explicit Wildcard row |
| Yuriko Oda | 1019 | `(Senku, Sayō)` | **FTO profiles 1–2 only** | explicit Wildcard row |

Do not import additional Wildcards or Fireteam permissions from vanilla JSA, Ōban, older editions, or another JSA sectorial.

## Unit → Fireteam access index

| Unit | Fireteam | Types | Access | Profile restriction | Min–max / notes |
|---|---|---|---|---|---|
| Senku | FT-01 | Haris/Core | native anchor | all | 1–5 |
| Jizamurai | FT-01 | Haris/Core | native | all | 0–2 |
| Hatamoto | FT-01 | Haris/Core | native | all | 0–1 |
| Taguraidā | FT-01 | Haris/Core | native | all | 0–1 |
| Kaizoku Spec-Ops | FT-01 | Haris/Core | optional | Spec-Ops mode | 0–1 |
| Jizamurai | FT-02 | Duo/Haris/Core | Bushi-tai anchor | all | 1–5 |
| Hatamoto | FT-02 | Duo/Haris/Core | counts-as Bushi-tai | all | 0–2 |
| Shizoku | FT-02 | Duo/Haris/Core | counts-as Bushi-tai | FTO 1–2 | 0–1 |
| Yamabushi | FT-02 | Duo/Haris/Core | native | FTO 1–2 | 0–1 |
| Tanuki | FT-03 | Duo/Haris | **required Sayō** | all | max 3 |
| Jizamurai | FT-03 | Duo/Haris | native | all | 0–2 |
| Yamabushi | FT-03 | Duo/Haris | counts-as Sayō | FTO 1–2 | 0–1 |
| Rui Shi | FT-03 | Duo/Haris | counts-as Sayō | all | 0–1 |
| Shizoku | FT-03 | Duo/Haris | Strategic Deployment member | **profile 3** | 0–1 |
| Aïda | FT-03 | Duo/Haris | FTO member | **profile 2** | 0–1 |
| Ioann Bann | FT-03 | Duo/Haris | native | all | 0–1 |
| Yamabushi | FT-04 | Duo | native anchor | FTO 1–2 | 1–2 |
| Ioann Bann | FT-04 | Duo | counts-as Yamabushi | all | 0–1 |
| Mechazoid | FT-05 | Duo | native anchor | all | 1–2 |
| Tanuki | FT-05 | Duo | native | all | 0–1 |
| Atom | FT-05 | Duo | native | all | 0–1 |
| Shurayuki | Wildcard | permitted teams | Wildcard counts-as Senku | all | max 1 |
| Yuriko Oda | Wildcard | permitted teams | Wildcard counts-as Senku/Sayō | FTO 1–2 | max 1 |

If this reverse index ever conflicts with the canonical Fireteam tables above, the canonical tables win.

## Optional-mode units

| Unit | ID | Mode | Normal Shindenbutai status |
|---|---:|---|---|
| Kaizoku Spec-Ops | 1924 | Spec-Ops | Optional only; may join FT-01 when the mode is enabled |
| JSA Team-Ops | 1938 | Team-Ops | Optional only |

Do not count either entry as an ordinary matched-play roster selection unless the corresponding optional mode is enabled.

## Character/relation constraints

The current source contains explicit relationship groups that must be preserved:

- Main **Yuriko Oda** (ID `1019`) is linked to source identity `1799` with `max: 1`. This prevents taking duplicate linked Yuriko identities across the relevant Main/Reinforcement construction.
- **Motorized Yojimbo** (ID `224`) and **Yojimbo, Sword for Hire** (ID `1834`) are in the same `max: 1` relation group together with linked identities `10224` and `11834`. Only one Yojimbo identity may be selected.

These restrictions are character-identity constraints, not AVA increases.

## Reinforcements boundary

Army links Shindenbutai to Reinforcement roster ID **1199**. Reinforcement-only profiles, AVA and Fireteam permissions remain outside this Main reference. Do not merge Reinforcement Fireteam permissions into the Main chart above.

The source relation hooks for Yuriko and Yojimbo continue across linked identities, so the Reinforcement boundary does not permit duplicate versions of those characters.

## Derived tactical index

This section is analytical and non-authoritative; the source profile data and Fireteam chart above take precedence.

| Block / tag | Strong Shindenbutai candidates |
|---|---|
| Long-range attack | Mechazoid AP HMG/MULTI Spitfire; Shizoku AP HMG; Tanuki HMG MSV2; Hatamoto Red Fury/Spitfire; Rui Shi |
| Long-range ARO | Raiden HRL/ML; Tanuki MULTI Sniper MSV2; Uran Missile Launcher; Garon TR HMG; Shizoku HRL |
| Mid-range attack | Hatamoto; Jizamurai; Shizoku; Tanuki; Lù Duān; Rui Shi |
| Close assault | Shurayuki; Saito; Yojimbo; Yamabushi; Jizamurai; Kyojin; Ioann Bann; Kurayami/Ninja |
| Specialist | Tokusetsu; Senku FO/Paramedic/Commlink; Nokizaru; Kurayami Hacker; Hatamoto; Metsuke; Monstrucker; Teishin; Taguraidā; Tanuki; Atom; Yuriko; Sāchā; Ruby Monday |
| Cheerleader / cheap orders | Senku; Robio; Warcor; Pangguling |
| TAG + support | Mechazoid or Triphammer + Tokusetsu/Monstrucker/Taguraidā/Yáozăo |
| REM + support | Rui Shi/Lù Duān/Garon/Uran/Atom/Robio/Pangguling + Tokusetsu/Monstrucker |
| DZ defense | Raiden; Garon; Uran; Tanuki sniper; Warcor; Pangguling TR |
| Midfield defense | Kurayami; Ninjas; Saito; camo Yamabushi; Kyojin; Aïda |
| Midfield specialist | Nokizaru FO/KHD; Ninja FO/Hacker; Kurayami Hacker; Sāchā; Yuriko |
| Warband | Yojimbo; Yamabushi; Ioann Bann; Kyojin |
| Airborne troops | Teishin Guntai |
| Enemy-DZ attacker | Teishin; Saito; Ninja/Kurayami; fast Yojimbo/Ioann pressure |
| Network projection | Tanuki Pitcher; Robio/Atom/Pangguling Repeaters |
| Vision control | Yojimbo/Saito smoke; Garon Smoke Grenade Launcher; MSV2 Tanuki/Rui Shi exploit smoke |
| Hacker | Kurayami; Teishin HD; Tanuki HD; Ninja HD |
| KHD | Nokizaru; Teishin KHD; Ninja KHD |
| Tech-counter | Atom Sensor; Tokusetsu/Monstrucker/Tanuki Engineers; Yáozăo servant support |
| Group-2 efficient | Warcor; Robio; Pangguling EVO; Garon/ARO pieces; Teishin waiting for an airborne run; Irregular Sāchā |

## Source-normalization and validation notes

- Standard roster count is **36 normal entries + 2 optional-mode entries**.
- Generic `merc-*` catalogue objects with empty `factions` arrays are excluded even though the aggregate dataset contains them. Explicit faction-`1102` mercenary/guest entries are retained.
- Source `DUO: 256` is normalized as effectively unlimited Duos.
- Senku and Jizamurai anchors use positive source `min` values despite `required: false`; those minimums are preserved.
- Sayō Tanuki has the inverse-looking source representation: `required: true` with `min: 0`. Both values are preserved; the required semantic is not erased.
- `Shizoku FTO` in Bushi-tai means profiles **1–2 only**. The Sayō `SHIZOKU (Strategic Deployment)` row maps to **profile 3 only**.
- `Yamabushi FTO` means profiles **1–2 only**.
- Sayō `AÏDA SWANSON` with comment `FTO` means **Aïda profile 2 only**.
- Wildcard `YURIKO ODA FTO` means **Yuriko profiles 1–2 only**.
- Pangguling profile 4 is labelled FTO in its unit data but the current Shindenbutai chart has no Pangguling row; no Fireteam access is inferred.
- Disabled Kobaruto/TurtleMek subordinate entries are not counted as independent roster selections.
- Main and Reinforcement roster `1199` remain separate except that source character-relation constraints still prevent duplicate identities.

## Provenance

- Sectorial ID: `1102`
- Parent faction: JSA (`1101`)
- Corvus Belli Army-derived revision: `7.26246.159`
- Source commit: `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b` (`army: N5.3 + ITS18`)
- Army data changed on: 2026-09-03
- Versioned source: `n5/shindenbutai/7.26246.159.json`
- Versioned source blob: `3b48c5df4a55cb9cb54bf1053e00e77e939cf12b`
- Aggregate source: `n5/shindenbutai/shindenbutai.json`
- Aggregate source blob at pinned commit: `75662995dc103c81c41a2d076bea0ef89b2c6e1d`
- InfinityDB commit: `4e2662be3f43387fbae42b3790a711b3e98570c4`
- Rules baseline: N5.3 + N5 FAQ v0.1
- Generated / verified: 2026-10-16
