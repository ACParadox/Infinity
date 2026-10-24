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
