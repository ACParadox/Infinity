---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 605
sectorial_slug: next-wave
sectorial_name: Next Wave
parent_faction: Combined Army
rules_baseline: N5.3
army_source_version: "7.26246.158"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-15
coverage: "Next Wave standard roster, AVA, profile stats and points/SWC, canonical Fireteam chart and reverse access index, optional Spec-Ops/Team-Ops hooks, and the separate Exrah Comissariat Reinforcement Fireteam chart."
---

# Next Wave

## Overview and provenance

Repository-native reference for the **Next Wave** sectorial roster, profile stats, points/SWC, AVA, canonical Fireteams, and linked Reinforcements in the pinned N5 Army source.

Sources used:

- Army-derived Next Wave source revision `7.26246.158` from `massayoshi/infinity-army-backup` commit `d4329bb596ffea5d568eb2435f74366c305a7630`.
- InfinityDB Fireteam normalization/semantics at commit `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: N5.3 + N5 FAQ v0.1.

Coverage notes:

- Covers the **35-unit standard Next Wave roster** in the pinned Army source.
- `BLUR SPEC-OPS`, `NEXUS-7 SPEC-OPS`, and `NEXT WAVE TEAM-OPS` are optional game-mode content and are listed separately rather than counted in the 35 standard entries.
- Generic Soldier of Fortune / `merc-*` catalogue entries with empty faction lists are excluded from the standard roster.
- Cross-faction entries are retained when the ordinary source entry explicitly contains faction ID `605`; this includes **Kazurabā Ruby Monday**, **Cube Jäger**, and **Ioann Bann**.
- Fireteam legality comes from the canonical Army chart, not from an `FTO` profile label alone.
- Profile-specific Fireteam access is preserved for **Patroclus FTO, Teucer FTO, Drakios FTO, Ko Dali FTO / FTO-2, Raindancer FTO, Wraith-1 FTO, and Gearhead FTO**.
- Ko Dali has two distinct linked profiles in the source: **FTO** and **FTO-2**. Team Achilles explicitly uses **FTO-2**; Harbinger, Heavies, and Control teams explicitly use **FTO**.
- Multiple `required: true` rows in the same mixed Fireteam are preserved as a **required-choice set**, not interpreted as requiring every marked troop simultaneously.
- Army `spec.DUO = 256` is treated as **unlimited Duos**.
- **Team Achilles Fireteams explicitly prohibit Wildcards.** The sectorial's normal Wildcards therefore do not enter that pool.
- Linked Reinforcement army ID `699` is **The Exrah Comissariat**. Its Fireteam chart is recorded separately and is not merged into standard Next Wave Fireteams.

## Sectorial summary

| Field | Value |
|---|---|
| Sectorial | Next Wave |
| Army ID | 605 |
| Army slug | `next-wave` |
| Parent faction | Combined Army, ID `601` |
| Discontinued | No |
| Rules baseline | N5.3 + FAQ v0.1 |
| Standard roster units | 35 |
| Optional-mode units | Blur Spec-Ops; Nexus-7 Spec-Ops; Next Wave Team-Ops |
| Reinforcement roster | The Exrah Comissariat, Army ID `699` |
| Fireteam limits | Core 1; Haris 2; Duo unlimited |

## Standard roster index

| Unit | ID | AVA | Type | Order / structure | Fireteam access |
|---|---:|---:|---|---|---|
| Contrabandoleros, Resource Extraction Team | 1883 | 2 | SK | Regular | — |
| Tekdrakens: Steeljaws | 1887 | 4 | WB | Irregular | Shadow / Research / Dragon / Heavies / Control |
| Med-Tech Obsidon Medchanoids | 507 | 1 | LI | Regular | — |
| Slave Drones | 526 | 2 | REM | Peripheral | — |
| Skyhounds, Combat and Recon Air Squadron | 1889 | 1 | VH | Regular | — |
| Gearheads, Tech Savant Team | 1884 | 2 | LI | Regular | **FTO profiles only** as Wildcard, max 1 |
| Tekdrakens: Blackhearts | 1888 | 4 | WB | Irregular | Research / Harbingers / Heavies / Control |
| Unidron Batroids | 493 | 2 | REM | Regular | Control required-choice foundation |
| Pandora, Team Achilles' Field Researcher | 1859 | 1 | LI | Regular | Team Achilles / Research |
| Teucer, Team Achilles' Shooter | 1860 | 1 | MI | Regular | **FTO profile only** in Team Achilles / Harbingers |
| M-Drones | 508 | 2 | REM | Regular; TacAware option | Control max 1 |
| Ikadron Batroid | 532 | 2 | REM | Regular | — |
| Bit & KISS! | 965 | 1 | LI + Peripheral | Regular | — |
| Special Operative Ko Dali | 1516 | 1 | MI | Regular | **FTO / FTO-2 profile-specific** |
| Sartroids: Puzzlers | 1886 | 2 | REM | Peripheral / Cyberplug | — |
| Nexus Operatives | 783 | 2 | MI | Regular | Wildcard max 2; counts as Unidron / Harbingers |
| Juggernauts, Armored Assault Cavalry | 1882 | 2 | TAG | Regular + Tactical Awareness | Heavies Duo foundation |
| Sartroids: Ranters | 1885 | 2 | REM | Peripheral / Cyberplug | — |
| Ironsides Heavy Mobile Regiment | 1881 | 3 | HI | Regular + Tactical Awareness | Dragon / Heavies |
| Stingers, Security Tactical Unit | 1877 | 3 | LI | Regular | Research max 3 |
| Wraith-1, Clandestine Action Group | 1880 | 2 | MI | Regular | **FTO profile only** in Research / Harbingers |
| Q-Drones | 509 | 1 | REM | Regular | — |
| Achilles | 1863 | 1 | HI | Regular; Lieutenant options | Team Achilles / Shadow / Research / Harbingers / Dragon |
| Drakios, Team Achilles' Dragon | 1861 | 1 | MI | Regular | **FTO profiles only** in Team Achilles / Dragon |
| Harbingers, New Mankind Defense Infantry | 1876 | 5 | LI | Regular | Shadow / Harbingers |
| Kazurabā Ruby Monday | 1890 | 1 | HI | Irregular | — |
| Raindancers, Light Assault Company | 1878 | 3 | LI | Irregular | **FTO profiles only** in Team Achilles / Shadow / Dragon |
| Cliff-Jumpers, Extreme Jump Unit | 1879 | 3 | LI | Regular | — |
| T-Drones | 510 | 1 | REM | Regular | — |
| E-Drones | 741 | 2 | REM | Regular | — |
| Cube Jäger, Mercenary Recoverers | 956 | 1 | LI | Irregular | — |
| Glyph Warcors, Ur Hegemony Journalists | 1873 | 1 | LI | Irregular | — |
| Patroclus, Team Achilles' Shadow | 1850 | 1 | HI | Regular | **FTO profiles only** in Team Achilles / Shadow |
| R-Drones | 511 | 1 | REM | Regular | — |
| Ioann Bann, Varangian Dog-Warrior | 1940 | 1 | WB | Irregular + Impetuous | — |

## Optional game-mode units

| Unit | ID | Role / note |
|---|---:|---|
| Blur Spec-Ops | 1921 | Infinity Spec-Ops; charted as optional member of Shadow and Harbinger Fireteams |
| Nexus-7 Spec-Ops | 1918 | Infinity Spec-Ops; no row in the pinned standard Next Wave Fireteam chart |
| Next Wave Team-Ops | 1935 | Team-Ops package; no row in the pinned standard Next Wave Fireteam chart |

## Profile reference

The lines below preserve the pinned Next Wave profile stats and all standard option costs/SWC. Weapon text is abbreviated where the profile's tactical identity is more useful than reproducing the entire Army serialization.

### Contrabandoleros, Resource Extraction Team

**ID 1883 · AVA 2 · SK** — `MOV 10-10 | CC 16 | BS 12 | PH 11 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Camouflage, Hidden Deployment, Infiltration (PH=16), Mimetism (-3), Stealth.

| Pts | SWC | Profile summary |
|---:|---:|---|
| 29 | 0 | Combi Rifle, Zapper, PARA Mine |
| 29 | 0.5 | Hacker; SMG, Zapper, D-Charges |
| 27 | 0 | Killer Hacker; SMG, Zapper, D-Charges |
| 26 | 0.5 | Minelayer; SMG, Zapper, Shock Mine |
| 26 | 0 | Forward Observer; Boarding Shotgun, Zapper, Flash Pulse, D-Charges |

No standard Fireteam access.

### Tekdrakens: Steeljaws

**ID 1887 · AVA 4 · WB** — `MOV 15-10 | CC 23 | BS 10 | PH 13 | WIP 13 | ARM 2 | BTS 3 | W 2 | S 5`. Irregular; Martial Arts L2, Mimetism (-3), Technorganic, Climbing Plus, Religious Troop.

| Pts | SWC | Profile summary |
|---:|---:|---|
| 18 | 0 | Sensor; Flash Pulse, Grenades, Viral Mine, Viral CC Weapon |
| 19 | 0 | Flash Pulse, Grenades, Armed Turret (Combi Rifle), Viral CC Weapon |

**FT:** Shadow max 2; Research max 2; Dragon max 2; Heavies max 1; Control required-choice max 2, where it counts as `Tekdraken`.

### Med-Tech Obsidon Medchanoids

**ID 507 · AVA 1 · LI** — `MOV 15-10 | CC 16 | BS 11 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 3`. Doctor + Engineer.

**Options:** `21/0`, `22/0` Deployable Cover, `24/0` Armed Turret (Combi), `25/0` Armed Turret (Marksman), `24/0.5` Cyberplug. No standard Fireteam access.

### Slave Drones

**ID 526 · AVA 2 · REM** — `MOV 15-10 | CC 11 | BS 8 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 1`. Servant Peripheral.

**Option:** `3/0`. No standard Fireteam access.

### Skyhounds, Combat and Recon Air Squadron

**ID 1889 · AVA 1 · VH** — `MOV 20-5 | CC — | BS 14 | PH 13 | WIP 13 | ARM 4 | BTS 6 | W 2 | S 7`. Aerial, Remote Presence, Tech-Recovery, Mimetism (-6), No Cover, enhanced Super-Jump/jet mobility.

| Pts | SWC | Profile summary |
|---:|---:|---|
| 33 | 0 | Plasma Carbine, AP Thunderbolt, Mine Dispenser; BS Attack (+1B) |
| 31 | 0 | MULTI Rifle (+1B), Flammenspeer, Mine Dispenser |

No standard Fireteam access.

### Gearheads, Tech Savant Team

**ID 1884 · AVA 2 · LI** — `MOV 10-10 | CC 14 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Technorganic / Cyberplug support family.

| Pts | SWC | Profile summary | FT |
|---:|---:|---|---|
| 13 | 0 | Vulkan Shotgun, Zapper; Cyberplug | — |
| 17 | 0 | Engineer, GizmoKit; Vulkan Shotgun, Zapper | — |
| 18 | 0 | **GEARHEAD FTO**, Engineer; Combi Rifle, Zapper, D-Charges | **Wildcard** |
| 19 | 0.5 | **GEARHEAD FTO**, Hacker Firewall (-6), Pitcher | **Wildcard** |
| 13 | 0 | **GEARHEAD FTO**, TAGCom / Minelayer utility | **Wildcard** |

Only the profiles explicitly named **GEARHEAD FTO** receive the Wildcard row.

### Tekdrakens: Blackhearts

**ID 1888 · AVA 4 · WB** — `MOV 15-10 | CC 17 | BS 13 | PH 12 | WIP 13 | ARM 2 | BTS 3 | W 2 | S 5`. Irregular; Technorganic, Mimetism (-3), Religious Troop.

**Options:** `25/0` Contender/Panzerfaust/E/Marat/Mine Dispenser; `29/0` MULTI Marksman Rifle; `27/0.5` Plasma Carbine; `29/0` AP Thunderbolt + E/M Carbine. **FT:** Research max 2; Harbingers max 1; Heavies max 1; Control required-choice max 2, where it counts as `Tekdraken`.

### Unidron Batroids

**ID 493 · AVA 2 · REM** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 12 | ARM 1 | BTS 6 | W 1 | S 2`. Remote Presence, Courage, Dogged.

| Pts | SWC | Profile summary |
|---:|---:|---|
| 14 | 0 | Plasma Carbine |
| 14 | 0 | K1 Combi Rifle |
| 15 | 0.5 | K1 Combi Rifle + TinBot Firewall (-3) |
| 24 | 1.5 | Plasma Sniper Rifle |
| 20 | 1.5 | Missile Launcher + Light Shotgun |
| 18 | 1 | Spitfire |
| 15 | 0 | Forward Observer, Plasma Carbine |
| 16 | 0 | Commlink (+1), Specialist Operative, Plasma Carbine |

**FT:** Control required-choice foundation, max 2. Nexus Wildcards count as Unidrons.

### Pandora, Team Achilles' Field Researcher

**ID 1859 · AVA 1 · LI** — `MOV 10-10 | CC 17 | BS 12 | PH 12 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`. NWI; Hacker with Zero Pain upgrade family; FT Master (Stingers).

**Options:** `24/0.5`; `26/0.5` with MediKit (+1B); `26/0.5` SMG/Pitcher; `29/0.5` Chain of Command. **FT:** Team Achilles max 1; Research **mandatory anchor** 1.

### Teucer, Team Achilles' Shooter

**ID 1860 · AVA 1 · MI** — `MOV 10-10 | CC 17 | BS 14 | PH 11 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. MSV2, Mimetism (-3), NWI.

| Pts | SWC | Profile summary | FT |
|---:|---:|---|---|
| 34 | 1.5 | Plasma Sniper Rifle | — |
| 35 | 1.5 | **TEUCER FTO**, Feuerbach | Team Achilles / Harbingers |
| 37 | 1.5 | Plasma Sniper Rifle, Neurocinetics | — |

### M-Drones

**ID 508 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Sensor, Forward Observer, Repeater, Deactivator, Triangulated Fire.

**Options:** `15/0`; `18/0` Tactical Awareness. **FT:** Control max 1.

### Ikadron Batroid

**ID 532 · AVA 2 · REM** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 6 | W 1 | S 2`. Baggage, Repeater, Remote Presence.

**Option:** `11/0`, Light Flamethrower (+1B). No standard Fireteam access.

### Bit & KISS!

**ID 965 · AVA 1 · LI + Peripheral** — Bit: `MOV 10-10 | CC 14 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 6 | W 1 | S 2`.

**Option:** `25/0.5` Hacker; SMG, Pitcher; includes KISS Repeater Peripheral. No standard Fireteam access.

### Special Operative Ko Dali

**ID 1516 · AVA 1 · MI** — `MOV 15-5 | CC 19 | BS 14 | PH 12 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. MSV2, Martial Arts L3, NWI/Protheion package.

| Pts | SWC | Profile summary | FT |
|---:|---:|---|---|
| 37 | 0 | Combat Jump / Parachutist; MULTI Rifle, Pulzar | — |
| 34 | 0 | Forward Deployment +20; MULTI Rifle, Pulzar | — |
| 33 | 0 | **KO DALI FTO**, Strategic Deployment, Mimetism (-3) | Harbingers / Heavies / Control |
| 30 | 0 | **KO DALI FTO-2**, Number 2, Mimetism (-3) | **Team Achilles only** |

The canonical chart distinguishes `FTO` from `FTO-2`; do not merge the two permissions.

### Sartroids: Puzzlers

**ID 1886 · AVA 2 · REM Peripheral**. Connected: `MOV 20-5 | CC 15 | BS 12 | PH 10 | WIP 12 | ARM 3 | BTS 6 | W 1 | S 5`; autonomous: `MOV 15-10 | CC 12 | BS 10 | PH 9 | WIP 11 | ARM 3 | BTS 6 | W 1 | S 5`. Cyberplugged infiltrating Peripheral.

**Options:** `13/0` Adhesive Launcher Rifle + E/Marat + Stun Pistol (+1B); `12/0` Akrylat-Kanone + E/Marat + Stun Pistol (+1B). Generates no order on its own. No standard Fireteam access.

### Nexus Operatives

**ID 783 · AVA 2 · MI** — `MOV 10-10 | CC 17 | BS 13 | PH 11 | WIP 13 | ARM 2 | BTS 6 | W 1 | S 2`. NCO, Number 2, Mimetism (-3).

**Options:** `24/0.5` Hacker with Oblivion (+1B); `27/0.5` Hacker with Carbonite (+1B); `23/0` Engineer; `29/1` Spitfire + Nanoscreen / No Cover; `22/0` Specialist Operative; `27/0.5` Lieutenant Hacker. **FT:** Wildcard max 2, counts as **Unidron** and **Harbingers**. Team Achilles still forbids Wildcards.

### Juggernauts, Armored Assault Cavalry

**ID 1882 · AVA 2 · TAG** — `MOV 20-5 | CC 22 | BS 14 | PH 15 | WIP 13 | ARM 8 | BTS 6 | W 3 | S 7`. Tactical Awareness, Remote Presence, Guard, Technorganic, Climbing Plus, integrated Staldron.

| Pts | SWC | Profile summary |
|---:|---:|---|
| 82 | 1.5 | Plasma Rifle (+1B), Heavy Rocket Launcher |
| 81 | 1.5 | MULTI HMG, **NCO** |
| 78 | 1.5 | MULTI HMG, **Lieutenant** |

**FT:** Heavies Duo required-choice foundation, max 2.

### Sartroids: Ranters

**ID 1885 · AVA 2 · REM Peripheral**. Connected: `MOV 15-10 | CC 16 | BS 13 | PH 12 | WIP 12 | ARM 3 | BTS 6 | W 1 | S 5`; autonomous: `CC 12 | BS 11 | PH 11 | WIP 11` with the same movement/defences. Cyberplugged Forward Deployment (+10), Mimetism (-6).

**Options:** `18/0` Mk12; `19/1` Spitfire; `12/0` SMG + Thunderbolt. Generates no order on its own. No standard Fireteam access.

### Ironsides Heavy Mobile Regiment

**ID 1881 · AVA 3 · HI** — `MOV 15-5 | CC 17 | BS 13 | PH 12 | WIP 13 | ARM 3 | BTS 6 | W 2 | S 2`. Albedo (-3), Combat Instinct, Tactical Awareness, Technorganic, Religious Troop.

| Pts | SWC | Profile summary |
|---:|---:|---|
| 36 | 0 | MULTI Rifle, Light Flamethrower, Disco Baller |
| 44 | 1.5 | AP HMG |
| 37 | 1.5 | Heavy Rocket Launcher, E/M Carbine |
| 34 | 0 | Killer Hacker; SMG, E/Mitter |
| 36 | 0 | Lieutenant, MULTI Rifle package |

**FT:** Dragon max 2; Heavies required-choice max 2.

### Stingers, Security Tactical Unit

**ID 1877 · AVA 3 · LI** — `MOV 10-10 | CC 15 | BS 13 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Mimetism (-3), NCO, Warhorse, Religious Troop.

**Options:** `26/0` MULTI Marksman Rifle; `30/1` HMG; `25/0` Killer Hacker; `25/0` Forward Observer; `29/0.5` MSV2 MULTI Marksman Rifle. **FT:** Research max 3.

### Wraith-1, Clandestine Action Group

**ID 1880 · AVA 2 · MI** — `MOV 10-10 | CC 15 | BS 12 | PH 11 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. MSV1, Biometric Visor, Mimetism (-3), Marksmanship.

| Pts | SWC | Profile summary | FT |
|---:|---:|---|---|
| 28 | 1.5 | MULTI Sniper Rifle, Surprise Attack, Hidden Deployment | — |
| 27 | 0.5 | MULTI Marksman Rifle, Surprise Attack, Forward Deployment +10, Hidden Deployment | — |
| 25 | 0.5 | **WRAITH-1 FTO**, MULTI Marksman Rifle, Forward Deployment +10 | Research / Harbingers |

### Q-Drones

**ID 509 · AVA 1 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Remote Presence, Total Reaction, Mimetism (-3), 360º Visor.

**Options:** HMG `25/1`; Plasma Rifle `24/1`; Thunderbolt (+1B) `20/0.5`. No standard Fireteam access.

### Achilles

**ID 1863 · AVA 1 · HI** — `MOV 15-10 | CC 24 | BS 15 | PH 15 | WIP 15 | ARM 3 | BTS 6 | W 3 | S 2`. Nanoscreen, Martial Arts L4, Mimetism (-3), No Cover, Stealth, Frenzy.

| Pts | SWC | Profile summary |
|---:|---:|---|
| 62 | 1.5 | AP Spitfire, Pulzar, EXP CC Weapon |
| 63 | 0 | Plasma Rifle, Pulzar, EXP CC Weapon |
| 62 | 1 | Lieutenant, AP Spitfire |
| 63 | +1 | Lieutenant, Plasma Rifle; **+1 SWC** |

**FT:** mandatory anchor in Team Achilles; required-choice member of Shadow; optional in Research, Harbingers, and Dragon.

### Drakios, Team Achilles' Dragon

**ID 1861 · AVA 1 · MI** — `MOV 15-5 | CC 21 | BS 13 | PH 13 | WIP 13 | ARM 2 | BTS 3 | W 2 | S 5`. Albedo (-6), Bangbomb, Martial Arts L1, Specialist Operative, Combat Instinct, FT Master. Ordinary profiles include a Kydoimos Peripheral.

| Pts | SWC | Profile summary | FT |
|---:|---:|---|---|
| 37 | 0 | MULTI Rifle, Heavy Flamethrower (+1B), Panzerfaust + Kydoimos | — |
| 39 | 0 | Mk12, Heavy Flamethrower (+1B) + Kydoimos | — |
| 39 | 1 | Red Fury, Heavy Flamethrower (+1B) + Kydoimos | — |
| 31 | 0 | **DRAKIOS FTO**, MULTI Rifle package, no Kydoimos | Team Achilles / Dragon |
| 33 | 0 | **DRAKIOS FTO**, Mk12 package, no Kydoimos | Team Achilles / Dragon |
| 33 | 1 | **DRAKIOS FTO**, Red Fury package, no Kydoimos | Team Achilles / Dragon |

### Harbingers, New Mankind Defense Infantry

**ID 1876 · AVA 5 · LI** — `MOV 10-10 | CC 15 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Courage, Combat Instinct.

| Pts | SWC | Profile summary |
|---:|---:|---|
| 13 | 0 | Combi Rifle, Zapper |
| 20 | 1 | HMG |
| 18 | 1.5 | Missile Launcher, Breaker Pistol (+1B) |
| 17 | 0 | AP Marksman Rifle, Zapper |
| 15 | 0 | Commlink (+1), Specialist Operative |
| 18 | 0.5 | Hacker + Minelayer, Vulkan Shotgun, E/M Mine |
| 14 | 0 | Minelayer, Vulkan Shotgun, Shock Mine |
| 13 | 0 | Forward Observer, AP SMG, Flash Pulse (+1B), WildParrot |
| 15 | 0 | Paramedic, Combi Rifle |
| 13 | 0 | Lieutenant, Combi Rifle |
| 17 | 0 | Killer Hacker + Deployable Repeater |

**FT:** Shadow required-choice foundation max 5; dedicated Harbingers team 1–4. Nexus Wildcards count as Harbingers.

### Kazurabā Ruby Monday

**ID 1890 · AVA 1 · HI** — `MOV 15-5 | CC 18 | BS 12 | PH 12 | WIP 13 | ARM 3 | BTS 6 | W 2 | S 2`. Irregular; Technorganic, Climbing Plus, Specialist Operative.

**Option:** `19/0`, Adhesive Launcher Rifle, Flash Pulse, E/M Grenades, Stun Pistol. No standard Fireteam access.

### Raindancers, Light Assault Company

**ID 1878 · AVA 3 · LI** — `MOV 15-5 | CC 23 | BS 12 | PH 12 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Irregular; Martial Arts L3, Mimetism (-6), Stealth, Religious Troop.

| Pts | SWC | Profile summary | FT |
|---:|---:|---|---|
| 18 | 0 | **RAINDANCER FTO**, SMG, Chain Rifle, Grenades | Team Achilles / Shadow / Dragon |
| 24 | 1 | **RAINDANCER FTO**, Red Fury, Chain Rifle | same |
| 20 | 0.5 | **RAINDANCER FTO**, Contender, BS Attack (+1B) | same |
| 19 | 0 | **RAINDANCER FTO**, Light Shotgun, BS Attack (+1B) | same |
| 23 | 0.5 | Forward Deployment +10, Minelayer, E/M Mine | — |

### Cliff-Jumpers, Extreme Jump Unit

**ID 1879 · AVA 3 · LI** — `MOV 10-10 | CC 16 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Parachutist, Combat Jump (PH=13), Super-Jump, Mimetism (-3).

**Options:** `21/0` Light Shotgun / Heavy Flamethrower / PARA Mine; `23/0` Killer Hacker SMG / Zapper / D-Charges; `22/0` Forward Observer Boarding Shotgun / Flash Pulse / PARA Mine. No standard Fireteam access.

### T-Drones

**ID 510 · AVA 1 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Guided Missile Launcher.

**Option:** `16/1.5`. No standard Fireteam access.

### E-Drones

**ID 741 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. EVO Hacking Device.

**Option:** `17/0.5`. No standard Fireteam access.

### Cube Jäger, Mercenary Recoverers

**ID 956 · AVA 1 · LI** — `MOV 10-10 | CC 16 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Irregular; Parachutist; Paramedic.

**Options:** `15/0` Boarding Shotgun + Monofilament CC Weapon; `18/0` SMG + E/Mitter + Monofilament CC Weapon. No standard Fireteam access.

### Glyph Warcors, Ur Hegemony Journalists

**ID 1873 · AVA 1 · LI** — `MOV 10-10 | CC 11 | BS 9 | PH 11 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Irregular Journalist.

**Options:** `4/0` with 360º Visor; `4/0` with Sixth Sense. Flash Pulse / Stun Pistol. No standard Fireteam access.

### Patroclus, Team Achilles' Shadow

**ID 1850 · AVA 1 · HI** — `MOV 15-10 | CC 22 | BS 13 | PH 13 | WIP 13 | ARM 2 | BTS 6 | W 1 | S 2`. Nanoscreen, Martial Arts L3, NWI, No Cover, Stealth, FT Master.

| Pts | SWC | Profile summary | FT |
|---:|---:|---|---|
| 35 | 1 | Holoprojector; HRL, Pulzar, Smoke Grenades | — |
| 43 | 0 | Holoprojector; MULTI Marksman Rifle, MediKit | — |
| 35 | 0 | **PATROCLUS FTO**, MULTI Marksman Rifle, MediKit | Team Achilles / Shadow |
| 31 | 1.5 | **PATROCLUS FTO**, HRL, BS Attack (+1B) | Team Achilles / Shadow |
| 36 | 1 | **PATROCLUS FTO**, HRL, Chain of Command | Team Achilles / Shadow |
| 40 | 0 | **PATROCLUS FTO**, MULTI Marksman Rifle, MediKit, Chain of Command | Team Achilles / Shadow |

### R-Drones

**ID 511 · AVA 1 · REM** — `MOV 15-15 | CC 13 | BS 8 | PH 11 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Repeater / Flash Pulse support.

**Option:** `7/0`. No standard Fireteam access.

### Ioann Bann, Varangian Dog-Warrior

**ID 1940 · AVA 1 · WB** — Dogface: `MOV 15-10 | CC 22 | BS 11 | PH 14 | WIP 13 | ARM 2 | BTS 3 | W 3 | S 2`; Dog-Warrior form: `CC 23 | PH 16 | ARM 4 | BTS 6 | W 3 | S 6`. Irregular + Impetuous; Berserk, Martial Arts L3, Super-Jump, Transmutation.

**Option:** `30/0`, Chain Rifle (+1B), Viral Tactical Bow, Grenades, AP Heavy Pistol (+1B), AP+T2 CC Weapon. No standard Fireteam access.

## Canonical Fireteam chart

Global standard limits from the pinned Army chart:

- **Core:** 1
- **Haris:** 2
- **Duo:** unlimited (`256` in Army source)

### Team Achilles Fireteams

**Types:** Core, Haris, Duo  
**Source note:** **No Wildcards**.

| Entry | Min | Max | Counts as / restriction |
|---|---:|---:|---|
| ACHILLES | 1 | 1 | Counts as Achilles; mandatory anchor |
| PATROCLUS | 0 | 1 | **FTO only**; counts as Achilles |
| PANDORA | 0 | 1 | Counts as Achilles |
| TEUCER | 0 | 1 | **FTO only**; counts as Achilles |
| DRAKIOS | 0 | 1 | **FTO only**; counts as Achilles |
| KO DALI | 0 | 1 | **FTO-2 only** |
| RAINDANCER FTO | 0 | 1 | FTO profile only |

The sectorial Wildcards (`NEXUS`, `GEARHEAD FTO`) cannot join this pool because the source explicitly says **No Wildcards**.

### Shadow Fireteams

**Types:** Core, Haris, Duo

| Entry | Min | Max | Counts as / restriction | Source required flag |
|---|---:|---:|---|---|
| PATROCLUS | 0 | 1 | **FTO only**, counts as Shadow | `required: true` |
| HARBINGER | 0 | 5 | Counts as Shadow | `required: true` |
| ACHILLES | 0 | 1 | — | `required: true` |
| RAINDANCER FTO | 0 | 2 | Counts as Shadow | false |
| STEELJAWS | 0 | 2 | Counts as Shadow | false |
| BLUR | 0 | 1 | Optional Spec-Ops only | false |

The three `required: true` rows are preserved as a **required-choice set**: a legal Shadow team must use the chart's foundation choice semantics, not all three entries simultaneously.

### Research Fireteams

**Types:** Core, Haris, Duo

| Entry | Min | Max | Counts as / restriction |
|---|---:|---:|---|
| PANDORA | 1 | 1 | Counts as Research; mandatory anchor |
| ACHILLES | 0 | 1 | — |
| STINGER | 0 | 3 | Counts as Research |
| WRAITH-1 | 0 | 1 | **FTO only** |
| STEELJAWS | 0 | 2 | — |
| BLACKHEART | 0 | 2 | — |

### Harbingers Fireteams

**Types:** Core, Haris, Duo

| Entry | Min | Max | Counts as / restriction |
|---|---:|---:|---|
| HARBINGER | 1 | 4 | Mandatory anchor |
| ACHILLES | 0 | 1 | — |
| WRAITH-1 | 0 | 2 | **FTO only**, counts as Harbingers |
| TEUCER | 0 | 1 | **FTO only** |
| KO DALI | 0 | 1 | **FTO only**, not FTO-2 |
| BLACKHEART | 0 | 1 | — |
| BLUR | 0 | 1 | Optional Spec-Ops only |

### Dragon Fireteams

**Types:** Core, Haris, Duo

| Entry | Min | Max | Counts as / restriction |
|---|---:|---:|---|
| DRAKIOS | 1 | 1 | **FTO only**, counts as Dragon; mandatory anchor |
| ACHILLES | 0 | 1 | — |
| RAINDANCER FTO | 0 | 3 | Counts as Dragon |
| IRONSIDE | 0 | 2 | Counts as Dragon |
| STEELJAWS | 0 | 2 | Counts as Dragon |

### Heavies Fireteams

**Type:** Duo

| Entry | Min | Max | Restriction | Source required flag |
|---|---:|---:|---|---|
| JUGGERNAUT | 0 | 2 | — | `required: true` |
| IRONSIDE | 0 | 2 | — | `required: true` |
| STEELJAWS | 0 | 1 | — | false |
| BLACKHEART | 0 | 1 | — | false |
| KO DALI | 0 | 1 | **FTO only**, not FTO-2 | false |

Juggernaut and Ironside form a required-choice set.

### Control Fireteams

**Types:** Haris, Duo

| Entry | Min | Max | Counts as / restriction | Source required flag |
|---|---:|---:|---|---|
| UNIDRON | 0 | 2 | — | `required: true` |
| STEELJAWS | 0 | 2 | Counts as Tekdraken | `required: true` |
| BLACKHEART | 0 | 2 | Counts as Tekdraken | `required: true` |
| M-DRONE | 0 | 1 | — | false |
| KO DALI | 0 | 1 | **FTO only**, not FTO-2 | false |

The three required rows are a required-choice set.

### Wildcards

| Entry | Min | Max | Counts as / restriction |
|---|---:|---:|---|
| NEXUS | 0 | 2 | Counts as **Unidron** and **Harbingers** |
| GEARHEAD | 0 | 1 | **FTO profiles only** |

Wildcards apply to legal standard Next Wave Fireteams **except Team Achilles**, whose chart explicitly says `No Wildcards`.

## Reverse Fireteam access index

| Troop / profile | Pool | Types | Max | Notes |
|---|---|---|---:|---|
| Achilles | Team Achilles / Shadow / Research / Harbingers / Dragon | Core, Haris, Duo | 1 | Team Achilles anchor; Shadow required-choice |
| Patroclus FTO | Team Achilles / Shadow | Core, Haris, Duo | 1 | **FTO profiles only** |
| Pandora | Team Achilles / Research | Core, Haris, Duo | 1 | Mandatory Research anchor |
| Teucer FTO | Team Achilles / Harbingers | Core, Haris, Duo | 1 | **FTO profile only** |
| Drakios FTO | Team Achilles / Dragon | Core, Haris, Duo | 1 | **FTO profiles only**; mandatory Dragon anchor |
| Ko Dali FTO-2 | Team Achilles | Core, Haris, Duo | 1 | **FTO-2 only** |
| Ko Dali FTO | Harbingers / Heavies / Control | Core/Haris/Duo as allowed by pool | 1 | **FTO only**, not FTO-2 |
| Raindancer FTO | Team Achilles / Shadow / Dragon | Core, Haris, Duo | 1 / 2 / 3 | Profile-specific |
| Harbinger | Shadow / Harbingers | Core, Haris, Duo | 5 / 4 | Shadow required-choice; dedicated team anchor |
| Steeljaws | Shadow / Research / Dragon / Heavies / Control | Varies | 2 | Control required-choice; Heavies max 1 |
| Blackheart | Research / Harbingers / Heavies / Control | Varies | 2 | Control required-choice; other pools lower caps |
| Stinger | Research | Core, Haris, Duo | 3 | Counts as Research |
| Wraith-1 FTO | Research / Harbingers | Core, Haris, Duo | 1 / 2 | **FTO profile only** |
| Ironside | Dragon / Heavies | Core, Haris, Duo / Duo | 2 | Heavies required-choice |
| Juggernaut | Heavies | Duo | 2 | Required-choice foundation |
| Unidron | Control | Haris, Duo | 2 | Required-choice foundation |
| M-Drone | Control | Haris, Duo | 1 | — |
| Nexus | Wildcard | Any legal standard team except Team Achilles | 2 | Counts as Unidron / Harbingers |
| Gearhead FTO | Wildcard | Any legal standard team except Team Achilles | 1 | **FTO profiles only** |
| Blur Spec-Ops | Shadow / Harbingers | Core, Haris, Duo | 1 | Optional mode only |

All standard roster entries absent from this reverse index have no Fireteam access in the pinned Next Wave chart.

## Reinforcement Fireteams — The Exrah Comissariat

Linked Reinforcement army: **The Exrah Comissariat (Army ID 699)**, source revision `7.26246.158`.

The Reinforcement source exposes global `fireteamChart.spec` values of **Core 0; Haris 0; Duo 0**, while its team rows explicitly declare Fireteam types. Both facts are preserved rather than inventing non-zero global caps.

### Reinforcement roster index

| Unit | ID |
|---|---:|
| Reinf. Nexus Operatives | 1619 |
| Reinf. WCD Base Operators | 1614 |
| Reinf. T-Drones | 1623 |
| Reinf. Q-Drones | 1622 |
| Reinf. M-Drones | 1621 |
| Reinf. WCD Void Operators | 1613 |
| Reinf. EXOs, Exrah Executive Officers | 1615 |
| Reinf. Caskuda | 1618 |
| Reinf. Umbra Legates | 1620 |
| Reinf. WCD Vector Operators | 1612 |
| Reinf. Special Operative Ko Dali | 1616 |
| Reinf. Slave Drones | 1617 |

### Void Reinforcement Fireteams

**Types explicitly listed by Army:** Duo, Haris

| Entry | Min | Max |
|---|---:|---:|
| VOID OPERATOR REINF | 1 | 3 |
| VECTOR REINF. | 0 | 1 |
| NEXUS REINF | 0 | 1 |

### Base Reinforcement Fireteams

**Types explicitly listed by Army:** Duo, Haris, Core

| Entry | Min | Max |
|---|---:|---:|
| BASE OPERATORS REINF | 1 | 5 |
| VOID OPERATOR REINF | 0 | 2 |
| NEXUS REINF | 0 | 1 |

### Caskuda Fireteam

**Type explicitly listed by Army:** Duo

| Entry | Min | Max |
|---|---:|---:|
| CASKUDA REINF | 1 | 1 |
| BASE OPERATORS REINF | 0 | 1 |

### Reinforcement Wildcards

| Entry | Max | Counts as / note |
|---|---:|---|
| EXO REINF | 1 | Base Operator / Void Operator |
| M-DRONE REINF | 2 | — |
| KO DALI REINF | 1 | — |

## Validation notes

- Standard roster count reconciled to **35** ordinary Next Wave entries after excluding optional `BLUR SPEC-OPS`, optional `NEXUS-7 SPEC-OPS`, optional `NEXT WAVE TEAM-OPS`, and generic empty-faction `merc-*` catalogue entries.
- Next Wave Army metadata is current and not marked discontinued in the pinned source.
- Global Fireteam limits reconcile to **Core 1 / Haris 2 / Duo unlimited** (`256`).
- The full standard chart is represented: Team Achilles, Shadow, Research, Harbingers, Dragon, Heavies, Control, and Wildcards.
- `Team Achilles Fireteams` explicitly prohibit Wildcards and this exception is preserved.
- Profile-specific access is preserved for Patroclus FTO, Teucer FTO, Drakios FTO, Ko Dali FTO/FTO-2, Raindancer FTO, Wraith-1 FTO, and Gearhead FTO.
- Ko Dali's `FTO-2` access is confined to Team Achilles; her ordinary `FTO` profile is the one charted in Harbingers, Heavies, and Control.
- Multiple `required: true` rows in Shadow, Heavies, and Control teams are preserved as required-choice sets rather than incorrectly made cumulative.
- Cross-faction ordinary entries with explicit faction `605` membership—Ruby Monday, Cube Jäger, and Ioann Bann—remain in the standard roster.
- `NEXUS-7 SPEC-OPS` and `NEXT WAVE TEAM-OPS` have no row in the pinned standard Fireteam chart; no Fireteam access is invented for them.
- Linked Reinforcement army resolves to **The Exrah Comissariat (699)**. Its chart is kept separate, including the source combination of global `spec` 0/0/0 and explicitly typed Fireteam rows.
- Source data and Fireteam normalization were rechecked on **2026-10-15** against the pinned Army snapshot and InfinityDB commit listed in the front matter.

## Expanded Next Wave tactical guide (2026-10-23)

See the [Next Wave N5.3 tactical and profile-selection guide](../../notes/factions/next-wave.md) for research-backed hero/team tradeoffs, Cyberplug, Juggernaut/Skyhound, specialist coverage and podcast disagreements. **FTO Patroclus has no Smoke Grenades in the pinned profiles**; only the separate Holoprojector HRL option does. Team Achilles excludes Wildcards; use this roster/chart above for actual link legality.

## Command-unit apex/value cross-reference (2026-10-23)

**Harbinger LT 13/0 + plausible decoy** is efficient when Next Wave needs Blackhearts, Gearheads and objective pieces more than a premium LT. **Pandora CoC 29/0.5** can be worth the cost for Research/Hacking/succession simultaneously; **Patroclus FTO CoC 36–40** supplies Fireteam Master/real assault support as a different, more exposed backup. **Stinger NCO** and **Ironside/Juggernaut TacAware** produce **personal or linked Tactical activations**, not transferable generic Orders; Blackheart/Steeljaw Irregular orders require legal Fireteam Master conversion.

See [cross-game Lieutenant, CoC and Order-economy tiers](../../notes/list-building/command-units-apex-and-value.md). **Current pinned profiles and Fireteam chart above govern legality.**

## N5.3 mission specialists — apex/value decisions (2026-10-23)

**Harbinger FO13 / Commlink+1 SO15** supplies low-cost Regular buttons/mission infrastructure alongside cheap 13pt LT+decoy. **Pandora CoC29/.5** can score while supplying Research/hacking if team use is legal; a pricey **Achilles/Ironside/Juggernaut** gun is not automatically a Specialist because it escorts one. **Blackheart/Steeljaw Irregular** require appropriate Fireteam Master interaction before counting link economy. Prefer two independent scorers when big hero team is exposed.

[Cross-game Mission Specialists / Button Pushers tiers](../../notes/list-building/mission-specialists-and-button-pushers-apex-value.md). The current faction profile and Fireteam reference above controls legality.

## Airborne and enemy-DZ attack choices — N5.3 (2026-10-23)

**Ko Dali 37/0 Combat Jump/Parachutist** is a genuine aerial strike; the **34pt FD+20** and 33/30pt FTO variants **do not inherit that AD simultaneously**. **Void Operator NCO or Ironside/Juggernaut fast attack** can exploit command Orders or self movement without being Combat Jump troops. **Harbinger LT13 + decoy** is cheap on-table command, not itself a rear-drop attacker; **Pandora CoC29/.5** is protected backup/support when chosen. Don't assume **Caskuda** legal unless Next Wave roster explicitly lists it (and its TauAware never becomes a generic Regular pool Order).

See [current cross-game apex/value, landing odds and expected-trade tiers](../../notes/list-building/airborne-and-enemy-dz-attackers-apex-value.md). **This roster and Fireteam chart control exact loadout/availability.**

## Active-turn gunfighter cross-reference (2026-10-23)

**Active-turn shooting choices:** **Skyhound33/0** is an outstanding **non-TAG aerial** BS14/Mimetism(-6) plasma/AP angle-maker when vertical terrain works; S7, No Cover and Repeaters punish its exposure. **Stinger HMG30/1** supplies cheap long-range backup; **Achilles** dominates a cleared close-assault route but does not need to take the first unfavorable FtF. **Borderbash 2026 winning discussion:** clear Mimetism and hostile hacking with other units before committing the expensive assault package. [Non-TAG and TAG value tiers, transcript evidence](../../notes/list-building/active-turn-gunfighters-apex-and-value.md).

## Warbands and cheap high-upside trading — N5.3

**Tekdraken Steeljaw18/0 (Sensor/Viral Mine) and Blackheart25/0 (Panzerfaust/E/Marat/Mine Dispenser)** offer **Irregular multiwound close-control and technical disruption**, not generic 5pt Chain Rifle warbands. **Blackheart27/.5 Plasma Carbine** has different cost/role. Some legal Fireteam Master/Commlink setups may change local Order utility; do not count their Irregular as pooled Regular without actual pinned skill and team conditions. Preserve **Harbinger LT13** and **Pandora CoC29/.5** separately from these traders.

[Current cross-game warband apex/value, target counters and LT/CoC tiers](../../notes/list-building/warbands-and-cheap-trading-units-apex-value.md). Pinned profile choices and canonical Fireteam chart in this roster remain authoritative.

## TAG tactical cross-reference (2026-10-23)

**Juggernaut (78–82)** is a high-commitment 20–5, ARM8, Climbing Plus, Guard/TacAware assault anchor; **NCO MULTI HMG** is best when an unused LT Order exists, while the plasma/HRL choice supplies a different close/mid-range angle. At this price, preserve enough independent specialists and screening pieces to protect its rear; its peak damage does not imply elite points efficiency.

Across all factions, compare **apex power** separately from **points value**, counterplay and mission fit: [N5.3 TAG guide](../../notes/list-building/tags.md). The current unit profiles and canonical Fireteam chart above take precedence over tactical opinions.

## Vehicle (VH) tactical cross-reference (2026-10-23)

**Skyhound AVA1:** **33/0 BS14 + Mimetism(-6), Plasma Carbine(+1B), AP Thunderbolt(+1B), Mine Dispenser** is arguably the strongest *raw value* flying shooter; **31/0 MULTI Rifle/Flammenspeer** gives up much of its advantage to save 2 points. **Shepherd (Oct 2025)** ranked it #3/8 counting Garuda because **Next Wave lacks cheap resilient support/backup**, not because the loadout is weak. **MetaChemistry #132** describes devastating plasma but an enemy Pitcher+Isolate neutralized it. Supply KHD/repair/exact jump LoF and safe exit; **no Fireteam rights**.

See [VH apex/value tier list and matchup guide](../../notes/list-building/vehicles-vh.md). **Current profiles, AVA and canonical Fireteam chart above remain authoritative.**

## Hacker and KHD tactical cross-reference (2026-10-23)

**Cheap cyber investment:** **Harbinger KHD + Deployable Repeater 17/0** is a low-SWC anti-Hacker/counterattacker; **Harbinger HD + Minelayer 18/0.5** brings Spotlight/Oblivion to ordinary heavies. **Gearhead FTO Hacker + Pitcher + Firewall(-6) 19/0.5** projects the network from a protected legal team; **Contrabandolero HD 29/0.5 vs KHD 27/0** is costlier mobile mission utility, and **Ironsides KHD34/0** buys armor/fighting. **Why:** Next Wave's Skyhound and pricey higher-end pieces need a *cheap complementary network*; an expensive solo KHD does not protect the vehicle from non-Hacker Oblivion unless enemy cyber threats can actually be engaged. Limit redundant hackers when losing one combat specialist already threatens list functionality.

See the [cross-game apex/value Hacker/KHD tier guide](../../notes/list-building/hackers-and-killer-hackers.md). **The sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative; device upgrades are profile-specific.**


## Cheerleader / Order-generation tactical cross-reference (2026-10-23)

Cross-faction [apex and cost-value Order-generator rankings](../../notes/list-building/cheerleaders-and-order-generators.md), circumstance guide and transcript disagreements. **This file remains authoritative for profiles, AVA, Training and Fireteam legality.**

- 7pt R-Drone — cheap transferable Order, Repeater and Flash ARO; uses S3 space and AVA.
- 11pt Ikadron — Regular Baggage/Repeater with 2 light-flamethrower shots; guards lanes better than a bare beacon.
- Unidron — more expensive than a Flash REM but adds plasma and a Fireteam body; pay for that specific work.
- Warcor — Irregular Flash Pulse ARO distraction, NOT a passive transferable Regular Order.
- Baggage — prioritize a legal 8pt basic bot if actually on roster, remembering its large base.

**When to pick:** Prefer transferable, safe Regular Orders when the Combat Group needs fuel; choose the higher-priced option only when its smoke, template, weapon, repeater, Fireteam function or scoring ability has a real job. Do not count Irregular/Impetuous/Tactical/Lieutenant Orders or Peripheral bodies as interchangeable Regular pool Orders; account for DZ footprint and link/enabler package costs.


## ARO apex/value cross-reference (2026-10-23)

The [N5.3 cross-faction ARO apex/value and matchup study](../../notes/list-building/aro-units-apex-and-value.md) compares hidden missile traps, Neurocinetics/TR, cheap templates/mines, DZ guards and conflicting creator opinions. Consult the **roster and Fireteam chart above** for legally available profiles, SWC, Training and AVA.

- **Q-Drone TR Thunderbolt** — 20pt/0.5SWC and Mimetism(-3), useful reactive presence with Engineer support; won't solo elite active guns
- **R-Drone Flash** — 7pt regular + Repeater and reactive stun threat; value is Order+network+minor tax, not a durable lane
- **Warcor Flash** — 3pt Irregular ARO tax/late-game Stun attempt, not a Regular Order
- **Ikadron Baggage/Flamethrower** — cheap multi-purpose DZ corner guard and Repeater; contributes more than pure filler without being a long gun

**Practical deployment:** put cheap disposable/Flash/DTW or mine pressure on the approach; retain a separate unseen or recoverable threat for the decisive square; avoid exposing a premium active attacker and check opponent Smoke, MSV, hacking, AD and pie-slicing. No automatic order from an off-table Hidden model; Irregular ARO units do not supply generic Regular Orders.

## Doctor / Engineer / Recovery cross-reference (2026-10-23)

**Med-Tech21** covers Doctor and Engineer behind forward **Achilles / Skyhound** pressure; **Slave Drones3** should be staged on different routes rather than stacked. **Gearhead Engineer/Cyberplug** can project support through an independently placed connected body, but **Cyberplug and Servant attachments cannot both be fielded on the same Controller**. Aerial **Skyhound** needs safe ranged GizmoKit/repair access, not assumed easy contact. [Doctor/Engineer apex/value, odds and media disagreement](../../notes/list-building/doctors-engineers-and-recovery-apex-value.md).

## Close-combat assassins and counter-CC — N5.3 (2026-10-23)

**Achilles AP Spitfire62/1.5 or Plasma63/0** is the **3W CC24/MA4 EXP** fighter who can shoot his own approach and keep attacking; the team costs more and must manage enemy hacking/E/M. **Patroclus35 FTO** contributes mobility/team support and MA3/CC22 as a *secondary* melee body; it is not another Achilles. **Skyhound** wins by aerial firing angles, not CC. **Med-Tech/Slave** supports recovery after retreat; do not fund a 60pt fighter purely to kill one 10pt defender. [Dedicated CC assassin apex/value, delivery and counter-CC](../../notes/list-building/dedicated-close-combat-assassins-apex-value.md).

## N5.3 network projection — Pitchers, Repeaters, TinBots and disposable delivery

**Bit & KISS!** supplies native-KISS / pitched / deployable Repeater delivery on the matching profile (check current Next Wave option); **Gearhead FTO hacker+Pitcher19/.5** is a cheap Fireteam-enabled projector with printed Firewall(-6), different from TinBot(Repeater). **R-Drone7/0**, **Ikadron11/0**, **M-Drone Sensor/FO/Repeater** are the inexpensive actual native nodes; **Harbinger KHD+Deployable Repeater17/0** places a node after activation, not a Turn-0 Minelayer unless the exact selected profile says so. **Counter:** do not buy multiple cyber support devices if Next Wave's high-speed direct fire resolves the critical target without hacking; risk of enemy counterhacking rises with exposed repeaters.

[Whole-game network projection: apex/value, current profiles, and opposing transcript views](../../notes/list-building/network-projection-repeaters-pitchers-apex-value.md).

## N5.3 rare abilities & unusual combinations — tactical synthesis

**Gearhead Cyberplug13/0** is a truly different N5.3 peripheral model: **Connected** (controller Idles for most declared actions) versus **Autonomous** (can spend pooled Orders and make independent ARO), chosen at start of Order/ARO; max one connected Cyberplug at a time. **Sartroid Puzzlers** have separate connected/autonomous profiles, not standard synchronized Servants. **Ko Dali FD34/0 vs Combat Jump37/0** is Protheion+MSV2+Specialist; special **FTO33/0 vs FTO-2 30/0** are explicitly different team permissions. **Drakios Albedo(-6)+Bangbomb+2W+Kydoimos peripheral37–39/0–1** creates paired assault, but **FTO31–33 no Kydoimos**; strong against enemy MSV, weaker when no visors and no secondary peripheral lane. **Opposing philosophy:** Cyberplug independent utility vs ordinary cheap engineer and direct Skyhound/Ironsides assault; test actual group Orders before paying for rare architecture.

[Cross-faction rare abilities apex/value, mechanics, and MCP source debates](../../notes/list-building/rare-capabilities-and-unique-combinations-apex-value.md). Current roster/Fireteam profile tables above are authoritative.

## Anti-TAG / Anti-HI without hacking — N5.3 (2026-10-23)

**Sartroid Puzzler E/Marat + Adhesive13 or E/Marat+Akrylat12** is cheap **Peripheral(Cyberplug)** anti-TAG control, but generates **no Order of its own**; count legal controller activation. **Unidron14 K1 Combi**, **Blackheart Tekdraken25 Panzerfaust+E/Marat / 29 E/M Carbine**, and **Cube Jäger15 Mono/18 E/Mitter+Mono** cover ranged, state and assassin roles. **Ironside44 AP HMG**, **Skyhound33 AP Thunderbolt** or **Teucer35 Feuerbach** give stronger sustained armor damage for more list resources. [Cross-game anti-armor apex/value, E/M and AP+EXP guide](../../notes/list-building/anti-tag-anti-heavy-infantry-non-hacking-apex-value.md).

## N5.3 objective holding, zone domination & carried-objective choices

**Next Wave** favors **Skyhound33/0** to clear/guard high ground (2W Mimetism(-6), No Cover S7 Aerial) and **Ironsides HI** to occupy dangerous scoring zones, with a **separate actual Specialist**. **Ko Dali Combat Jump37/0 or FD34/0** is eligible Specialist+MSV2+Protheion, strong *late pickup* if arrival and exit safe; FTO/FTO-2 lose distinct deployment tools and are not interchangeable. **Sartroid/Puzzler Cyberplug** distributed connected/autonomous body can guard separated approach lanes, but its actual Cost/Null behavior decides zone VP; **Gearhead13/0** is not a free extra scoring body for every bot. **Borderbash 2026 winner:** cheap Ikadron or comparable Baggage units flipped *Superiority* because mission added points; don't copy bonus to ordinary Domination. Counter: Skyhound isn't a box carrier and No Cover makes its aerial zone occupation risky.

[Cross-game zone-holder and carrier apex/value, mission rules, and opposing transcripts](../../notes/list-building/objective-holding-zone-domination-and-carriers-apex-value.md). Current local roster/FT chart is authoritative.

## Force multipliers — N5.3 role/value cross-reference (2026-10-23)

**FT Masters**: Pandora24–29/.5 (Stingers), Patroclus FTO31–40, Drakios FTO31–33 regularize the **Irregular members in their legal teams** at Order Count; don't inherit every team or optional non-FTO profile. **Gearhead Cyberplug13/0** with a **Puzzler12–13** costs **25–26pts combined**; connected/autonomous chosen on each Order/ARO under N5.3 and Puzzler has no Order. Ikadron/Echodron Baggage supports dispenser/Pitcher ammunition, not Non-Reloadable deployed turrets. Shepherd and LoL praise these dependencies; MetaChemistry recommends targeting FT Masters and Gearhead controllers to collapse support efficiency. [Global tiers](../../notes/list-building/force-multipliers-special-abilities-apex-value.md).

## Anti-Tech — enemy visors, Mimetism, markers and Impersonation (2026-10-23)

**M-Drone Sensor/FO/Repeater/Triangulated Fire** and **Tekdraken Steeljaw18/0 with Sensor** are the value **Camo/Hidden** hunters (different mobility, cost and Order structure). **Ko Dali MSV2** and rostered **MSV2 gunfighters** clear actual Mimetism shots; **Ironsides Albedo(-3)** and other Albedo(-6) profiles punish enemy MSV/Marksmanship *only* when it exists. **Counter:** an Albedo gun is not concealed versus plain HMGs. Buy Sensor to reveal clustered Camo first, then a separate high-Burst gun; don't spend the entire Turn just discovering one disposable marker.

[Non-hacking & tech-specific counter-selection, N5.3 anti-tech apex/value and opposing MCP transcripts](../../notes/list-building/anti-tech-msv-mimetism-camo-impersonation-apex-value.md).

## N5.3 peripheral / synchronized / multi-body apex-value update

**Cyberplug apex:** **Gearhead Cyberplug13/0 + 2 Puzzler Akrylat12/0=37/0** (one25/0). Two infiltrating **ARM3/BTS6 E/Marat + adhesive** Sartroids with **Connected BS12 vs Autonomous BS10** and 20-5 vs 15-10 MOV: **one Connected, one Autonomous** each Order. Autonomous spends **pooled Orders**, may independently ARO, **does not generate Order**; after Gearhead dies/Isolated, both Autonomous **not inert**. **Reactive exception:** when Gearhead takes its own ARO, **both Cyberplugs may independently ARO as Autonomous**; selecting one Connected instead makes the Gearhead Idle. This is three potential legal reacting bodies, **not three Order generators**. **Ranter SMG+Thunderbolt12/0** alternatively gives FD(+10), Mimetism(-6), **Connected BS13/Autonomous BS11**, better midrange gun but generally weaker covert/EM denial. **Two Gearheads and 4 Sartroids** has two different controllers and actual **full package cost**, not 4×12px. **Bit+KISS!** is separately standard synchronized, no Cyberplug autonomy. **Shepherd N5 review:** Puzzler/2 stronger in almost any normal list than pricier Ranter; counter-argument is Saturation/neutralization and lack of pooled Regular Orders in short mission with few cyber targets.

[Whole-game N5.3 Peripheral & Multi-Body Apex/Value guide](../../notes/list-building/peripheral-synchronized-multibody-apex-value.md). Exact current roster, dependency and Fireteam chart above override commentary.

## Battle-report effectiveness and combinations (qualitative, 2026-11-01)

**Supported combinations:** **Achilles + Harbingers + Pandora/hacker + Puzzlers/Repeaters**, with **Blackheart/Stinger/Skyhound** as another angle, succeeded when missions specifically rewarded a **Key Ops** centerpiece (#001/#156 same event context, #165 a separate winner). **Harbinger FOs and defensive Puzzler adhesive/E/M** kept the list from being only a hero gunline; #165's alternative **Steeljaw-heavy Defensive Dinos** claimed Battleground/Hardlock zones instead of chasing kills. [#001](../../notes/battle-reports/001-010-n5-battle-report-tactical-analysis.md) · [#156](../../notes/battle-reports/151-160-n5-battle-report-tactical-analysis.md) · [#165](../../notes/battle-reports/161-170-n5-battle-report-tactical-analysis.md).

**High-profile failures:** #197's overextended Achilles was locked by **Tunguska Interventor/Kulak/Cybermine**; #239's Next Wave Skyhound/Stinger offense damaged O-12 but lacked necessary Hacker/mission coverage and lost **Area of Interest 4–2**. [#197](../../notes/battle-reports/191-200-n5-battle-report-tactical-analysis.md) · [#239](../../notes/battle-reports/231-240-n5-battle-report-tactical-analysis.md).

**Decision rule:** Choose **Achilles for a defined scoring job**, not because elite kills look impressive; build a second specialist route, recoverable denial and anti-repeater option. No retrospective win implies a universal Achilles auto-include.

[Cross-report synthesis and evidence cautions](../../notes/battle-reports/cross-report-unit-effectiveness-and-combinations.md).

## Mission performance — battle-report evidence (2026-11-01)

| Mission(s) | Tested composition / scoring mechanism | Evidence |
|---|---|---|
| **Cutthroat / Key Ops** | Achilles + Patroclus/Juicer + Harbingers/Pandora/Puzzlers used for high-value assault in tailored packets; not a generic compulsory include. | [#001](../../notes/battle-reports/001-010-n5-battle-report-tactical-analysis.md), [#156](../../notes/battle-reports/151-160-n5-battle-report-tactical-analysis.md), [#165](../../notes/battle-reports/161-170-n5-battle-report-tactical-analysis.md) |
| **Battleground / Hardlock / Corporate zone holding** | Alternative Defensive Dinos: multiple Steeljaws + Harbinger/Wraith specialists and Patroclus/Drakios held zones rather than pursue kills. | [#165](../../notes/battle-reports/161-170-n5-battle-report-tactical-analysis.md) |
| **Provisioning / frontline objectives** | Skyhound/Stinger/Steeljaw gun and mine pressure with Puzzler/Harbinger specialists; retain objective workers. | [#187](../../notes/battle-reports/181-190-n5-battle-report-tactical-analysis.md) |

**Limits:** #001 and #156 cover one event. #197 and #239 show Achilles/fast vehicles losing mission value to hacking or insufficient objective bodies. Game-era qualitative evidence, not a win-rate or current Fireteam claim. [Full mission evidence audit](../../notes/battle-reports/cross-report-mission-performance-by-sectorial.md).

## Counterplay — observed N5 battle-report responses (2026-11-02)

| Threat / target | Observed response and limitation | Battle reports |
|---|---|---|
| **Defensive Fireteams / edge pressure** | Achilles/Patroclus plus Puzzler/Harbinger network threatened forward HI; alternatively four Steeljaws/Harbinger-Wraith ‘Defensive Dinos’ saturated Battleground and hard zones. | [#165](../../notes/battle-reports/161-170-n5-battle-report-tactical-analysis.md) |
| **Against Camo gunlines** | Skyhound/Stinger and Puzzler/Tech Dragon can reach markers from odd ranges, but Shasvastii quad-Shrouded+Dazers retained Area of Interest zones; more guns were insufficient. | [#196](../../notes/battle-reports/191-200-n5-battle-report-tactical-analysis.md) |
| **Counter-counterplay: hackers and hidden mines** | Overextended Achilles was isolated/IMM'd by Tunguska Interventor/Kulak/Cybermines, 7–3; O-12 cheap Razor/Gangbuster/Moonraker Camo and cyber contest outscored Next Wave 4–2. | [#197](../../notes/battle-reports/191-200-n5-battle-report-tactical-analysis.md), [#239](../../notes/battle-reports/231-240-n5-battle-report-tactical-analysis.md) |

**Limit:** #165 reports distinct mission lists; do not mash both archetypes into one illegal or unaffordable roster. These are historical qualitative interactions, not present N5.3 unit, Fireteam, or win-rate claims. [Full cross-report counterplay analysis](../../notes/battle-reports/n5-cross-report-counterplay-tags-hi-hacking-camo-impersonators-fireteams.md).

---

## Must-have / Go-to / Avoid — source-backed recommendations (2026)

Dated source-backed tactical preferences and miniature purchasing priorities; opinions do not override N5.3 roster, profile or Fireteam data above.

**Original audit title:** Combined Army — must-have, go-to and avoid audit (N5.3, 2026-10-23)

**Scope:** Vanilla Combined Army, Morat Aggression Forces (MAF), Shasvastii Expeditionary Force (SEF), Onyx Contact Force (OCF), Next Wave. The user-defined categories are deliberately demanding: **must-have** = an almost-every-list personal default reported by a speaker or genuinely indispensable faction engine; **go-to** = broadly good when assigned a sensible role; **never take / avoid** = profile-level displacement or explicit speaker rejection, **not** proof of mathematical domination. An empty hard-veto category is more accurate than inventing one.

**Factual authority:** the five [current repository sectorial reference files]() (all `status: current`, N5.3, Army `7.26246.158`, changed 2026-09-03), then [rules](../../rules/README.md). These establish **legality, costs and loadouts**, while videos/podcasts establish **opinions and observed results**. Earlier N4/2025 advice cannot override the current roster. [Official N5.3/ITS18 changes](https://infinityuniverse.com/en/news/infinity-rules-update-5-3) include updated Team-Ops/Spec-Ops and Sāchā availability. Normal-list recommendations do **not** silently assume optional Team-Ops.

**Evidence key:** **Direct** = attributable preference or rejection from a full transcript checked for this audit; **Corroborated** = source discussion + existing reviewed guide; **Contested** = sourced counter-opinion exists; **Edition-limited** = pre-N5.3 material must be interpreted using current reference. “Near-must” is still **not a mandatory unit**.

### Quick comparison

| Army | Strongest near-default evidence | Go-to engines | Credible profile-level avoid | Absolute unit veto? |
|---|---|---|---|---|
| **Vanilla** | Dāturazi Smoke; Bit & KISS **KISS Pitcher** option; Libertos Mine layer (all speaker-personal, not all mandatory) | Vector + Unidrons, Legate HD+, Sheskiin, elite Aspects | Umbra Legate LT, non-LT Charontid if LT version fits, wrong Bit & KISS for network projection | No |
| **Morats** | Dāturazi or **alternative** Smoke engine; no uncontested individual compulsory purchase | Sogarat LT/NCO, Yaogat MSV2, Dartok FTO, Oznat/Hungries | Yaogat Combi/Panzerfaust or BSG/Panzerfaust as default shooters; unbalanced double-Krakot team | No |
| **Shasvastii** | **None universal**: 2026 winner reports distinct sneak and face-up lists | Speculo, Caliban, Shrouded, Noctifer, Sheskiin, Mentor, Gwailo/Victor | Cadmus KHD over basic BSG **for a pure assassination/drop role** | No |
| **Onyx** | No uncontested must: 2026 hosts **disagree on Unidron quantity** | Nexus + Unidrons, Bit & KISS, Overdron, Xeodron/Nourkias, Noctifer | Void Operators as default generic team fillers; generic Suryat gun package when it crowds out Onyx tools | No |
| **Next Wave** | **Pandora** (Shepherd says every list); **Gearhead + Puzzler** near-core in disruption builds | Blackheart, Stinger, Harbinger specialists, Wraith FTO, Skyhound/Ironside | Harbinger HMG/ML, Wraith Hidden MULTI Marksman, naked Gearhead Engineer over useful alternatives | No |

### 5. Next Wave

**Sources:** [Robert Shepherd, *N5 Next Wave faction focus*, Dec 2025](https://www.youtube.com/watch?v=52aFgWpv8es) (**full transcript rechecked**); [Tactical Awareness, E36 Next Wave](https://open.spotify.com/episode/1c9pgE6IkthlQ2mzQpH4Qe) (full transcript rechecked); [Loss of Lieutenant E172, *List Building 101: Next Wave*, Aug 2026](https://open.spotify.com/episode/5cVwqFnBxM9xYIskCHHuDt) (full transcript rechecked); [MetaChemistry E148 opposing Next Wave](https://open.spotify.com/episode/3X6yHHjjJNYmZVO8qltsUZ) and [existing guide](../../notes/factions/next-wave.md); [N5.3 roster](next-wave.md).

**Near-must / genuine speaker defaults**
- **Pandora 24–29/.5** — **Direct strongest:** Shepherd expressly says he puts her in **every Next Wave list**, praises durable Zero Pain defensive hacking, specialist capability, and Fireteam Master. In an army with thin affordable hacking, multiple roles in one piece matter more than the raw weapon. **Not unconditional:** list/mission exceptions and the desired MediKit/CoC/Pitcher are **different actual loadouts**.
- **Gearhead Cyberplug 13/0 + Sartroid Puzzler 12–13/0 (total package ≥25)** — Shepherd calls the Puzzler a top disruption piece; **Loss of Lieutenant E172 (~17min)** independently argues it may be **Next Wave's best unit**. Hidden/forward E/Marat, PARA/Repeater denial stops TAGs or an aggressive Fireteam before it reaches scoring. **Not two Regular Orders:** Cyberplug controller, connected/autonomous modes and N5.3 Peripheral rules are real costs. It's near-core in disruption lists, not necessarily every rush/TAG list.

**Go-to**
- **Harbinger LT 13 + decoy / FO 13 / hacker/KHD** — indispensable *type of job* (affordable Regular orders, secure command, specialist glue); do not imply a fixed Harbinger loadout mandatory. Current roster allows other plans.
- **Tekdraken Blackheart, and Steeljaw when protecting a hero** — broad all-range threat and mine/E/Marat coverage; Fireteam Master converts **only qualifying** linked Irregular Orders. Don't count peripherals/Tekdrakens as free generic Regular Orders.
- **Stinger MSV2 or HMG based on lanes; Teucer MSV2; Ironside Albedo** — shooting modifiers and anti-MSV/smoke answers; pick complementary rangebands and avoid paying for three redundant premium guns.
- **Wraith-1 FTO 25/.5 + Harbinger Research / support link** — cheap (for this faction) linkable MSV/Mimetism midrange gun; Shepherd calls it standout for freeing 300-point list budget.
- **Sāchā, Contrabandolero, Cliff-Jumper, Skyhound VH, Achilles, Juggernaut TAG** — late scoring, objective deployment, AD flank, fast anti-ARO or centerpiece, depending on mission. **Sāchā AVA changed in N5.3**; no assumption that October 2025 cap still holds.
- **Drakios** — **contested go-to only when needing fast *nonhackable* specialist/Albedo and a particular Fireteam Master.** Shepherd openly dislikes him; **Loss of Lieutenant E172 (~23min)** expressly counters that Drakios has won useful roles and isn't what's wrong with the sectorial. Don't mislabel as universal veto.

**Avoid / explicit transcript negatives, current-profile checked**
- **Harbinger HMG 20/1 and Missile Launcher 18/1.5** — **Direct strongest:** Shepherd says **never** buy either; plain BS11 line-gunner and SWC cost compete badly with Stinger/Blackheart/Wraith/Teucer shooting while Harbinger LT/FO/Hacker provide more useful jobs. Profile-level advice, not condemnation of Harbingers.
- **Wraith-1 27/.5 Hidden Deployment MULTI Marksman** — **Direct:** Shepherd says **do not take** it; the **28/1.5 Hidden MULTI Sniper** better uses hidden surprise/range, while 25/.5 **FTO MMR** buys link value. **Exception:** strict SWC or a specific hidden-midrange corridor.
- **Gearhead plain Engineer 17/0 as a blind pick** — **Direct:** Shepherd says he never takes this profile; **13/0 Cyberplug** buys Puzzler access, while **18/0 Engineer FTO** can Wildcard and repair with a team. Choose Engineer only when its location/team eligibility beats the alternatives.
- **Next Wave Bit & KISS 25/.5 as a network-shooting cornerstone** — **Direct:** Shepherd calls its KISS Repeater version very weak versus the KISS Pitcher configuration found in other armies. **Current roster has ONLY the 25/.5 version in Next Wave**: this is an avoid *for long-range Pitcher work*, not a nonexistent alternate 22pt profile you can select here. Useful local hacking is still possible.
- **Not “never take”: Drakios** (direct conflicting Aug 2026 podcast), **Achilles** (high investment but legitimate), **Juggernaut** (TAG skew), or **Sāchā** (source AVA has changed).

### Confidence rules and conclusion

1. **Strict “never take” labels attach to exact current loadouts**, not to entire units. Use *speaker strongly avoids* rather than declaring a mathematical theorem from one opinion.
2. **Every faction has successful alternative list architectures.** At most a handful of troop choices are speaker-verified near-defaults; in Onyx and Shasvastii, **no individual unit has sufficiently strong all-build consensus**.
3. **Preserve opposing speakers.** Especially: Morat **Sogarat vs Kornak**, Shasvastii **Gwailo and Jayth skepticism vs 2026 winner**, Onyx **Unidron density**, Next Wave **Drakios**, Vanilla **Avatar effectiveness vs list cost**.
4. The roster is **N5.3, September 2026**, but most opinions are earlier; they are tactical heuristics, **not independently updated tournament win-rate data**. The Oct 2026 Onyx review and 2026 SEF tournament testimony receive more weight than older recordings where they conflict.

### Whole-unit purchasing audit — can I skip the miniature? (2026-10-30)

**Whole-unit** here means *every currently legal profile of that named troop in the specified army*, not one disliked loadout. **Defer** is a collection-building recommendation, not a competitive ban; evaluate the same miniature again when playing a different sectorial. **Hard whole-unit avoids: none established by these recordings.**

| Army | Entire model/unit to defer buying? | Why; what would change the answer |
|---|---|---|
| **Vanilla Combined** | **No source-supported whole-unit skip** | The Umbra Legate **LT** and non-LT Charontid criticisms leave useful alternative profiles; Bit & KISS's wrong network loadout does not disqualify its Pitcher configuration. Avatar is *strong but optional*, not bad. |
| **Morat** | **No** | Cheap Yaogat Panzerfaust profiles are disliked, but the MSV2 Spitfire/sniper are positively recommended. Suryat, Kornak and TAGs still have distinct uses. |
| **Shasvastii** | **No** | Cadmus KHD criticism applies to a backline-kill role; the BSG and KHD specialist jobs differ. 2026 results directly contradict blanket Gwailo/Jayth skips. |
| **Onyx** | **Defer Void Operator unless deliberately using its rocket/KHD utility — low confidence** | An [Irregular Order #56](https://open.spotify.com/episode/7b2QJ494pgPp6NY6WQ9QWF) host never preferred it over Base Operator; another defends its unique tools. A *personal* buying deferral, **not** all-profile dominance. |
| **Next Wave** | **No** | Harbinger heavy guns, Wraith hidden MMR, plain Gearhead Engineer and Bit & KISS as a *Pitcher substitute* are the poor choices. Other profiles/uses remain legitimate, so do **not** skip those entire model families. |

**Purchase rule:** consider skipping a full unit only when its *best* viable profile also loses its expected role in your chosen army. A bad SWC weapon or wrong Fireteam configuration does **not** justify avoiding an entire kit. See the [cross-faction buying shortlist](../../notes/factions/model-purchase-avoid-summary-2026.md).

### Worst-value, circumstantial and proxy-first miniature purchases by army (2026-10-30)

**Question:** For **Vanilla Combined Army, Morat Aggression Forces, Shasvastii Expeditionary Force, Onyx Contact Force and Next Wave**, which are the **weakest everyday picks**, most specialized rarely *needed* purchases, or **good units better represented by a proxy before buying an extra miniature**? An **AVA maximum is not a shopping target**. “Rare/circumstantial” below is a *qualitative estimate of how often a particular job arises in the reviewed list plans*, **not a measured tournament pick rate**. The current [N5.3 roster files]() (Army data 3 September 2026) take priority over earlier recordings for exact variants, base/silhouette, unit access and Fireteams.

**Decision labels:** **Defer/skip as a default dedicated miniature** = an explicit reviewer's negative judgment on that *usual role*, with exceptions explained. **Proxy first** = a specialized yet legitimate **inferred purchase priority**, *not* an invented direct quotation. **Avoid profile, NOT unit** = the named loadout/Fireteam plan is poor but other choices are strong. **Proxy the extra** = first copy or alternative sculpt may be a normal good purchase, but redundant physical duplicates need demonstrated simultaneous use. **Contested** = dated contrary opinions, successful tournament use or a distinct current-profile benefit make a universal “worst” label dishonest. **No verified complete-unit all-profile hard ban exists** in the present evidence.

#### 5. Next Wave — most direct weak-profile evidence and debated expensive specialty kits

| Whole model or exact profile | Source basis, replacement and caveat | Buying action |
|---|---|---|
| **Harbinger HMG20/1 or Missile Launcher18/1.5 as ordinary Fireteam gun** | **Direct strongest — [Shepherd Next Wave](https://www.youtube.com/watch?v=52aFgWpv8es) says “never” for these two gun profiles**: BS11 line gun SWC better spent on **Stinger, Wraith FTO, Blackheart, Teucer or Ironside**. **Harbinger LT/Decoy/FO/Hacker** remains important economical order/mission backbone. | **Avoid *these loadouts only*; NOT Harbinger sculpts**. Proxy an occasional gun sculpt; buy enough Harbinger bodies for real LT/specialist/team roles. |
| **Wraith-1 Hidden MULTI Marksman 27/.5 used as default assassin/sniper** | **Direct — Shepherd** calls this **weak compared to its own 28/1.5 Hidden MULTI Sniper** for true hidden-ranged attack, while **25/.5 FTO MMR** is a good link-ready value piece. SWC/range/mission can still favour hidden midrange. | **Avoid *Hidden MMR default profile*; do not skip Wraith FTO**. One suitably sized sculpt can proxy mutually exclusive options; buy second only if genuinely fielded together (AVA2). |
| **Gearhead plain Engineer17 as automatic choice over Cyberplug13 or FTO Engineer18** | **Direct — Shepherd** seldom/never selects naked Engineer when **Cyberplug13 + Sartroid Puzzler** buys major disruption or **FTO Engineer18** has legal Wildcard repair access. Current Puzzlers/Ranters are **Cyberplug peripherals** with **no separate Regular Orders**. | **Avoid naked Engineer *profile* as default; NOT Gearhead**. **Proxy a specialist variant on one Gearhead** and use separate Sartroid models when the chosen profile actually includes them. |
| **Bit & KISS 25/.5 as long-range Pitcher delivery substitute** | **Direct review critique:** Next Wave has **KISS Repeater**, **NOT KISS Pitcher**. The 22/.5 Vanilla option **does not appear** in this sectorial; buying identical-looking minis cannot give the unlisted ability. | **Avoid the *Pitcher-projection plan*, NOT Bit & KISS's local KHD/Rept role**. **Proxy first** if Next Wave's Gearhead/Pandora network already covers all needed control. Model **Bit + KISS** separately. |
| **Drakios as compulsory Achilles escort/main anti-MSV attacker** | **Direct, contested across 2026:** Shepherd is sceptical of extra cost; [Loss of Lieutenant E172 Aug 2026](https://open.spotify.com/episode/5cVwqFnBxM9xYIskCHHuDt) defends Drakios's **nonhackable specialty/Albedo/mobility**, especially into MSV/Repeater opponents. **Dragon family requires Drakios FTO**, so he can be a mandatory *team anchor* in that chosen archetype. | **Proxy-test Drakios first**, especially when you already field Achilles/Ironside. **Not a universal never**; buy for a recurrent anti-MSV/Dragon/mission use. |
| **Juggernaut TAG or second Juggernaut as a default response to every enemy** | **Contested:** high-cost (~80pt) **Guard/armour/Climbing Plus/NCO** offers extraordinary sustained threat, but [Shepherd](https://www.youtube.com/watch?v=52aFgWpv8es) warns its cost hollows the supporting Order/mission plan. [MetaChemistry E148](https://open.spotify.com/episode/3X6yHHjjJNYmZVO8qltsUZ) highlights genuine enemy concern about double Juggernaut. | **Proxy/borrow a TAG-sized model before buying**; **second Juggernaut only for a tested skew** with sufficient Harbinger/Pandora/Engineer support. **TAG, not Vehicle**. |
| **Skyhound S7 Vehicle when it is intended to take Cover or open hard MSV AROs unaided** | **Strong disagreement:** [Loss of Lieutenant E172](https://open.spotify.com/episode/5cVwqFnBxM9xYIskCHHuDt) likes **Plasma/Mine Dispenser** and high-reach angles; Shepherd warns that **S7, No Cover, hackable** flyer has a low survival floor when revealed into an unbroken enemy lane. A fast vertical finisher remains excellent when terrain/Ironside/Drakios enables it. | **Proxy the single specialty VH before buying**, particularly on low-vertical tables. **Not a bad whole model**; a Skyhound isn't a TAG, Overdron or interchangeable flyer in legal Army. |
| **Patroclus bought to throw Smoke while Fireteamed with Achilles** | **Hard current-profile legality trap:** **unlinked 35/1 Holoprojector HRL Patroclus has Smoke**; **FTO linked Patroclus has no Smoke**. **[Next Wave guide](../../notes/factions/next-wave.md)** explicitly warns these are different strategic variants. | **Avoid purchasing based on an impossible “linked FTO Smoke” combo**. **One Patroclus miniature** can represent a clearly declared *legal* option; buy for FTO team/master/CoC or unlinked Smoke separately as a *list decision*. |
| **Extra Teucer or Stinger to duplicate the same MSV gun lane; extra Ironside when Achilles occupies the attack budget** | **Inference:** Stinger efficient midrange active MSV2, Teucer specialized long-range sniper/ARO, Ironside Albedo/BS Attack(-3) and Achilles high-ceiling lead all solve **different** problems but cannot all use every active Order. | **Proxy the *additional* premium gun or character variant**; buy a chosen Stinger/Teucer/Ironside once the **range/anti-MSV mission** really asks for it. None is an evidenced “bad unit.” |
| **Raindancer FTO as generic assault body when Steeljaw/Blackheart is already better fitted** | **Recorded competing-role views — [Next Wave guide](../../notes/factions/next-wave.md), [Loss of Lieutenant E172](https://open.spotify.com/episode/5cVwqFnBxM9xYIskCHHuDt):** Steeljaw can buy Sensor/turret defense, Blackheart stronger attack, while Raindancer's **FTO** has actual Shadow/Team Achilles/Dragon role. **Only FTO options link.** | **Proxy-test Raindancer first** unless its particular Fireteam/mobility package is recurring; no all-profile veto. |
| **Extra Cyberplug Puzzler/Ranter without the right Gearhead/controller and model count** | **Direct Puzzler praise** from [Shepherd](https://www.youtube.com/watch?v=52aFgWpv8es) and [Loss of Lieutenant E172](https://open.spotify.com/episode/5cVwqFnBxM9xYIskCHHuDt); **not a bad buy** but *Puzzler/Ranter* are distinct no-Order peripherals. A low-cost hidden trap is not a reason to assume four new Regular Orders or buy unlimited companion kits. | **Prioritize one correctly modeled Gearhead + Puzzler when the trap matters; proxy extra peripheral versions**, not first Puzzler. Check option pairing, **Cyberplug requirements**, body counts and Autonomous fallbacks. |
| **Ruby Monday, second Cliff-Jumper, Cube Jäger or other situational solo flank character solely for completeness** | **Unrated shopping inference:** these have differentiated surprise/Irregular specialist, off-board or rescue roles, but **no direct recording in the reviewed sources establishes they are uniformly bad**. More off-table points can weaken initial Orders/ARO defense. | **Proxy the extra one-off figure first** and commit to a sculpt when its specific late-game route/mission becomes a regular plan. |
| **A purported Next Wave Sāchā purchase** | **Source conflict flag:** the [older Next Wave tactical note](../../notes/factions/next-wave.md) mentions Sāchā as a possible mission piece, but **the current pinned Next Wave standard roster index does not list Sāchā**. A later narrative mention is not authority for current Army inclusion. | **Do not buy/plan Sāchā *for standard Next Wave* without verifying current Army legality**; proxying also cannot make an unlisted unit legal. This is a **document inconsistency**, not a claim Sāchā is a weak game unit. |

**Direct and opposing evidence:** [Shepherd Next Wave](https://www.youtube.com/watch?v=52aFgWpv8es), [Tactical Awareness Next Wave](https://open.spotify.com/episode/1c9pgE6IkthlQ2mzQpH4Qe), [Loss of Lieutenant E172](https://open.spotify.com/episode/5cVwqFnBxM9xYIskCHHuDt), [MetaChemistry E148](https://open.spotify.com/episode/3X6yHHjjJNYmZVO8qltsUZ), [Next Wave guide](../../notes/factions/next-wave.md), [current roster](next-wave.md). **Keep** **Pandora**, a reasonable **Gearhead/Puzzler**, **Harbinger LT/FO/Hacker**, chosen **Blackheart/Steeljaw**, and a purposeful **Stinger/Wraith FTO/Ironside** attack role as legitimate purchases; don't turn weakness of two Harbinger guns into a no-Harbingers stance.

#### Cross-Combined Army — even useful models often make better first proxies

**Physical collection unknown:** No authoritative Combined Army collection counts were found at the expected paths **\`inventory/combined-army.md\`, \`inventory/morat.md\`, \`inventory/shasvastii.md\`, \`inventory/onyx.md\`, \`inventory/next-wave.md\`**. The guide does **not** assume you own or lack particular minis. Actual collection and list needs should override any inferred purchase quantity.

| Potential purchase | Proxy-first / shared-model recommendation | When to buy, and what must match |
|---|---|---|
| **Alternative weapon/role sculpt of the same troop** — Yaogat, Charontid, Unidron, Nexus, Rodok, Sogarat, Caliban, Shrouded, Noctifer, Gwailo, Overdron, Harbinger, Wraith-1, Stinger | Use a distinct **correct-silhouette/base model** to represent the selected *N5.3 profile*, with the actual rifle/ML/MSV/HD+/LT/FTO effects declared. For example, **a Yaogat Sniper and Spitfire are mutually exclusive equipment**, and **Charontid HD+/Sepsitor is not MSV3 by default**. | A separate sculpt is needed when **two physically distinct loadouts appear in one list**, repeated use or tournament proxy/paint requirements justify it. A single mini is often enough for every non-simultaneous profile of an AVA1 character. |
| **Named heroes / specialty operators** — Kornak, Victor Messer, Kerr-Nau, Ko Dali, Sheskiin, Nourkias, Pandora, Drakios, Patroclus, Achilles, Ruby Monday | Before buying all collectible personalities, test a **distinct correctly sized existing Corvus Belli figure** for the *one* legal name/role in a list. Don't reuse one physical mini for two characters *on the same table*. | Buy as the hero becomes a recurring component. **Some are excellent and near-auto** (e.g. Pandora in Shepherd's Next Wave lists); proxy-first does *not* mean “bad.” |
| **Shared Combined Army R-/M-/T-/Q-/E-Drones and Unidrons** | Test optional **Guided/EVO/anti-Camo or extra ARO** use with unused **matching-footprint REMs**, but do not assume different REM families share the same silhouette or model count. **Unidron is a trooper**, not a proxy for every drone chassis by default. | Buy more after real *simultaneous* REM count exceeds your physical pool; example: **Q-Drone + T-Drone** plus a separate linkable Unidron if needed. No false Core memberships. |
| **TAG substitutes** — Avatar, Sphinx, Caskuda, Overdron, Xeodron, Raicho, Bultrak, Juggernaut | Borrow/test an **appropriately based and silhouetted TAG** before spending heavily; do not confuse **weapon chassis differences, hidden/deployment states or faction legality**. One physical TAG can stand in as a different TAG only if its size and event rules permit. | When that exact large attack plan recurs or multiple TAGs are fielded **simultaneously**. A stock S2 infantry figure is not a safe proxy for a large TAG; **Vanilla does not automatically gain sectorial TAGs**. |
| **Next Wave Skyhound (VH) or other unusual non-TAG chassis** | Use a matching **Vehicle-sized model**; a Skyhound is neither a Juggernaut TAG nor a regular infantry hacker. Test no-Cover/vertical table dependence before buying a unique vehicle. | Purchase for a recurring altitude/attack/specialist plan; model the physical footprint and current movement/LoF geometry accurately. |
| **Extra Speculo/Fiday-like infiltrators, Greif, Shasvastii Caliban/Shrouded/Malignos and hidden troops** | Use spare **distinct camouflaged infantry sculpts** with suitable silhouette/base. **A Greif Operator is not a Speculo Killer and has different rules**; disguise/markers change information, not legal unit access. | Buy duplicate impostors/skirmishers when your actual **two-Speculo or three-Caliban** list repeatedly puts them all on-table together; an unmatched model is fine for a practice game only by agreement. |
| **Bit + KISS, Med-Tech + Slave Drones, Gearhead + Sartroid Puzzlers/Ranters** | **Represent each controller AND every actually fielded peripheral/servant body**. Do not count Puzzlers, KISS or Slave Drones as extra Regular Orders. The correct Cyberplug/Connected configuration must be chosen. **KISS Pitcher versus KISS Repeater varies by army/profile**; the plastic model itself cannot override a roster. | Buy a complete unit/partner set when it becomes a recurring list component. You can't represent a two-model team with one physical base and claim both independently. |
| **Taigha, Gaki, Preta, Dāturazi, Krakot and other warband quantities** | **Proxy additional compatible silhouettes** to try a large-screen build before buying to AVA. In Morats, **Oznat + Hungries** requires separate individual bodies and exact current Fireteam permission; unlinked Irregular warbands do not create pooled Regular Orders. | Buy when *simultaneous* legal body counts exceed the existing pool and the intended list's Regular Order economy still works. |
| **Unrated one-off specialists** — Zabuk, Tyrok, Maakrep, Cube Jäger, Ruby Monday, Kurgat second Engineer, Shasvastii Aïda/Dukash, Drakios | When a full transcript does not single out a unit negatively, do not invent a “never buy.” **Proxy a named legal variant** and track **which mission, matchup, Fireteam or deployment actually improves** before making an expensive character purchase. | Buy for a repeated *specific* role, not because a unit exists in the N5.3 index. Cross-faction model reuse is about physical proxying, not magically sharing AVA or access. |
| **Optional-mode Spec-Ops / Team-Ops models** | Most ordinary matches do **not** use these modes. **Do not buy a dedicated optional-mode sculpt just to complete a sectorial catalog**. | Buy only when your league/scenario expressly allows the relevant optional mode. N5.3 changed some optional-mode availability: older list entries may be obsolete. |

**Model proxy legality:** disclose all substitutions to opponents; verify the actual **Silhouette, base diameter, physical model count and selected roster's present legal Fireteam row**. Check the *current* ITS season and event organizer policy before competitive play rather than asserting an older season's proxy permission. A model cannot be a larger/smaller trooper by assumption; an appropriate TAG, REM, Vehicle or peripheral should be physically representable at the required footprint. **No proxy changes actual availability, Army classification or weapon/program option.**

**Bottom-line purchasing order:** **Most explicitly criticized everyday roles:** Vanilla **Umbra Legate Spitfire LT/non-LT Charontid gun default**, Morat **Yaogat Combi/BSG Panzerfaust and poor double-Krakot link**, Shasvastii **Cadmus KHD for BSG-only assassination**, Onyx **Void Operator as generic Base alternative**, Next Wave **Harbinger HMG/ML, hidden Wraith MMR, plain Gearhead Engineer**. **Most worthwhile *whole-model* defer/proxy tests:** **Avatar/Sphinx/Caskuda** and other large TAG or Skyhound plans, **Morat alternative TAGs**, extra **Shasvastii Speculo/Caliban/Sphinx**, **Onyx Void or second premium TAG**, **Next Wave Juggernaut/Drakios/Skyhound**, unusual named characters and extra FTO/weapon-option sculpts. Retain the detailed contrary tournament/podcast evidence before deciding that a unit is really weak.
