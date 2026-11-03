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

**Faction pick/avoid research (23 Oct 2026):** [Transcript-backed three-JSA-sectorial must-have, go-to and avoid comparison](#must-have--go-to--avoid--source-backed-recommendations-2026). Opinions are tactical evidence, not alterations to the canonical roster and Fireteam rules.


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
`MOV 10-10 | CC 21 | BS 11 | PH 13 | WIP 12 | ARM 0 | BTS 0 | W 1 | S 2`. CC Attack (+1B), Camouflage (1 Use), Forward Deployment (+20), Mimetism (-3), Surprise Attack (-3), Stealth, Super-Jump, Terrain (Total), Religious Troop.

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

## Mission specialist choices — N5.3 cross-game evaluation

**Ninja KHD/FO**, fast Aragoto-style specialist or **Shikami SO** only where they are **actually listed** in Shindenbutai, may win hidden/late objective access. Its own **Shindenbutai Fireteam chart and profile roster**, not Vanilla JSA's, determines scoring toolkits and whether a specialist moves with the attack team. Favor 2–3 geographically separated mission routes and avoid buying an expensive combat unit only because a same-name Vanilla profile is a Specialist.

See [Mission Specialists / Button Pushers apex and value tiers](../../notes/list-building/mission-specialists-and-button-pushers-apex-value.md). This roster and its Fireteam chart are the final authority for exact options.

## N5.3 airborne / backline-strike archetypes and trades (2026-10-23)

**Teishin BSG19/0, KHD21/0, FO19/0** combines cheap **Combat Jump/normal Parachutist** with scoring/anti-hacker utility, not guaranteed enemy-DZ access. **Ninja/Kurayami hidden/infiltrating** troops attack from set-up midfield approaches; deep enemy-half Infiltration costs a PH−3 roll and failure reveals at own DZ edge. **Do not import Shinobu/Vanilla Oniwaban** if this Shindenbutai roster does not list them. **Shindenbutai's own Fireteam required-choice constraints** still apply; off-table AD troops do not get automatic pooled Orders.

[Full N5.3 apex/value and delivery-probability tier guide](../../notes/list-building/airborne-and-enemy-dz-attackers-apex-value.md). Current roster/profile restrictions and canonical Fireteam chart above govern legal choices.

## Active-turn gunfighter cross-reference (2026-10-23)

**Active-turn shooting choices:** **Hatamoto Plasma Carbine34/0** is the **non-TAG** Mimetism(-3)/Nanoscreen, Specialist Operative + strong CC **short-range** attack with 0 SWC cost; **Red Fury40/1** buys more open midfield Burst, **Spitfire41/1.5** a stronger sustained near-mid lane. Don't rate the 34pt Plasma Carbine as a long HMG: its value is angle/movement, survivability and mission actions. **O-Yoroi** is an entirely separate TAG long-range investment wherever rostered, not the same category of active gun. [Non-TAG and TAG value analysis](../../notes/list-building/active-turn-gunfighters-apex-and-value.md).

## Warband cheap trading / order economy — N5.3

**Ioann Bann30/0** (not Tohaa/Starmada 32pt loadout) is a high-end **Irregular multi-Wound dog-warrior** using Chain(+1B), Viral Tactical Bow(+1SD), Grenades and AP+T2 CC; **this Shinden printed option lacks Smoke**, so don't import the 32pt counterpart's Smoke Grenades. **Teishin BSG19/0 and Ninja/Kurayami concealed** are alternative flank/hidden attacks, not cheap Impetuous warbands. A 30pt Ioann should ideally survive multiple attacks/contest a lane rather than die for a single 10pt kill; **do not import Ōban Yuan Yuan if Shinden roster lacks them**.

[Current cross-faction warband apex/value, opponent counters, Lt/CoC packages](../../notes/list-building/warbands-and-cheap-trading-units-apex-value.md). This faction's own pinned profile and Fireteam rows control legality.

## TAG tactical cross-reference (2026-10-23)

**Mechazoid** is the native TacAware TAG with a potential legal Duo to reinforce JSA's midrange shooting; **Triphammer (48–53 in other current rosters; check this file for exact options)** is the cheaper mercenary with flexible AP Spitfire/HRL and a swingy damaged state. Mechazoid for mission/team integration, Triphammer when the saved points buy a real specialist or independent attacker.

Across all factions, compare **apex power** separately from **points value**, counterplay and mission fit: [N5.3 TAG guide](../../notes/list-building/tags.md). The current unit profiles and canonical Fireteam chart above take precedence over tactical opinions.

## Hacker and KHD tactical cross-reference (2026-10-23)

**Tanuki HD+Pitcher+Disco Baller 20/0.5** is a particularly efficient network **and visibility** extender; **Nokizaru KHD27/0** supplies stealthy field cyber assassination, **Ninja KHD26/0** protected mission access. **Teishin Combat Jump KHD21/0 vs HD23/0.5** is a low-cost airborne scoring/Trinity or anti-HI alternative; **Kurayami HD26/0.5** handles forward Oblivion/Carbonite; **Pangguling EVO14/0.5** merits consideration only if its REM/Combat Jump support programs actually help several units. **Why:** a cheap Tanuki can create a real Repeater net for KHD defense, whereas three independent hidden KHDs without HD/White Noise do not automatically control TAGs.

See the [cross-game apex/value Hacker/KHD tier guide](../../notes/list-building/hackers-and-killer-hackers.md). **The sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative; device upgrades are profile-specific.**


## Cheerleader / Order-generation tactical cross-reference (2026-10-23)

See the N5.3 [cross-game apex/value rankings and transcript-backed competing assessments](../../notes/list-building/cheerleaders-and-order-generators.md). The current roster and official Fireteam definitions above remain authoritative; unit access/cost may differ from vanilla.

- Yuriko/Engineer — buy for recovery and mission support, not cheap generic Order generation.
- 3pt Warcor — very useful Irregular Flash ARO/cheap screen, NOT an ordinary transferable Order.

**Selection rule:** Count deployed, transferable Regular Orders per Combat Group, not total models or restricted bonus Orders; choose the lowest-cost protected Regular profile that *also* contributes a relevant Repeater, Baggage, Fireteam, template, ARO or Specialist job. Check Group slots and DZ hiding space before buying a third large-base REM or replacing a needed scoring piece.


## ARO apex/value cross-reference (2026-10-23)

[Best ARO units across N5.3 — absolute apex vs points-value](../../notes/list-building/aro-units-apex-and-value.md) compares hidden reactive fire, TR/Neurocinetics, Flash/DTW/expendable defenders and why competing creators disagree. The **roster here** is authoritative for actual costs, Training, AVA and Fireteam construction.

- **Garon TR** — 16pt/0SWC Thunderbolt/smoke option shifts from passive guard to active smoke enablement where legal
- **Raiden HRL/ML** — concealed surprise launcher + mine, high ambush ceiling; the ML can cost 2SWC, so choose the defended scoring lane carefully
- **Warcor 3pt Flash** — disposable Irregular Stun/Orders tax, not a generic Regular cheerleader
- **Total Reaction support** — use recoverable remote for routine lanes, rather than expose primary active gun

**Best circumstance:** long exposed lanes justify a real sniper/missile/linked gun; dense tables, DZ landings and mission rooms favor E/M, mine, Shotgun, Riotstopper and hidden traps. Cover the destination/approach, layer serial threats rather than two pie-sliceable visible guns, and preserve scoring units for the active turn.

## Doctor / Engineer / Recovery cross-reference (2026-10-23)

**Tokusetsu14 Doctor versus Engineer** are distinct 65%-base medical/technical roles; **Yáozăo3** cuts the travel cost to the likely casualty. **Yuriko Oda25 Engineer** adds Mimetism, Minelayer and forward technical support, whereas **Monstrucker12** gives cheap Irregular Engineering. When **Hatamoto** pushes far beyond the support network, the theoretical 65% revival chance may never be usable. [Recovery support tiers, probabilities and transcript disputes](../../notes/list-building/doctors-engineers-and-recovery-apex-value.md).

## Close-combat assassins and counter-CC — N5.3 (2026-10-23)

**Hatamoto Plasma34/0 (MA4, NBW, Monofilament/E/M, 2W, Specialist)** is the roster's all-round CC counter-duelist while advancing in support of the gun; **34pt is not a Hidden/Infiltrating assassin** and must choose which attack role to solve. **Teishin19 Combat Jump** is a flank **shotgun** attacker, merely MA1/CC21, not equivalent to an Oniwaban. Use the legal midfield/Smoke and ranged covering unit before risking a costly HI in CC; consider enemy Guard and NBW. [Cross-game CC assassin apex/value, Guard and delivery disputes](../../notes/list-building/dedicated-close-combat-assassins-apex-value.md).

## N5.3 network projection — Pitchers, Repeaters, TinBots and disposable delivery

**Tanuki Hacking Device+Pitcher+Disco Baller20/.5** gives **BS13 ranged Repeater and vision control on one Regular Warhorse MI**, very strong economy if its **legal team** can add applicable bonuses. **Robio7/0 native Repeater/Flash**, **Atom Sensor/FO/native Repeater**, and **Pangguling8/0 Baggage/Repeater** cover cheap mobile network and reload. **Pangguling FTO12/0** is a *different* profile; source team-chart legality still required. **Opposing case:** JSA's powerful camo/assassins can dominate non-Hackable tables; avoid paying for more network unless a standard HD is present to actually exploit the position.

[Whole-game apex/value network guide, current profiles, and opposing media views](../../notes/list-building/network-projection-repeaters-pitchers-apex-value.md).

## Anti-TAG / Anti-HI without hacking — N5.3 (2026-10-23)

**Yamabushi15 Panzerfaust FTO /16 Camo(1 use)** gives inexpensive AP+EXP deterrence; **Yuriko Oda FTO23 Panzerfaust or 25 E/Mitter** adds technical mission roles. **Lù Duān20 E/M Carbine+E/M Mine** can disable heavily armored victim without entering CC; **Hatamoto34 Plasma+Monofilament/E/M CCW** is 2W mobile finisher; **Shizoku43 AP HMG** is the sustained ranged kill plan. **Triphammer48 TAG Panzerfaust(+1B)** and Mechazoid are higher cost categories; not a free value substitute. [Cross-game non-hacking anti-armor apex/value guide](../../notes/list-building/anti-tag-anti-heavy-infantry-non-hacking-apex-value.md).

## Tactical cross-reference — indirect fire (2026-10-23)

**Uran Guided Missile16/1.5** is an *optional* payoff for **Tanuki HD Pitcher20/.5 + Robio/Atom/Pangguling Repeater/FO**, not Shinden's mandatory primary long gun. Shepherd prefers a direct **Trinity attack on enemy Hacker** to Guided in many early Network windows; a Uran already positioned in Group 2 can still punish Targeted/Spotlight ARO. The **Garon Smoke GL16/0** is visibility control, not a high-damage speculative grenade. [Whole-game decision guide](../../notes/list-building/indirect-fire-speculative-guided-apex-value.md).

## N5.3 objective holding, zone domination & carried-objective choices

**Hatamoto Specialist+Nanoscreen+NCO34/0** is a durable-but-mobile W2 carrier that also protects himself in CC; can use NCO Orders, not an automatic extra Regular Order. **Karakuri is not imported from Ōban just because JSA has it**; exact Shindenbutai roster lacks it. Choose available **Tanuki20/.5 Hacker+Pitcher+Disco**, **Yukina/Yūgao/other roster-legitimate specialists** for position, with cheap 7pt Robio Repeater and defensive traps rather than imagining a Karakuri wall. **Counter:** a 34pt Hatamoto in full view of multiple guns is less safe than a 20pt specialist behind terrain.

[Cross-game zone-holder and carrier apex/value guide, rules, and transcript disagreements](../../notes/list-building/objective-holding-zone-domination-and-carriers-apex-value.md). Source roster/FT chart above wins over tactical comparisons.

## Anti-Tech — enemy visors, Mimetism, markers and Impersonation (2026-10-23)

**Atom Aibōt FO/Sensor15/0** is the *cheap* Hidden/Camo counter rather than sending a pricey Mechazoid into speculative Discover. **Tanuki HD + Disco20/.5** bypasses opposing MSV/Marksmanship using Eclipse-style placement; do not call a Tanuki hacker White Noise HD+ without verifying its printed device. **Tanuki MSV2 HMG29/1.5 or MSR27/1.5** and **Rui Shi MSV2 Spitfire23/1** are direct guns against revealed Mimetism; these are not the 20pt Disco loadout. **Choose:** Sensor for many markers, Disco for a defended lane, MSV2 gun for an ARO that must be killed. Count Fireteam and ammo restrictions.

[Anti-tech N5.3 whole-game apex/value and counter-matchups](../../notes/list-building/anti-tech-msv-mimetism-camo-impersonation-apex-value.md).

## Force multipliers — N5.3 role/value cross-reference (2026-10-23)

**Metsuke LT Strategos1/Counterintel22/0** is a cost-efficient command shell; **LT(+1 Order)23/0** is alternative, not combined. **Shizoku HRL(+1B) Strategic Deployment38/1.5** applies FD(+4″) to a **legal Sayō** team only; Yamabushi's individual FD **doesn't trigger +8″**. **Taguraidā Mechazoid Pilot12/0 TAGCom** benefits same-group TAG only per bracketed Dodge/GizmoKit MODs. **Pangguling8 Baggage/Repeater vs14/.5 EVO** supports Rui Shi/Dispensers/airborne when effect actually activates. [Whole-game guide](../../notes/list-building/force-multipliers-special-abilities-apex-value.md).

## Battle-report effectiveness and combinations (qualitative, 2026-11-01)

**Observed recurring combination:** **Hatamoto Lieutenant extra Orders + NCO attack lane**, **Shizoku rocket team + Yamabushi Paramedic/specialist**, **Tanuki gun/hacker**, and **Yojimbo smoke/flank** create both killing and actual objective conversions. #224 records Hatamoto breaking a Tohaa carried-objective defense; #228 a **Yamabushi Paramedic** scored the final beacon action to secure a **3–3** despite other combat losses; #233 used Shizoku/Yojimbo pressure to open The Dig tasks. [#224, #228](../../notes/battle-reports/221-230-n5-battle-report-tactical-analysis.md) · [#233](../../notes/battle-reports/231-240-n5-battle-report-tactical-analysis.md).

**Counters and confidence:** #056's **Tunguska Pitcher/Spotlight/Guided/Oblivion** repeatedly disrupted an elite Hatamoto-linked approach: invest in repeater clearance or independent nonhackable specialists. #233's **9–1 is projected after play stopped**, not a finalized result. The #224 player's proposed **MSV2 Tanuki / second Yamabushi** substitutions are opinions, not pieces proved in that game. Confirm current **Sayō/team composition and profile eligibility** in canonical Fireteams before copying historical Shizoku links.

[Cross-report synthesis and evidence cautions](../../notes/battle-reports/cross-report-unit-effectiveness-and-combinations.md).

## Mission performance — battle-report evidence (2026-11-01)

| Mission(s) | Tested composition / scoring mechanism | Evidence |
|---|---|---|
| **Critical Intervention defensive objective room** | Hatamoto Lieutenant/NCO, Shizoku launcher/Yamabushi, Tanuki and Yojimbo controlled carrier exit; Hatamoto removed final Tohaa package carrier. | [#224](../../notes/battle-reports/221-230-n5-battle-report-tactical-analysis.md) |
| **B-Pong / beacon last-turn** | Yamabushi Paramedic finished beacon WIP and altered last-turn score to 3–3 despite Morat attacking guns. | [#228](../../notes/battle-reports/221-230-n5-battle-report-tactical-analysis.md) |
| **The Dig** | Shizoku rocket + Yamabushi and Yojimbo smoke removed defenders and reached hyperthermal tasks; 9–1 **projected after early stop**, not finalized. | [#233](../../notes/battle-reports/231-240-n5-battle-report-tactical-analysis.md) |
| **Hardlock vs Ōban** | Double Hatamoto/Raiden pressure defeated Ōban's skirmishers in a tournament recap, exact score unverified. | [#236](../../notes/battle-reports/231-240-n5-battle-report-tactical-analysis.md) |

**Limits:** Elite Hatamoto team remains hackable (#056); verify current Shizoku team membership and mission packet. Game-era qualitative evidence, not a win-rate or current Fireteam claim. [Full mission evidence audit](../../notes/battle-reports/cross-report-mission-performance-by-sectorial.md).

## Counterplay — observed N5 battle-report responses (2026-11-02)

| Threat / target | Observed response and limitation | Battle reports |
|---|---|---|
| **Vs Tohaa room and E/M** | Hatamoto NCO/Lt + Shizoku HRL + Tanuki hacker/Pitcher and expendable Yojimbo Koalas attacked Sukeul/Makaul/Kriigel fortress; Hatamoto removed last data carrier. | [#224](../../notes/battle-reports/221-230-n5-battle-report-tactical-analysis.md) |
| **Vs sniper Fireteam** | Yojimbo Smoke + Shizoku + Yamabushi Paramedic cleared Torchlight Vidoc/Moonraker early in The Dig; reported 9–1 **projected** after stop. | [#233](../../notes/battle-reports/231-240-n5-battle-report-tactical-analysis.md) |
| **Counter-counterplay: hacking** | Tunguska Pitcher/Spotlight/Guided/Oblivion made Hatamoto HI spend Orders Resetting; do not march linked elite through exposed Repeaters without engineering/backup scorer. | [#056](../../notes/battle-reports/051-060-n5-battle-report-tactical-analysis.md) |
| **Hidden strike** | Raiden HRL and hidden Oniwaban/Killer/Koala traps can force additional Discover/short-range attack before opponent reaches WIP specialists. | [#220](../../notes/battle-reports/211-220-n5-battle-report-tactical-analysis.md), [#224](../../notes/battle-reports/221-230-n5-battle-report-tactical-analysis.md) |

**Limit:** The double-Hatamoto or Shizoku historic Fireteam is not automatically legal today; avoid claiming #233 final win. These are historical qualitative interactions, not current N5.3 profile/Fireteam or faction win-rate claims. [Full cross-report counterplay analysis](../../notes/battle-reports/n5-cross-report-counterplay-tags-hi-hacking-camo-impersonators-fireteams.md).

---

## Must-have / Go-to / Avoid — source-backed recommendations (2026)

Dated source-backed tactical preferences and miniature purchasing priorities; opinions do not override N5.3 roster, profile or Fireteam data above.

**Original audit title:** JSA / Ōban / Shindenbutai — Must-have, Go-to, and Avoid (N5.3, source-backed)

*Audit 23 October 2026. Three distinct rosters: [Vanilla JSA](jsa.md), [Ōban](oban.md), [Shindenbutai](shindenbutai.md). Current pinned N5.3 Army data from Sept 2026 is authority for availability, exact profile costs, AVA and Fireteams. The following claims are **assessments grounded in directly reviewed YouTube and/or podcast MCP transcripts**, not statistical pick rates. An old interview's point cost or link assumption is NOT evidence of a current profile.*

### How to read the labels

- **Must-have / near-auto-include:** a creator expressly says "every list", "auto-include", "always", or several **actually played** builds repeatedly include it; when even one credible competing architecture omits the piece, call it "**near-must, not compulsory**" instead of inventing consensus.
- **Go-to:** source-reviewed as a repeatedly strong selection with a clear role that remains worthwhile even though an independent successful list can omit it. **Never imply all go-tos fit in one list.**
- **Never take / strong avoid:** commentator expressly rejects the **specific profile**, preferably for a direct substitute **in that same roster**, confirmed in current Army. **No faction has a defensible blanket "never take" list for every profile of an entire multi-option unit.** Where another interview disagrees, place it in **contested** rather than pretending an objective veto.
- **Specific source** is cited in the row (video/podcast, and approximate podcast minute when identifiable). These are opinions, not N5.3 legality. [Ōban transcript-reviewed tactica](../../notes/factions/oban.md), [Shindenbutai tactica](../../notes/factions/shindenbutai.md), and [Vanilla JSA event analysis](../../notes/factions/vanilla-jsa.md) contain deeper alternatives.

### 2. Shindenbutai (Army 1102)

#### Must-have / closest to universal

| Profile | Confidence, why and exception | Direct media evidence |
|---|---|---|
| **Tanuki Hacker / Pitcher / Disco Baller 20/.5** | **Near-must, very high**. One affordable *Regular* model provides hacking node projection, **Eclipse** to blind MSV lanes, mission specialist and **required anchor for Sayō** Duo/Haris. It is useful even if WIP13 never wins a cyber fight. **Not literally compulsory:** a Hatamoto/Senku, solo TAG or alternative control architecture can intentionally omit Sayō; be careful not to assume **Tanuki CoC** and **Tanuki Hacker** are simultaneously one profile. | [MetaChemistry #115 — Shindenbutai](https://open.spotify.com/episode/7DXYTzfxRzdPi8SQTniHPi) ~24m explicitly anticipates **minimum one Tanuki in every list**; [Robert Shepherd — Shinden focus](https://www.youtube.com/watch?v=odeyiO-fm4E) calls 20pt hacker unusually dense utility and puts **two** in his sample; [Dice Gods Shinden](https://www.youtube.com/watch?v=sFrtYKwC6WI) calls it a standout. |

#### Go-to

| Unit | Why and when | Direct evidence |
|---|---|---|
| **Metsuke Strategos LT22/0** or **LT(+1 Order)23/0** | Safest default command/Counterintelligence/Holoprojector shell versus extra Order for Hatamoto NCO. **Choose one option**. | [Shepherd Shinden](https://www.youtube.com/watch?v=odeyiO-fm4E): explicitly "**if in doubt, take this**" while saying Metsuke are *not* complete auto-includes. |
| **Hatamoto** (36–39pt LT variants, selected weapon; other NCO 34–41) | **Top general active HI**: specialist, Nanoscreen, Mimetism(-3), Nanoscreen, X-Visor, NCO, specialist status and substantial CC. Can operate as aggressive LT+extra Order or second NCO premium. | [MetaChemistry #115](https://open.spotify.com/episode/7DXYTzfxRzdPi8SQTniHPi) ~16–20m calls it **#1/possibly best model**; [Tactical Awareness Shinden](https://open.spotify.com/episode/7C5EmW5EwRQkHxqjHMopUi) builds two; **[Shepherd](https://www.youtube.com/watch?v=odeyiO-fm4E) publishes a no-Hatamoto list** → cannot be a genuine must-have. |
| **Shizoku HRL(+1B) Strategic Deployment** / **AP HMG FTO** | Strong **actual long-range** solution for an army otherwise tempted into all-short/mid HI, and excellent complementary Sayō gun to Tanuki+Rui Shi. | [Shepherd Shinden](https://www.youtube.com/watch?v=odeyiO-fm4E) builds a Shizoku+Tanuki+Rui Shi Haris; [MetaChemistry #115](https://open.spotify.com/episode/7DXYTzfxRzdPi8SQTniHPi) ~24m calls it primary long-range gun. *Current Sayō uses only the right Strategic Deployment Shizoku profile; don't swap in nonlegal FTO.* |
| **Rui Shi MSV2 Spitfire23/1** or **MSV1 Red Fury + Mine Dispenser21/.5** | Ideal efficient *Sayō* member with Tanuki: first shoots Mimetism targets, second builds disposable mine zones with Pangguling resupply. Different profiles, not one model with both. | [Shepherd Shinden](https://www.youtube.com/watch?v=odeyiO-fm4E) sample buys **both** with two Tanuki; [Tactical Awareness Shinden](https://open.spotify.com/episode/7C5EmW5EwRQkHxqjHMopUi) tests mine Rui Shi. |
| **Camo Yamabushi** and **Kyojin HFT+Flammenspeer15/0** | Cheap forward **independent speed bumps**, marker uncertainty, template/disposable threats; AVA2 Kyojin can trade against expensive enemies, Yamabushi one-use Camo pressures midfield. They're Irregular where roster says so; do not mistake for cheap pooled orders. | [MetaChemistry #115](https://open.spotify.com/episode/7DXYTzfxRzdPi8SQTniHPi) ~29m says both **commonly appear**; [Tactical Awareness Shinden](https://open.spotify.com/episode/7C5EmW5EwRQkHxqjHMopUi) uses duplicates. |
| **Motorized Yojimbo20/0** | Cheap fast Smoke/Koala/CC makes an asymmetric answer to conventional ranged AROs and supports Rui Shi MSV. **Not needed** if the list already uses Tanuki Disco instead of a Smoke+MSV gun plan. | [Shepherd Shinden](https://www.youtube.com/watch?v=odeyiO-fm4E) includes in sample; [Tactical Awareness Shinden](https://open.spotify.com/episode/7C5EmW5EwRQkHxqjHMopUi) reviews shared JSA bikes. |
| **Monstrucker** / **Pangguling Baggage/EVO**, as a pair of **roles**, not compulsory units | Remotes/TAGs and Pitcher/disposable schemes benefit from **repair**, Baggage reload and support-state spending when Group 2 has no good shots. Don't pay infrastructure tax in pure infantry pressure list. | [Shepherd Shinden](https://www.youtube.com/watch?v=odeyiO-fm4E) support-heavy sample; [Tactical Awareness Shinden](https://open.spotify.com/episode/7C5EmW5EwRQkHxqjHMopUi) ~17m uses Monstrucker turret to tax Orders; [Dice Gods](https://www.youtube.com/watch?v=sFrtYKwC6WI) discusses Regular-Order versus Irregular-support concerns. |
| **Raiden HRL25/1.5** | A **go-to for layered hidden ARO**, not a lone unbeatable rooftop B1 gun. Its mine/Hidden uncertainty can stall expensive advances. **Two** valid but SWC-hungry. | [Tactical Awareness Shinden](https://open.spotify.com/episode/7C5EmW5EwRQkHxqjHMopUi) ~4m takes **two**; [Shepherd](https://www.youtube.com/watch?v=odeyiO-fm4E) is more skeptical of a lone unprotected reactive shot. |

#### “Never take” / avoid — with source and patch check

| Exact profile | Verdict and competing unit | Evidence and caveat |
|---|---|---|
| **Aïda Swanson 24/.5 Decoy+Viral Minelayer, non-FTO** | **Strong avoid as general Shinden midboard trap.** **Raiden HRL25/1.5** offers Hidden Deployment, BS13, X-Visor, Mimetism, better ranged ambush and mine with only +1 point (but **+1 SWC**, not strictly identical cost). **Kyojin15** supplies cheaper mobile forward trade; Tanuki/other actual specialists score rather than paying 24 for a nonspecialist. | [Tactical Awareness Shinden](https://open.spotify.com/episode/7C5EmW5EwRQkHxqjHMopUi) ~24–26m: the panel specifically says Aïda is **outclassed**, contrasting a **+1pt Raiden**. **Counter:** Aïda has Forward Deployment(+10), **Viral** mine, Decoy and lower SWC; the **21/0 FTO Minelayer** is a different profile and can have a legitimate team/0-SWC job. Do **not** call Aïda's entire entry universally unusable. |
| **Senku basic Rifle 9/0 / HMG17/1 as “my main gun plan”** | **Avoid for premium combat function, not as inexpensive Orders/eligible team bodies.** Cheap Senku FO10, Commlink11, Paramedic11 or 9pt line can efficiently staff a planned Hatamoto team; but they are not replacements for Shizoku AP HMG/HRL, Rui Shi/Tanuki or Hatamoto as active gun. | [Dice Gods Shinden](https://www.youtube.com/watch?v=sFrtYKwC6WI) sharply criticizes generic Senku as unexceptional line infantry; [Shepherd](https://www.youtube.com/watch?v=odeyiO-fm4E) uses cheap Senku for *specific* link/utility rather than dismissing them. **Not a universal never take**: no strict cost-equivalent replacement in all Fireteam circumstances. |
| **Jizamurai bought *only* because a Bushi-tai Fireteam could exist** | **Avoid the empty tax**, not every Jizamurai: meaningful Bushi-tai + anti-HI E/Mitter/Thunderbolt reason is fine, but a pointless filler/body tying a Fireteam slot is not. | [MetaChemistry Shinden](https://open.spotify.com/episode/7DXYTzfxRzdPi8SQTniHPi) ~20m discusses Jizamurai as a **required** Bushi-tai piece supporting Hatamoto/Shizoku; [Shepherd](https://www.youtube.com/watch?v=odeyiO-fm4E) favors smaller Sayō structures in other lists. |

**Important current N5.3 reversal:** [Shurayuki](shindenbutai.md) now has **Senku-counting Wildcard** access. Early 2025 critiques of weak linkability cannot justify an N5.3 **“never take”** verdict. Similarly, [Ruby Monday](../../notes/factions/shindenbutai.md) was unavailable to early reviews, so they cannot have judged her current value.

### Cross-sectorial decision — starting a new list

| List | Start with | If you need.. | Be skeptical of.. |
|---|---|---|---|
| **Ōban** | Tankō Disco19, one Ryūken HRL23, command source/insurance | Shikami42/Karakuri durable objective, Domaru LT23 + Daiyōkai HMG50 attack engine, Kuroshi/Rui Shi/Yojimbo fast modules | Genbutai BSG18 as pure trader, Saito33 without a unique Smoke+Hidden thesis, oversized melee/hidden piles |
| **Shinden** | Tanuki Hacker20/.5, choose Metsuke22/23 vs Hatamoto LT, affordable lane opener | Rui Shi+Tanuki Sayō, Kyojin/Yamabushi tax, Raiden layer, Yojimbo, Shizoku gun | Aïda24/.5 default trap, all-Senku HMG plan, pointless max-size Fireteams |
| **Vanilla JSA** | Tankō Disco19 + ask whether Hatamoto LT+CoC and Ryūken can be shared shell | Shikami scoring, Karakuri/Yuriko durable team, alternate Raiden/hidden scalpel, one real ranged answer | Sōhei16 **unless specific classified job**, Shurayuki30 as generic fighter, Genbutai BSG18 as pure trade, extra hidden heroes |

**Do not misread the tournament example:** Azoka's two [Krug lists](../../notes/factions/vanilla-jsa.md) are **both Vanilla JSA**. Their shared choices establish an excellent *tested starting template*, not Ōban legality, Shinden AVA, population pick rate, or a global all-JSA “must”.

### Highest-value primary recordings (MCP transcripts directly retrieved in this audit)

| Video or podcast | Which explicit evaluation this supports |
|---|---|
| [Robert Shepherd Ōban](https://www.youtube.com/watch?v=AhicCreNCUQ) | Tankō Disco as signature route enabler; one Ryūken HRL as defensive baseline; Domaru versus Tankō use |
| [Tactical Awareness Ōban video](https://www.youtube.com/watch?v=nlYuuOmgfu4) · [podcast](https://open.spotify.com/episode/5EJe58gg1Lyo9xZxff2g75) | **Actual explicit "never take" 18pt Genbutai BSG**; contrasting Mushashi, Ninja and TAG/HI shells |
| [Robert Shepherd Shinden](https://www.youtube.com/watch?v=odeyiO-fm4E) | **Tanuki hacker extremely dense**, Metsuke “if in doubt,” real **no-Hatamoto** network list |
| [Tactical Awareness Shinden video](https://www.youtube.com/watch?v=z8gHfE3aZJI) · [podcast](https://open.spotify.com/episode/7C5EmW5EwRQkHxqjHMopUi) | **Aïda vs Raiden** near-price critique, two Raiden, double Hatamoto, cheap Kyojin/Yamabushi |
| [MetaChemistry #115 — Shinden](https://open.spotify.com/episode/7DXYTzfxRzdPi8SQTniHPi) | Explicit **1+ Tanuki in every list** forecast, Hatamoto and Shizoku near-defaults, cheap midfield tools |
| [The Dice Gods — Shinden](https://www.youtube.com/watch?v=sFrtYKwC6WI) | **Tanuki Hacker standout**, harsh Senku critique, Mechazoid/Triphammer opportunity cost |
| [Tactical Awareness Vanilla video](https://www.youtube.com/watch?v=YzCHVZyRY5o) · [podcast](https://open.spotify.com/episode/4IoGC1kGYyuVFhLXOjcEle) | Different vanilla lists, critical Sōhei/Genbutai/Kyoshō view, Shikami and Rui Shi options |
| [WIP12 E186 — JSA with a Pro Goblin](https://open.spotify.com/episode/5BonmJ8H86R4UCEHvWCXlz) | Explicit **Tankō Disco vanilla auto-include**, Hatamoto+Shikami, **Sōhei counterargument**, Raiden/Ryūken, Teishin KHD |
| [MetaChemistry #153 — CB Krug 2026 winner](https://open.spotify.com/episode/3VWppA6FkPPN9v001kUS0j) | **2026 practical results** Tankō Disco, Karakuri, deliberate two-list mission split and actual common shell |

**Confidence:** very high for explicitly stated Tanuki/Tankō/a few strong-avoid *profile* opinions, medium for extrapolating repeat usage to a broader meta, low for truly universal **“never take” entire units**. Absent play-rate data, a stronger categorical claim would be invented.

### Whole-unit purchasing audit — avoid the full model? (2026-10-30)

**Whole unit** means the named troop's entire usable current entry, not a weak weapon variant. The recordings do **not** justify a universal all-profile never-buy for Ōban, Shindenbutai or Vanilla JSA. These are **conditional collection deferrals** only.

| Army | Complete miniature/unit to defer | Why / still legitimate use |
|---|---|---|
| **Ōban — Saito Tōgan** | **Defer as a first stealth assassin purchase** | [Shepherd Ōban](https://www.youtube.com/watch?v=AhicCreNCUQ) compares him with cheaper Oniwaban29 and useful Ninja KHD26. Saito's **Hidden + Smoke + EXP CC** combo is *distinct*, so buy if the specific entry/smoke assassination is required. |
| **Ōban — Genbutai** | **Do NOT skip the unit** | [Tactical Awareness](https://open.spotify.com/episode/5EJe58gg1Lyo9xZxff2g75) condemns the **18pt BSG**, but **Engineer, Paramedic, Specialist and NCO Red Fury** are separate jobs that prevent a full-unit ban. |
| **Shindenbutai — Aïda Swanson** | **Defer the *non-FTO* ambush model/usage**, not every legal profile | [Tactical Awareness Shinden](https://open.spotify.com/episode/7C5EmW5EwRQkHxqjHMopUi) prefers a Raiden HRL for generic traps; the **21pt FTO Minelayer/0 SWC** is a different purchase rationale and legal team piece. |
| **Shindenbutai — Shurayuki** | **Do not categorically skip** | Some old complaints predate **N5.3 Senku-counting Wildcard**, which creates a new reason for the miniature. |
| **Vanilla JSA — Sōhei Tsugekitai** | **Defer if you do not build Firefight/Decapitation/Classified utility lists** | [Tactical Awareness](https://open.spotify.com/episode/4IoGC1kGYyuVFhLXOjcEle) questions the legacy model; [WIP12 E186](https://open.spotify.com/episode/5BonmJ8H86R4UCEHvWCXlz) documents an actual player using it for **nonspecialist objectives**. Explicit disagreement rules out a universal skip. |
| **Vanilla JSA — Kyoshō/Shurayuki** | **No proven all-profile veto** | Both retain niche hacking/command or updated Fireteam/close-combat roles; negative opinions are broad or earlier-epoch, not an exhaustive current-profile comparison. |

**Purchasing advice:** decide first whether a *unique* smoke, engineer, infiltrating or legal Fireteam role is absent from your collection. Only then turn the narrower “avoid” entries into a decision to skip a kit. [All-army shortlist](../../notes/factions/model-purchase-avoid-summary-2026.md).

### Worst-value, circumstantial and proxy-first miniature purchases by JSA army (2026-10-30)

**Scope:** Ōban, Shindenbutai, and Vanilla JSA are **three distinct current armies**, each with separate legal profiles and Fireteam charts. This section distinguishes **a genuinely criticized profile**, **a seldom-needed specialist whose dedicated miniature can be deferred**, **a strong unit worth proxying before buying duplicates**, and **a multi-body/size/legality trap**. The [pinned Ōban](oban.md), [Shinden](shindenbutai.md), and [Vanilla JSA](jsa.md) references (N5.3, Army 7.26246.159, September 2026) control exact rules. Actual direct negative evidence is from previously checked [YouTube/podcast transcripts](#highest-value-primary-recordings-mcp-transcripts-directly-retrieved-in-this-audit); **buy/proxy judgment is a reasoned inference unless called a direct reviewer verdict**. *Rare/circumstantial* means an unusual role in reviewed standard list architectures, **not measured event usage**. **No fully evidenced universal, whole-unit never-take exists.**

**Buying labels:** **Avoid profile only** = wrong gun/task for the cost, not a ban on the unit. **Defer whole dedicated model / proxy first** = a specialized valid choice whose role should be demonstrated before purchasing. **Proxy extra copy** = one model is good, but buying to AVA/owning every weapon sculpt is unnecessary. **Contested** = source disagreement or current roster changes defeat absolute rankings. A proxy must still match required silhouette/base and represent every actual separately deployed figure; check current event rules.

#### 2. Shindenbutai — current collection-aware skips and proxy priorities

**Actual source:** [your Shindenbutai miniature inventory, 2026-10-30](../../inventory/shindenbutai.md). It records **2 Tanuki, 1 Hatamoto, 3 Senku, 1 Jizamurai, 1 Raiden, 1 Mechazoid, 1 Teishin, 2 Kyojin, two physical Yáoxiè chassis shared between Rui Shi/Lù Duān, and both foot/motorized Yojimbo sculpts**. It also records **Shurayuki1, Shizoku1, Yuriko1, Yamabushi2 (shared Kestrel)**. **You explicitly wanted more Tanuki and another Hatamoto**; these are legitimate priorities to *test*, not to silently replace with a blanket “skip” because they're below AVA.

| Model or selected variant | Criticism and valid counterexample | What to do with your collection |
|---|---|---|
| **Aïda Swanson non-FTO24/.5** | **Direct — [TA Shinden](https://open.spotify.com/episode/7C5EmW5EwRQkHxqjHMopUi) ~24–26m:** **Raiden HRL25/1.5** is preferred for ordinary forward trap/ambush because of Hidden Deployment, BS13 and long-range weapon for +1pt, **but costs +1SWC**. **Aïda FTO21/0** Viral Minelayer is a separate legitimate zero-SWC Fireteam-support choice; don't equate it to the non-FTO Decoy profile. | **Aïda0, Raiden1 owned**. **Defer entire dedicated Aïda purchase / proxy first** unless the **21pt FTO, Viral Mine, zero-SWC** role specifically helps a legal formation. No all-profile dominance claim. |
| **Senku HMG17/1 or a fifth Senku solely for gunfighting** | **Direct — [Dice Gods Shinden](https://www.youtube.com/watch?v=sFrtYKwC6WI)** doubts generic BS11 Senku guns. **Senku9 basic, FO10, Commlink11, Paramedic11** have *excellent cheap order and legal team* roles. Use **Shizoku AP HMG/HRL, Rui Shi or Hatamoto** for a premium gun. | **Senku3/AVA5** already. **Avoid HMG as main gun; proxy any fourth/fifth FO/utility body** before buying. Don't buy two more only for AVA. |
| **Several Jizamurai21–24 to fill a default Bushi-tai Core** | **Inferred, not direct weak-unit opinion.** The **Jizamurai** offers Climbing Plus, Mimetism, E/Mitter/Thunderbolt and real Bushi-tai eligibility, but **Sayō/Tanuki/Rui Shi** plans don't need a Bushi-tai. [MetaChemistry Shinden](https://open.spotify.com/episode/7DXYTzfxRzdPi8SQTniHPi) discusses required Bushi-tai composition. | **Jizamurai1/AVA5 owned**. **Proxy extra Jizamurai and weapon versions**, only buy more for an actual *simultaneous, legal* Bushi-tai. No blanket no-Jizamurai. |
| **Triphammer48–53 plus TurtleMek** as an automatic second TAG | **Contested TAG choice:** [Shinden tactical guide](../../notes/factions/shindenbutai.md) and [Dice Gods](https://www.youtube.com/watch?v=sFrtYKwC6WI) compare economical **Triphammer 48–52pt, sometimes zero SWC** to a strong **Mechazoid66/1.5** Climbing Plus/CC/NCO-style alternative. **Triphammer is S7, Mechazoid S6** and each has a *different* S1 Ancillary. | **Triphammer0; Mechazoid1 owned**. **Proxy/borrow suitable S7 Triphammer + separate S1 TurtleMek** before buying any model. A second TAG belongs only in a repeated specialized list, not an AVA completion. |
| **Second Mechazoid66–69**, solely because AVA2 | **Good TAG, costly duplicate.** A legal **Mechazoid Duo** exists, but two TAGs devour Orders, Engineer and objective budget. Current Mechazoid includes **Kobaruto S1**, which is a separate Ancillary body **without its own Regular Order**. | **Mechazoid1/AVA2**. **Proxy second correct-sized S6 TAG + additional Kobaruto** before buying. **Kobaruto physical ownership not reported**; do not assume already owned or count it as zero confirmed. |
| **Second Hatamoto34–41** / extra gun variants | **Pro and con sources:** [MetaChemistry Shinden](https://open.spotify.com/episode/7DXYTzfxRzdPi8SQTniHPi) and [TA Shinden](https://open.spotify.com/episode/7C5EmW5EwRQkHxqjHMopUi) like **two Hatamoto**; [Shepherd Shinden](https://www.youtube.com/watch?v=odeyiO-fm4E) has a strong **no-Hatamoto** list. Every Hatamoto option has **NCO**, with Plasma/Red Fury/Spitfire/LT +1 Order jobs. | **Hatamoto1/AVA2; second explicitly desired.** **Proxy-test a second *simultaneous* Hatamoto** and buy if it repeatedly pays; one sculpt covers *alternative non-simultaneous guns*. This is a defensible purchase, not a default avoid. |
| **Tanuki third/fourth/fifth model** without a named Sayō/command role | **Strong positive first models, selective extras:** [Shepherd](https://www.youtube.com/watch?v=odeyiO-fm4E) and [MetaChemistry](https://open.spotify.com/episode/7DXYTzfxRzdPi8SQTniHPi) praise **Tanuki Hacker20/.5** for **Pitcher/Disco + Sayō anchor**. **CoC18, Engineer19, Paramedic20, MSV2 HMG29/1.5, MSV2 Sniper27/1.5** are all separate profiles, not free upgrades on the Hacker. | **Tanuki2/AVA5, additional desired.** First build with existing two; **proxy third Tanuki** if a *Hacker plus CoC/Engineer/sniper* plan needs three simultaneous bodies, then buy one if recurring. **Do not order three more merely to reach AVA5.** |
| **Raiden Missile Launcher33/2 or buying to Raiden AVA3** | **Contested:** [TA Shinden](https://open.spotify.com/episode/7C5EmW5EwRQkHxqjHMopUi) plays two **Raiden HRL25/1.5**, while [Shepherd](https://www.youtube.com/watch?v=odeyiO-fm4E) questions overpaying for an isolated B1 ARO. **ML33/2** is 8pts/.5SWC above HRL; distinct range/template/ammo prevent strict domination. | **Raiden1/AVA3**. **Proxy second/third or ML sculpt** and purchase only if multiple separate Hidden lanes prove useful. |
| **Shurayuki30 solo bruiser**, or another Shurayuki sculpt | [WIP12 Vanilla](https://open.spotify.com/episode/5BonmJ8H86R4UCEHvWCXlz) is skeptical of a 30pt 1W+NWI bruiser. **Current Shinden N5.3 expressly grants Senku-counting Wildcard**: old no-link criticism is obsolete; Holomask/Viral CC and specific teams have real merit. | **Shurayuki1 owned, AVA1**. **No second purchase.** Can *physically proxy Metsuke0* using that model, **only when not simultaneously fielding Shurayuki**. |
| **Saito/Ninja when missions don't need another Hidden attacker** | **Inferred:** Saito's Hidden+Smoke+EXP, Ninja Hidden cyber/CC, **Kurayami** hacking, **Nokizaru** MSV/FO and **Teishin KHD21/FO19** have differing roles. One duplicate elite assassin can be redundant if Teishin/Nokizaru score already. | **Saito0, Ninja0**, but **Kurayami1, Nokizaru1 and Teishin1** available. **Proxy Saito/Ninja with a suitable spare Kurayami/Nokizaru**; avoid simultaneous collision. |
| **Metsuke22–23** solely because a dedicated sculpt is missing | **Actually a strong go-to:** [Shepherd Shinden](https://www.youtube.com/watch?v=odeyiO-fm4E) calls Metsuke “if in doubt” commander; distinct **Strategos vs LT(+1 Order)** options. Model may be worth buying if both command/other hidden identities are present. | **Metsuke0; Shurayuki1 is proposed proxy**. **Keep proxy for now**, buy proper Metsuke if routinely fielding Metsuke *and* Shurayuki or tournament clarity demands it. |
| **Sāchā, Ruby Monday, extra Teishin/Kyojin** as catalog purchases | **Lower-confidence, no old-tape verdict**: **Ruby19 Irregular STR2 specialist** is a current real option **not graded by early recordings**; **Sāchā** mission-dependent Irregular role; **Teishin** Combat Jump KHD/FO and **Kyojin** disposable templates can genuinely work. | **Sāchā0, Ruby0, Teishin1, Kyojin2/2 already**. **Proxy the missing named specialists first**; no extra Kyojin needed, and second Teishin only for true simultaneous off-table play. |
| **All four Aibōts, Pangguling and extra Yáoxiè or servants bought as new kits** | **Useful REMs, often purchase redundancy:** **Robio7 Repeater, Atom Sensor/FO, Garon TR/Smoke GL, Uran Guided** have different jobs; **Pangguling Baggage** helps reloading while EVO/Guided require an actual plan. Different silhouette/base and simultaneous physical counts matter. | **0 dedicated Aibōts/Pangguling** but owned **4 PanO Dronbots and 2 PanO Mulebots** are proposed proxies; **two shared physical Yáoxiè** for Rui Shi/Lù Duān; **2 Yudbots or 2 Palbots** are servant proxies. **Use these first, without counting one model as multiple remotes simultaneously.** |
| **Monstrucker, Taguraidā support pilot, Yáozăo and Kobaruto/TurtleMek accessories** with no matching asset | **Repair support is strong when a TAG/REM is present; otherwise conditional.** **Monstrucker is Irregular**, **Taguraidā is a separately selectable model**, **Kobaruto/TurtleMek are Ancillaries**, **Yáozăo are Servants**. | **Monstrucker0 → owned Tech-Bee proxy; Taguraidā0 → HVT suggestion not independently owned; Servants0 dedicated → Yudbot/Palbot proxies.** Ancillary/bot counts are **unreported**, not confirmed absent. Buy only missing simultaneously needed physical figures. |
| **Both Yojimbo sculpts, another Yamabushi or Warcor** | No power issue. Yojimbo forms are **mutually exclusive in one list**, while **Yamabushi Regular** has independent FTO/camo use and **Warcor** is Irregular. | Already have **one Yojimbo mounted + one foot**, **two Yamabushi** (shared Kestrel) and **one shared Warcor**. **Buy none of these again for Shinden.** |

**Shinden purchasing action order:** **Keep existing Tanuki/Hatamoto/Raiden/Mechazoid/Yojimbo, test a third Tanuki and a second Hatamoto** because both were on the actual wishlist, reuse **PanO Dronbots/Mulebots, Tech-Bee, Yudbots/Palbots**, and **defer Aïda24, Triphammer, additional Senku/Jizamurai, second/third Raiden, Saito and Ruby/Sāchā** until a named mission or legal team requires them. Ownership of Kobaruto, TurtleMek, CrazyKoala markers, the proposed Dog-Warrior and HVT bodies is **not verified**. [Shinden inventory](../../inventory/shindenbutai.md).

#### 4. Cross-JSA — even good miniatures better represented by proxies or shared bodies

**Ownership boundary:** only [Shindenbutai](../../inventory/shindenbutai.md) currently has a verified 2026-10-30 miniature inventory. Its known physical miniatures may be **reused for the same legal troop in another JSA army**, but **no independent Ōban/Vanilla whole-collection count was found**. Do not assume the user physically owns Ōban-only Tankō, Domaru, Shinobu or O-Yoroi.

| Miniature category | Good proxy-first/reuse choice | Physical, rules and buying limit |
|---|---|---|
| **Alternate S2 troop/weapon sculpts** — Tanuki hacker/CoC/MSV2 gun, Hatamoto Plasma/Red Fury/Spitfire, Senku FO/Commlink/HMG, Jizamurai Thunderbolt/E/Mitter, Shikami42/47, Genbutai BSG/Engineer, Ryūken HRL/KHD, Aïda FTO/non-FTO | Use **one correctly sized and distinguishable miniature** per selected trooper, declaring the actual option and card. **Tanuki Hacker20/.5 is not also CoC18**, and Aïda21 FTO does not inherit non-FTO Decoy. | Extra exact-weapon miniatures only when *two profiles are fielded together* and the event's proxy standards require them. An FTO label is not universal Fireteam permission. |
| **Named character and Hidden operative proxies** — Saito, Shinobu, Ninja, Oniwaban, Kyoshō, Metsuke, Shurayuki | **Owned Shinden Kurayami1/Nokizaru1** are explicit potential **Ninja/Saito** proxies; **owned Shurayuki1** can proxy **Metsuke0**. Hidden/Camo/Decoy models need distinguishable markers and correct silhouette when revealed. | A model used as Saito cannot *also* be Kurayami in that same army list. Buy a dedicated character when both are repeatedly taken together or event policy requires more visual distinction. |
| **Bike versus foot Yojimbo, Aragoto/Kuroshi and other rider sculpts** | **Mounted and foot Yojimbo are both physically owned (1 each)**. Use the correct silhouette/form for the current selected mode. A correct-size motorcycle may proxy a different legal biker in another game. | **Only one Yojimbo identity may be fielded in a list.** A second sculpt is not a second permitted trooper; a separate Aragoto or Kuroshi on the same table needs another physical model. |
| **Shared JSA remotes** — Rui Shi / Lù Duān, Robio/Garon/Uran/Atom Aibōts, Pangguling and Yáozăo | **Two total Yáoxiè chassis** shared Rui Shi/Lù Duān; **4 PanO Dronbots** proposed Aibōt proxies, **2 PanO Mulebots** for Pangguling; **2 ALEPH Yudbots / 2 PanO Palbots** potential Servants. Only matching base and silhouette qualify. | Do not count two Yáoxiè as two *each* Rui Shi and Lù Duān in the same list. A different REM chassis/weapon or Supportware plan may justify distinct models, especially when all used simultaneously. |
| **TAG and Ancillary pairings** — Mechazoid S6+Kobaruto, O-Yoroi S7+Kobaruto, Triphammer S7+TurtleMek | **Mechazoid1 physically owned**; borrow correctly sized TAG if testing O-Yoroi/Triphammer; **Ancillaries must be separate represented S1 models**. A S7 TAG isn't automatically a permitted stand-in for an S6 TAG. | Buy when recurring exact TAG plans or a simultaneous second TAG require a distinct chassis; **Kobaruto/TurtleMek physical ownership is unreported**, not proven absent. Ancillaries are not extra Regular Orders. |
| **Repair specialists and servants** — Tokusetsu, Monstrucker, Yuriko, Taguraidā, Yáozăo | **Owned Tech-Bee1** is suggested Monstrucker proxy, **Yudbot/Palbot** can proxy Yáozăo, **Yuriko1 owned**, Taguraidā has a proposed but **unconfirmed HVT** stand-in. | Buy only if a real Doctor/Engineer/Servant repair architecture needs more *simultaneous* figures. A Servant isn't an independent Regular-order generator. |
| **Extra optional-mode Spec-Ops / Team-Ops and old Fireteam box sets** | These modes aren't standard roster entries by default. Old N4 links don't override 2026: **Shinden Shurayuki now counts as Senku**, but **Shinden/Ōban Pangguling FTO still does not grant Fireteam access**. | Do not buy a model/box solely for an illegal or optional-mode team. Current charts decide legality, not a sculpt name. |
| **Physical markers vs extra troops** — CrazyKoalas, Disco Ballers, mines, Decoys, Turrets, Kobaruto/TurtleMek | Make actual deployed **Ancillary/Servant** models physically distinct, but use clear legal markers for equipment and hidden/Decoy states; mark the selected loadout so opponents can follow it. | Koala/mines/disco markers do not create new pooled Orders. Avoid buying multiple premium kits simply to obtain optional equipment markers. |

**Shopping priority by *real need*, not AVA:** For **Ōban**, buy/represent the first **Tankō Disco19**, one **Ryūken HRL**, a real objective specialist, a coherent Domaru/Keisotsu/long-gun engine; proxy Saito, second Shikami/Karakuri, extra bike/TAG. For **Shinden**, keep **existing two Tanuki, first Hatamoto, Raiden, Mechazoid, Kyojin/Yojimbo, support REM proxies**, **proxy-test third Tanuki and second Hatamoto** (the actual desired extras), postpone extra Jizamurai/Senku, Aïda non-FTO, Triphammer. For **Vanilla**, prioritize **Tankō Disco19**, **Hatamoto LT+Kempeitai CoC if following proven 2026 template**, first Ryūken, low-cost Robio/Pangguling and mission scoring, and defer extra hidden killers / alternative TAGs.

**Event safety:** choose a unit *legally present* in the selected current N5.3 roster, then proxy only with an appropriate, identifiable **silhouette/base and number of physical troopers**, with peripheral/ancillary bodies separately represented. Check current ITS/organizer policy for competitive games and agree substitutions with casual opponents. Proxies do **not** grant missing profiles, adjust SWC or AVA, revive obsolete Fireteams, or permit one sculpt to stand for two simultaneous troopers.

**Condensed purchasing verdict:** Ōban's clearest **profile-only no-buy is Genbutai BSG18**; Shinden's clearest direct **profile traps are Aïda24 non-FTO and generic Senku HMG17**, while **Triphammer and surplus expensive model quantities** are test-before-buy; Vanilla's main **whole-model defers are Sōhei/Kyoshō/standalone Shurayuki**, plus extra elite assassins and alternative TAGs. **Tankō, Tanuki, Hatamoto, Ryūken, Karakuri, Shikami and well-planned support REMs remain strong choices**.
