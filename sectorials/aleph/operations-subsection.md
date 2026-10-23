---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 703
sectorial_slug: operations-subsection
sectorial_name: Operations Subsection
parent_faction: ALEPH
rules_baseline: N5.3
army_source_version: "7.26246.159"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-15
coverage: "Standard Operations Subsection roster, profiles/loadouts and composite states, canonical Fireteam chart, exact FTO restrictions, reverse Fireteam access, optional-mode hooks, and Reinforcements boundary."
---

# Operations Subsection (OSS) — N5.3 sectorial reference

## Overview and provenance

This file is the repository reference for **Operations Subsection (OSS)** (Army sectorial ID `703`). It is intended to be sufficient for ordinary list-building questions about OSS roster membership, AVA, profile costs/SWC, profile distinctions, dependencies, and Fireteam legality.

Primary data source:

- Corvus Belli Army data snapshot mirrored by `massayoshi/infinity-army-backup`.
- Pinned source commit: `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b`.
- Army dataset: `n5/operations/7.26246.159.json`.
- Source blob: `a37001ab696082155005eea050bbf013c702a7ac`.
- Army version: **7.26246.159**.
- Sectorial ID: **703**.
- Parent ALEPH ID: **701**.
- Reinforcements list ID exposed by the dataset: **799**.
- Cross-check/reference model commit: InfinityDB `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: **N5.3 + N5 FAQ v0.1**.

Coverage policy:

- The **48 standard logical roster entries** whose faction availability includes OSS are included below.
- Generic Soldier-of-Fortune catalog records present in the aggregate payload with `factions: []` are excluded.
- Faction-listed mercenary/NA2-origin records such as Authorized Bounty Hunters, Sforza, Ruby Monday, CSU, Miranda Ashcroft, Motorized Bounty Hunters, Hawkwood, Andromeda, Johnny Kao, Maximus, and Claire Lazhari are normal OSS roster entries and are included.
- **Chandra Spec-Ops** and **ALEPH Team-Ops** are optional-mode hooks, not ordinary matched-play roster entries.
- Reinforcements (`army_id: 799`) are kept distinct from the normal OSS roster and Fireteam chart.
- Fireteam legality comes from the canonical chart below, not from an `FTO` label by itself.
- Where Army marks multiple alternatives `required: true`, this file follows the repository convention and treats them as a **required source-choice set**: a legal Fireteam must contain a member from that required set; every marked row is not simultaneously mandatory.
- Composite/alternate profiles and Peripherals remain under their parent logical unit rather than becoming extra roster entries.

## Sectorial summary

| Field | Value |
|---|---|
| Sectorial | Operations Subsection (OSS) |
| Parent faction | ALEPH |
| Army ID | 703 |
| Rules baseline | N5.3 |
| Standard roster units | 48 |
| Optional-mode records | 2 |
| Linked Reinforcement roster | Army ID 799 |
| Main Fireteam chart | yes |

## Fireteam chart limits and sectorial-level restrictions

| Constraint | Value / wording |
|---|---|
| Core | `1`: maximum 1 |
| Haris | `1`: maximum 1 |
| Duo | `256`: unlimited sentinel in the Army source |
| OperationS | Duo / Haris / Core |
| Samarthan | Duo / Haris / Core |
| Asuras | Duo / Haris |
| Bounty Hunters | Duo / Haris |
| MAX-OP | Duo |
| Optimates | Duo / Haris / Core |
| Main/Reinforcement mixing | no source exception recorded; charts are kept separate |
| Required rows | required-choice set, not all required rows simultaneously |
| FTO labels | only a chart-level FTO restriction limits Fireteam access to FTO loadouts |

### Exact chart-level profile restrictions

- **Kyra Sharma:** Samarthan and Optimates use **option 1, `KYRA SHARMA FTO`**, only.
- **Claire Lazhari:** Asuras and MAX-OP explicitly say **FTO**, so only **option 2** is legal there. Samarthan and Optimates name Claire generically, so both normal OSS Claire profiles are eligible there.
- **Sforza:** Bounty Hunter access is **FTO only**, options **2 and 3**.
- **Rudra:** Wildcard access is **FTO only**, options **2 and 4**.
- **Arjuna:** Wildcard access is **FTO only**, options **1, 7, and 10**.
- **Samekh:** Wildcard access is **FTO only**, option **2**.
- **Optimate Agent Maximus:** Wildcard access is **FTO only**, options **2 and 4**, and is context-limited to **Samarthan** and **Optimates**.
- **Hawkwood:** Wildcard access is context-limited to **Bounty Hunters**; the chart does not impose an FTO restriction.
- An FTO-labelled profile without a matching chart row does not gain Fireteam access merely because it says FTO.

## Standard roster index

| Unit | Army ID | AVA | Type | Fireteam access |
|---|---:|---:|---|---|
| Danavas Hackers | 950 | 3 | LI | OperationS max 1 |
| Dawon Tacbots | 1770 | 2 | REM | OperationS max 1; Samarthan max 2 |
| Authorized Bounty Hunters | 49 | 3 | LI | Bounty Hunter required-choice source, max 3 |
| Posthumans | 597 | special | LI/SK/HI/MI | —; 2–3 Proxies as one G:Jumper troop |
| Shakti, Yadu Officer | 1191 | 1 | MI | Samarthan; Asuras; counts as Yadu/Asura as charted |
| Asuras | 584 | 4 | HI | Asuras Duo/Haris, min 1 max 3 |
| Father Lucien Sforza | 198 | 1 | MI | Bounty Hunters, FTO opts 2–3 only |
| Dasyus | 587 | 3 | SK | — |
| Arjuna Unit | 1178 | 2 | MI | Wildcard, FTO opts 1/7/10 only |
| Kazurabā Ruby Monday | 1890 | 1 | HI | — |
| Maruts | 585 | 2 | TAG | MAX-OP required-choice source, max 1 |
| Netrods | 595 | 2 | LI | — |
| Yudbots | 192 | 4 | REM | —; Servant Peripheral |
| Satrah Unit | 1772 | 1 | MI | Samarthan max 1 |
| Andromeda | 788 | 1 | MI | — |
| CSU, Corporate Security Unit | 122 | 2 | LI | OperationS max 2 |
| Dart, Optimate Huntress | 1130 | 1 | SK | — |
| Thorakitai | 600 | 2 | MI | — |
| Apsaras | 1174 | 2 | LI | Samarthan max 1 |
| Miranda Ashcroft | 51 | 1 | LI | Bounty Hunters max 1 |
| Probots | 596 | 2 | REM | — |
| Deva Functionaries | 109 | 5 | MI | OperationS; Samarthan; Asuras; Bounty Hunters; MAX-OP |
| Artalis Unit | 1771 | 1 | LI | OperationS; Samarthan; MAX-OP |
| Maximus, Optimate and HexaDome Legend | 1720 | 1 | TAG | MAX-OP required-choice source, max 1 |
| Nagas | 59 | 3 | SK | — |
| Kyra Sharma | 1897 | 1 | HI | Samarthan/Optimates, FTO opt 1 only |
| Kinnara Scoutbots | 1901 | 2 | REM | — |
| Johnny Kao | 1892 | 1 | MI | MAX-OP; Optimates required-choice source |
| Daleth Rebots | 590 | 2 | REM | — |
| Lamedh Rebots | 593 | 2 | REM | — |
| Motorized Bounty Hunters | 1565 | 2 | LI | Bounty Hunter required-choice source, max 2 |
| Samekh Rebots | 592 | 1 | REM | Wildcard, FTO opt 2 only |
| John Hawkwood | 1556 | 1 | MI | Wildcard in Bounty Hunters only |
| Optimate Agent Maximus | 1862 | 1 | MI | Wildcard in Samarthan/Optimates, FTO opts 2/4 only |
| Garuda Tacbots | 110 | 3 | REM | — |
| Tarkshya Interception Wing | 1904 | 1 | VH | — |
| Pilot-X Team | 1903 | 1 team | LI + REM | Optimates max 1 |
| Shukra Consultants | 1128 | 2 | LI | — |
| Riksha Tacbots | 1769 | 2 | REM | OperationS max 1; Samarthan required-choice max 2 |
| Zayin Rebots | 591 | 1 | REM | — |
| Warcors | 50 | 1 | LI | — |
| Yadu | 1129 | 5 | MI | Samarthan required-choice; Asuras; MAX-OP |
| Sophotects | 185 | 2 | MI | — |
| Rudras GunBots | 1197 | 2 | REM | Wildcard, FTO opts 2/4 only |
| Sharvara HoundBots | 1899 | 2 | REM | OperationS; Samarthan; MAX-OP; Optimates |
| Yaksha Tacbots | 1906 | 2 | REM | — |
| Dr. Claire Lazhari | 1894 | 1 | LI | Samarthan/Optimates all profiles; Asuras/MAX-OP FTO opt 2 only |
| Dikpala Tacbots | 1898 | Total | REM | OperationS required-choice source, max 5 |

### Optional-mode entries

| Unit | Army ID | Mode | Fireteam hook |
|---|---:|---|---|
| Chandra Spec-Ops | 1922 | Infinity Spec-Ops | chart placeholder max 1 in OperationS, Samarthan, Asuras, Bounty Hunters, MAX-OP |
| ALEPH Team-Ops | 1936 | Infinity Team-Ops | optional-mode only; not an ordinary matched-play roster entry |

## Unit details

Notation: stats are `MOV CC BS PH WIP ARM BTS VITA S`. `STR` is called out where the source models Structure. Costs are `pts / SWC`. Army option IDs are preserved.

### Danavas Hackers — `danavas-hackers`

- **Stats:** `10-10 15 11 11 15 1 3 1 2`; AVA 3, LI.
- **Rules:** Courage; Cube 2.0.
- **Option 2:** **22 / 0.5** — Combi Rifle, Pitcher, Breaker Pistol, CC Weapon; Hacker, Hacking Device Plus with **Oblivion (+1B)**.

### Dawon Tacbots — `dawon-tacbots`

- **Stats:** `15-10 22 11 13 12 1 3 1 2`; AVA 2, REM/STR.
- **Rules/equipment:** Remote Presence, Martial Arts L2, Courage, Dogged, Religious Troop, Immunity (Enhanced); ECM: Hacker (-3). The source carries two Dodge modifiers (`+3` and `+5`) and they are preserved as source data rather than collapsed here.
- **Option 1:** **20 / 0** — Chain Rifle (+1B), Flammenspeer, MULTI Pistol (+1B), E/M CC Weapon (PS=6).
- **Option 2:** **19 / 0** — Pulzar (+1B), Blitzen, MULTI Pistol (+1B), Shock CC Weapon (PS=6).
- **Option 3:** **20 / 0** — Boarding Shotgun, MULTI Pistol (+1B), Shock CC Weapon (PS=6).
- **Option 4:** **19 / 0** — Chain Rifle, Flammenspeer, MULTI Pistol (+1B), E/M CC Weapon (PS=6).
- **Option 5:** **18 / 0** — Pulzar, Blitzen, MULTI Pistol (+1B), Shock CC Weapon (PS=6).

### Authorized Bounty Hunters — `authorized-bounty-hunters`

- **Stats:** `10-10 16 12 10 13 1 3 1 2`; AVA 3, LI.
- **Rules:** Booty (ReRoll), Stealth.
- **Option 2:** **12 / 0** — Boarding Shotgun, Heavy Riotstopper, Pistol, PARA CC Weapon (-6).
- **Option 3:** **19 / 0.5** — Sniper Rifle, Breaker Pistol (+1B), PARA CC Weapon (-6).
- **Option 4:** **21 / 1** — Spitfire, Boarding Pistol, PARA CC Weapon (-6).
- **Option 5:** **12 / 0** — Submachine Gun, Akrylat-Kanone, Breaker Pistol, PARA CC Weapon (-6).

### Posthumans — `posthumans`

**Army relation:** select **minimum 2, maximum 3 Proxies**. Only one Proxy may be taken per model. All selected Proxies must be in the same Combat Group and together count as one trooper for the G:Jumper troop.

#### Proxy Mk.1

- **Stats:** `10-10 13 13 11 15 2 3 1 2`; LI.
- **Rules:** G:Jumper, Courage, Mimetism (-3), No Wound Incapacitation.
- **Option 1 Hacker:** **14 / 0.5** — Combi Rifle, Nanopulser, Pistol, CC Weapon; Hacking Device.
- **Option 2 Engineer:** **13 / 0** — Combi Rifle, Nanopulser, D-Charges, Pistol, CC Weapon; Deactivator, GizmoKit.
- **Option 3 Doctor:** **13 / 0** — Combi Rifle, Nanopulser, Pistol, CC Weapon; MediKit.

#### Proxy Mk.2

- **Stats:** `10-10 13 13 13 15 1 0 1 2`; SK.
- **Rules:** G:Jumper, Surprise Attack (-3), Courage, Camouflage, Infiltration, Mimetism (-6), Stealth, NWI, Total Terrain.
- **Option 1:** **26 / 1.5** — MULTI Sniper Rifle, Pistol, CC Weapon.
- **Option 2 Hacker:** **22 / 0.5** — Boarding Shotgun, Pistol, CC Weapon; Hacking Device.

#### Proxy Mk.4

- **Stats:** `10-10 13 14 14 15 5 6 2 2`; HI.
- **Rules:** G:Jumper, BS Attack (-3), Courage, Immunity (AP).
- **Option 1:** **30 / 1.5** — HMG, Nanopulser, Pistol, CC Weapon.
- **Option 2:** **26 / 1.5** — Heavy Rocket Launcher, Submachine Gun, Nanopulser, Pistol, CC Weapon.

#### Proxy Mk.5

- **Stats:** `10-10 14 13 11 15 3 3 1 2`; MI.
- **Rules:** G:Jumper, Courage, Forward Deployment (+10), NWI.
- **Option 1:** **21 / 0.5** — Mk12, Heavy Pistol, CC Weapon; BS Attack (+1SD).
- **Option 2 FO:** **13 / 0.5** — Submachine Gun (+1B), Flash Pulse, E/M Grenades, Heavy Pistol, CC Weapon; Forward Observer.

### Shakti, Yadu Officer — `yadu-officer-shakti`

- **Stats:** `15-5 16 13 11 14 3 6 2 2`; AVA 1, MI.
- **Rules/equipment:** Courage, Number 2, Warhorse; Albedo (-6), Killer Hacking Device with Trinity (PS=5).
- **Option 1:** **35 / 0** — Mk12, E/Marat, AP Mine, Heavy Pistol, CC Weapon; Hacker.
- **Option 2:** **37 / 0** — option 1 plus Armed Turret (E/Mitter); Hacker.
- **Option 3 Lieutenant:** **35 / 0** — option 1 weapons; Hacker, Lieutenant.
- **Option 4 Lieutenant:** **37 / 0** — option 2 weapons; Hacker, Lieutenant.

### Asuras — `asuras`

- **Stats:** `15-5 20 14 14 15 5 6 2 2`; AVA 4, HI.
- **Rules/equipment:** Courage, NWI; ECM: Hacker (-3), MSV3.
- **Option 2:** **61 / 1.5** — AP Spitfire, Pulzar, MULTI Pistol, AP CC Weapon (PS=6).
- **Option 3 Hacker:** **63 / 0.5** — MULTI Marksman Rifle, Pulzar, MULTI Pistol, AP CC Weapon (PS=6); Hacking Device Plus, Trinity (+1SD).
- **Option 5 Lieutenant:** **65 / 1** — option 2 weapons; Lieutenant (+1 Order), generating two Lieutenant orders.
- **Option 6 Lieutenant Hacker:** **67 / 0** — option 3 weapons; Lieutenant (+1 Order), Hacking Device Plus, Trinity (+1SD).

### Father Lucien Sforza — `father-lucien-sforza`

- **Stats:** `10-10 19 13 11 13 2 3 1 2`; AVA 1, MI.
- **Rules/equipment:** X-Visor; BS Attack (+1SD), Immunity (ARM), Combat Instinct, Stealth, NCO, Dogged, Warhorse.
- **Option 1 — SFORZA:** **26 / 0** — Viral Rifle, Adhesive Launcher Rifle, Nanopulser, Heavy Pistol, PARA CC Weapon (-9); Holoprojector, Surprise Attack (-3), Forward Deployment (+10). **Not FTO.**
- **Option 2 — SFORZA FTO:** **23 / 0** — same core weapons; FTO.
- **Option 3 — SFORZA FTO:** **26 / 0** — option 2 plus Albedo (-6); FTO.

### Dasyus — `dasyus`

- **Stats:** `15-5 16 13 12 14 1 3 1 2`; AVA 3, SK.
- **Rules:** BS Attack (+1SD), Surprise Attack (-3), Courage, Camouflage, Hidden Deployment, Mimetism (-6), Infiltration (ReRoll), Immunity (Shock), Stealth, Total Terrain.
- **Option 2:** **28 / 0** — Boarding Shotgun, Pulzar, D-Charges, Silenced Pistol (PS=7), CC Weapon.
- **Option 3:** **34 / 1.5** — MULTI Sniper Rifle, Pulzar, Silenced Pistol (PS=7), CC Weapon.
- **Option 4 KHD:** **31 / 0** — AP Submachine Gun, Pulzar, D-Charges, Silenced Pistol (PS=7), CC Weapon; Killer Hacking Device.
- **Option 5 Hacker:** **33 / 0.5** — option 4 weapons; Hacking Device.
- **Option 6 FO:** **29 / 0** — AP Submachine Gun, Pulzar, D-Charges, Flash Pulse, Silenced Pistol (PS=7), CC Weapon; Deployable Repeater, Forward Observer.
- **Option 8:** **30 / 0.5** — AP Submachine Gun, Pulzar, Viral Mine, D-Charges, Silenced Pistol (PS=7), CC Weapon; Minelayer (2).

### Arjuna Unit — `arjuna-unit`

- **Stats:** `15-5 17 13 11 14 3 3 1 2`; AVA 2, MI.
- **Rules:** Immunity (Shock), Mimetism (-3), Specialist Operative, Dodge (+5), Tactical Awareness, Religious Troop. Non-FTO field profiles add Forward Deployment (+20).
- **FTO option 1:** **21 / 0** — Boarding Shotgun (+1SD), Flash Pulse (PS=5), D-Charges, Breaker Pistol, CC Weapon.
- **Option 2:** **32 / 0** — option-1 weapons + Forward Deployment; includes KiranBot 1.
- **Option 3:** **25 / 0** — option-1 weapons + Forward Deployment; no peripheral.
- **FTO option 7:** **30 / 1.5** — Spitfire, D-Charges, Breaker Pistol, CC Weapon; TinBot Firewall (-3).
- **Option 8:** **42 / 1.5** — option-7 weapons + Forward Deployment; includes KiranBot 1.
- **Option 9:** **35 / 1.5** — option-7 weapons + Forward Deployment; no peripheral.
- **FTO option 10:** **23 / 0** — AP Submachine Gun, E/Mitter, D-Charges, Breaker Pistol, CC Weapon; TinBot Firewall (-3).
- **Option 11:** **33 / 0** — option-10 weapons + Forward Deployment; includes KiranBot 1.
- **Option 12:** **26 / 0** — option-10 weapons + Forward Deployment; no peripheral.
- **Option 13:** **32 / 0** — option-1 weapons + Forward Deployment; includes KiranBot 2.
- **Option 14:** **33 / 0** — option-10 weapons + Forward Deployment; includes KiranBot 2.
- **Option 15:** **42 / 1.5** — option-7 weapons + Forward Deployment; includes KiranBot 2.
- **KiranBots:** `15-5 13 11 11 11 1 3 1 2`, REM/Peripheral; ECM Hacker (-3), Peripheral (Synchronized), Courage, Forward Deployment (+20), Dodge (+2.5), Mimetism (-6). KiranBot 1 carries Deployable Repeater, E/Marat (+1B), AP Heavy Pistol, PARA CC Weapon. KiranBot 2 carries Pulzar (+1B), Repeater, AP Heavy Pistol, PARA CC Weapon. Each is an internal 7-point included profile.

### Kazurabā Ruby Monday — `kazuraba-ruby-monday`

- **Stats:** `15-5 18 12 12 13 3 6 2 2`; AVA 1, HI/STR; Irregular.
- **Rules:** BS Attack (+1B), Booty, Dodge (+3), Immunity (IMM-B), Technorganic, Total Terrain, Climbing Plus, Specialist Operative.
- **Option 1:** **19 / 0** — Adhesive Launcher Rifle, Flash Pulse, E/M Grenades, Stun Pistol, CC Weapon; Irregular.

### Maruts — `maruts`

- **Stats:** `15-10 18 15 17 15 8 9 3 7`; AVA 2, TAG/STR.
- **Rules/equipment:** Remote Presence, Courage, Dodge (PH=11), GizmoKit (PH=13), Tactical Awareness, Total Terrain, CC Attack (+1B), BS Attack (SR-1); ECM: Guided (-6), MSV2.
- **Option 1:** **86 / 1.5** — MULTI HMG, Heavy Flamethrower, Pulzar, AP CC Weapon (PS=3); includes Karkata; Regular + Tactical Awareness.
- **Option 2 Lieutenant:** **90 / 2** — same weapons; Lieutenant, Strategos L2; includes Karkata.
- **Karkata:** `15-10 — — 10 12 0 3 1 1`, REM/STR; Courage, Dodge (+3), Mimetism (-3), Specialist Operative, Total Terrain, Peripheral (Ancillary). Internal source cost 3.

### Netrods — `netrods`

- **Stats:** immobile deployment profile; AVA 2, LI/STR.
- **Rules:** must deploy by Combat Jump during the Deployment Phase; Warhorse, Combat Jump (PH=12), Religious Troop.
- **Option 1:** **6 / 0** — no weapons; Regular order.

### Yudbots — `yudbots`

- **Stats:** `15-10 11 8 10 13 0 3 1 1`; AVA 4, REM/STR Peripheral.
- **Rules:** Peripheral (Servant), Courage, Mimetism (-3).
- **Option 1:** **3 / 0** — PARA CC Weapon (-3); no independent order.

### Satrah Unit — `satrah-unit`

- **Stats:** `10-10 16 13 11 14 2 3 1 2`; AVA 1, MI.
- **Rules/equipment:** Stealth, Climbing Plus; Albedo (-6), MSV2.
- **Option 1:** **24 / 0** — Thunderbolt (+1B), Pulzar, Heavy Pistol, CC Weapon.
- **Option 4:** **24 / 0** — MULTI Marksman Rifle, Pulzar, Heavy Pistol, CC Weapon.
- **Option 5 Hacker:** **20 / 0** — Submachine Gun, Pulzar, Cybermine, Heavy Pistol, CC Weapon; Killer Hacking Device carrying the source Firewall (-3) upgrade.

### Andromeda — `andromeda`

- **Stats:** `15-5 21 12 12 13 2 3 1 4`; AVA 1, MI.
- **Rules:** Martial Arts L3, Courage, Dodge (+5), Guard, Immunity (Shock), Mimetism (-3), Specialist Operative, Stealth, NWI, Infiltration (PH=15).
- **Option 5:** **30 / 0** — Submachine Gun, Zapper, Flash Pulse, D-Charges, Breaker Pistol, DA CC Weapon (PS=6).
- **Option 6:** **33 / 0** — Boarding Shotgun (+1B), Zapper, Flash Pulse, D-Charges, Breaker Pistol, DA CC Weapon (PS=6).

### CSU, Corporate Security Unit — `csu-corporate-security-unit`

- **Stats:** `10-10 16 12 10 12 0 3 1 2`; AVA 2, LI.
- **Rules:** MetaChemistry, Sixth Sense; several profiles are Specialist Operatives.
- **Option 1:** **10 / 0** — Breaker Rifle, Nanopulser (+1B), MULTI Pistol, PARA CC Weapon (-6).
- **Option 2:** **11 / 0** — Combi Rifle, Nanopulser (+1B), MULTI Pistol, PARA CC Weapon (-6).
- **Option 3:** **11 / 0** — Boarding Shotgun, MULTI Pistol, Adhesive Launcher Rifle (+1B), PARA CC Weapon (-6).
- **Option 4 Specialist:** **11 / 0** — Rifle, Light Shotgun, MULTI Pistol, Nanopulser (+1B), PARA CC Weapon (-6); Specialist Operative.
- **Option 5 Specialist:** **13 / 0** — Breaker Combi Rifle, Nanopulser (+1B), MULTI Pistol, PARA CC Weapon (-6); Specialist Operative.

### Dart, Optimate Huntress — `dart-optimate-huntress`

- **Stats:** `10-10 16 13 13 13 1 3 1 2`; AVA 1, SK.
- **Rules/equipment:** MSV1; Surprise Attack (-3), Camouflage, Courage, Forward Deployment (+20), Mimetism (-3), Immunity (Shock), Stealth, NWI, Total Terrain, Climbing Plus, Specialist Operative, Decoy (1).
- **Option 1:** **35 / 0** — AP Submachine Gun, Viral Tactical Bow (+1SD), E/M Grenades, Pistol, CC Weapon.
- **Option 2:** **35 / 0** — AP Submachine Gun, Viral Tactical Bow (+1SD), Shock Mine, Pistol, CC Weapon.
- **Option 3:** **36 / 0.5** — option 2; Minelayer.
- **Option 4:** **42 / 0.5** — option 3; includes Sharvara_K-9 HoundBot.
- **Sharvara_K-9:** `15-10 22 11 12 12 0 3 1 3`, REM/Peripheral; Camouflage, Courage, Forward Deployment (+20), CC Attack (-6), Dodge (+3/+5 as source entries), Natural Born Warrior, Mimetism (-3), Stealth. Flash Pulse, Heavy Riotstopper, E/Marat, DA CC Weapon (PS=7), PARA CC Weapon. Internal source cost 6.

### Thorakitai — `thorakitai`

- **Stats:** `10-10 16 12 11 13 3 0 1 2`; AVA 2, MI.
- **Option 1:** **12 / 0** — Submachine Gun, E/Mitter, Pulzar, Pistol, CC Weapon.
- **Option 2:** **14 / 0** — Combi Rifle, Nanopulser, Pistol, CC Weapon.
- **Option 6 FO:** **13 / 0** — option 1 plus Flash Pulse; Forward Observer.
- **Option 7 Paramedic:** **14 / 0** — option 1; MediKit, Paramedic.
- **Option 9:** **23 / 1.5** — Feuerbach, Nanopulser, Pistol, CC Weapon.

### Apsaras — `apsaras`

- **Stats:** `10-10 15 13 10 14 1 3 1 2`; AVA 2, LI.
- **Equipment:** Killer Hacking Device with Firewall (-3); Deployable Repeater on all listed profiles.
- **Option 1:** **17 / 0** — Submachine Gun, Zapper, Pistol, CC Weapon; Hacker.
- **Option 2 RemDriver:** **20 / 0** — same weapons; Hacker, RemDriver with source modifiers `CC=15`, `BS=13`, `WIP=14`.
- **Option 3 TAGCom:** **18 / 0** — same weapons; Hacker, TAGCom with Dodge (PH+3) and GizmoKit (PH+1).
- **Option 4 Lieutenant:** **20 / 0** — option 2; Hacker, Lieutenant.

### Miranda Ashcroft — `miranda-ashcroft-authorized`

- **Stats:** `10-10 19 12 10 13 1 3 1 2`; AVA 1, LI.
- **Rules:** CC Attack (-6), Mimetism (-6), Specialist Operative, Marksmanship, Stealth.
- **Option 1:** **27 / 0** — MULTI Rifle, PARA Mine, Boarding Pistol, Monofilament CC Weapon.
- **Option 2:** **25 / 0** — Boarding Shotgun, PARA Mine, Boarding Pistol, Monofilament CC Weapon.
- **Option 3:** **28 / 0** — Combi Rifle, E/Mitter (+1B), PARA Mine, Boarding Pistol, Monofilament CC Weapon.

### Probots — `probots`

- **Stats:** `10-10 13 11 10 13 2 3 1 4`; AVA 2, REM/STR.
- **Rules/equipment:** Remote Presence, Courage, Baggage.
- **Option 1:** **8 / 0** — PARA CC Weapon (-3); Deactivator, Repeater.
- **Option 2 EVO:** **14 / 0.5** — PARA CC Weapon (-3); EVO Hacking Device, Hacker.
- **Option 3 TR:** **17 / 0** — Combi Rifle, PARA CC Weapon (-3); Repeater, Total Reaction.

### Deva Functionaries — `deva-functionaries`

- **Stats:** `10-10 15 12 11 15 2 3 1 2`; AVA 5, MI.
- **Rules:** Courage, Number 2, NWI, Immunity (Isolated).
- **Option 1:** **20 / 0** — Combi Rifle, Nanopulser, Pistol, CC Weapon.
- **Option 2:** **24 / 0** — option 1; includes Devabot.
- **Option 3:** **22 / 0** — MULTI Rifle, Nanopulser, Pistol, CC Weapon.
- **Option 4 Hacker:** **25 / 0.5** — option 1; Hacking Device.
- **Option 5 KHD:** **20 / 0** — Boarding Shotgun, Pistol, CC Weapon; Killer Hacking Device.
- **Option 6:** **21 / 0** — option 1; Triangulated Fire, Sensor.
- **Option 8 FO:** **21 / 0** — Combi Rifle, Nanopulser, Flash Pulse, Pistol, CC Weapon; Forward Observer.
- **Option 9:** **29 / 1** — Spitfire, Nanopulser, Pistol, CC Weapon; MSV2.
- **Option 10 Lieutenant:** **20 / 0** — option 1; Lieutenant.
- **Option 11 Lieutenant:** **24 / 0** — option 1; Lieutenant; includes Devabot.
- **Option 12 Lieutenant:** **21 / 0** — option 1; Lieutenant, Triangulated Fire, Sensor.
- **Devabot:** `15-10 13 10 10 11 0 3 1 2`, REM/Peripheral; Courage, Peripheral (Synchronized); Heavy Flamethrower, PARA CC Weapon (-3). Internal source cost 4.

### Artalis Unit — `artalis-unit`

- **Stats:** `10-10 17 12 10 14 1 3 1 2`; AVA 1, LI.
- **Rules/equipment:** BS Attack (SR-1), Dodge (+2.5), Immunity (Shock), NCO; Deactivator (ReRoll).
- **Option 1 Engineer:** **27 / 0** — Combi Rifle, Light Rocket Launcher, D-Charges, AP Heavy Pistol, CC Weapon; GizmoKit, Engineer.
- **Option 2 Engineer:** **23 / 0** — K1 Combi Rifle, D-Charges, AP Heavy Pistol, CC Weapon; GizmoKit, Engineer.
- **Option 3 Engineer:** **23 / 0** — MULTI Rifle, D-Charges, AP Heavy Pistol, CC Weapon; GizmoKit, Engineer.
- **Option 4 Doctor:** **23 / 0** — K1 Combi Rifle, D-Charges, AP Heavy Pistol, CC Weapon; MediKit, Doctor.

### Maximus, Optimate and HexaDome Legend — `maximus`

- **Stats:** `15-10 24 14 13 13 6 6 4 6`; AVA 1, TAG/STR.
- **Rules/equipment:** CC Attack (-6), BS Attack (SR-1), Courage, Dodge (+5), Natural Born Warrior, Immunity (ARM), Immunity (POS), Tactical Awareness, Transmutation (Escape System -3); ECM: Guided (-6).
- **Option 1:** **82 / 1.5** — AP HMG, E/M Carbine, Heavy Pistol, AP+DA CC Weapon (PS=4); Regular + Tactical Awareness.
- **Option 2:** **80 / 1** — AP Thunderbolt (+2B), E/M Carbine, Heavy Pistol, AP+DA CC Weapon (PS=4); Regular + Tactical Awareness.
- **Option 3 Lieutenant:** **82 / 0** — option 1 weapons; Lieutenant.
- **Operator Maximus alternate state:** `15-5 22 13 13 13 3 3 4 2`, MI; CC Attack (-6), Courage, Dodge (+2.5), Natural Born Warrior, Immunity (ARM), Specialist Operative, Tactical Awareness. Disabled/internal loadouts track the selected TAG loadout.
- **Army relation:** this Maximus and **Optimate Agent Maximus** are mutually exclusive normal-roster versions; the source also relates this Maximus to its Reinforcement counterpart.

### Nagas — `nagas`

- **Stats:** `10-10 16 12 12 14 1 0 1 2`; AVA 3, SK.
- **Rules:** Surprise Attack (-3), Courage, Camouflage, Infiltration, Mimetism (-3), Stealth, Dogged, Total Terrain.
- **Option 3:** **29 / 1.5** — MULTI Sniper Rifle, Nanopulser, Pistol, CC Weapon; BS Attack (+1SD).
- **Option 4:** **25 / 0.5** — Boarding Shotgun, Nanopulser, Shock Mine, Pistol, CC Weapon; Minelayer.
- **Option 5 KHD:** **27 / 0** — AP Submachine Gun, Nanopulser, D-Charges, E/M Mine, Pistol, CC Weapon; Killer Hacking Device.
- **Option 6 Hacker:** **29 / 0.5** — AP Submachine Gun, Nanopulser, D-Charges, Pistol, CC Weapon; Hacking Device with Carbonite (+1SD), Deployable Repeater.
- **Option 7 FO:** **25 / 0** — AP Submachine Gun, Nanopulser, Flash Pulse, D-Charges, Pistol, CC Weapon; Deployable Repeater, Forward Observer.
- **Option 8:** **26 / 0.5** — AP Submachine Gun, Nanopulser, Monofilament Mine, Pistol, CC Weapon; Minelayer.

### Kyra Sharma — `kyra-sharma-the-iron-maiden-of-the-optimates`

- **Stats:** `15-10 18 14 12 14 3 3 2 2`; AVA 1, HI.
- **Rules/equipment:** BS Attack (SR-1), Courage, Dodge (+5), Regeneration, Tactical Awareness, Super-Jump (+7.5; Jet Propulsion), source Immunity entries for ARM and Critical; MediKit (+1B).
- **Option 1 — KYRA SHARMA FTO:** **45 / 0** — MULTI Marksman Rifle, Light Riotstopper (+1B), WildParrot, Breaker Pistol (+1SD), PARA CC Weapon (-6); Paramedic. **Only this option receives Kyra's charted Fireteam access.**
- **Option 2:** **52 / 0** — MULTI Rifle, Light Riotstopper (+1B), Akrylat-Kanone, WildParrot, Breaker Pistol (+1SD), PARA CC Weapon (-6); Parachutist, Combat Jump, Paramedic. Not FTO.

### Kinnara Scoutbots — `kinnara-scoutbots`

- **Stats:** `15-5 23 12 12 12 1 3 1 2`; AVA 2, REM/STR.
- **Rules/equipment:** Remote Presence, Martial Arts L2, Surprise Attack (-3), Courage, Dodge (+5), Mimetism (-3), Sensor, Decoy (2), Stealth, Climbing Plus, Specialist Operative, Total Terrain; ECM Hacker (-3).
- **Option 1:** **25 / 0.5** — Vulkan Shotgun, Heavy Flamethrower, D-Charges, E/M Mine, Pistol, Monofilament CC Weapon; Infiltration, Minelayer.
- **Option 2:** **24 / 0** — Vulkan Shotgun, Heavy Flamethrower, D-Charges, Eclipse Grenades, Pistol, Monofilament CC Weapon; Parachutist.
- **Option 3:** **24 / 0** — Submachine Gun, E/M Carbine, D-Charges, Eclipse Grenades, Pistol, Monofilament CC Weapon; Parachutist.

### Johnny Kao — `johnny-kao-optimate-and-technomancer-master`

- **Stats:** `15-5 18 13 12 14 3 6 2 2`; AVA 1, MI; Non-Hackable.
- **Rules/equipment:** Engineer (ReRoll), Mimetism (-3); Deactivator (ReRoll), GizmoKit (+1B), X-Visor.
- **Option 1:** **36 / 0** — Plasma Carbine, Zapper, Monofilament Mine, D-Charges, MULTI Pistol, CC Weapon.
- **Option 2:** **40 / 0** — MULTI Rifle, Zapper, Drop Bears (`ARM=0` source modifier), D-Charges, MULTI Pistol, CC Weapon.
- **Option 3:** **42 / 0** — MULTI Rifle, Zapper, Monofilament Mine, D-Charges, Armed Turret (Plasma Carbine), MULTI Pistol, CC Weapon.

### Daleth Rebots — `daleth-rebots`

- **Stats:** `15-10 13 11 10 13 0 3 1 3`; AVA 2, REM/STR.
- **Rules/equipment:** Remote Presence, Courage, Triangulated Fire, Forward Observer, Sensor, Climbing Plus; Deactivator, Repeater.
- **Option 1:** **15 / 0** — Combi Rifle, Flash Pulse, PARA CC Weapon (-3).
- **Option 2:** **18 / 0** — same weapons; Tactical Awareness.

### Lamedh Rebots — `lamedh-rebots`

- **Stats:** `15-15 13 8 11 13 0 3 1 3`; AVA 2, REM/STR.
- **Rules/equipment:** Remote Presence, Courage, Mimetism (-3); Repeater.
- **Option 1:** **7 / 0** — Flash Pulse, PARA CC Weapon (-3).

### Motorized Bounty Hunters — `motorized-bounty-hunters`

- **Stats:** `20-15 17 12 10 13 1 3 1 4`; AVA 2, LI; Irregular + Impetuous.
- **Rules/equipment:** Booty (ReRoll), Limited Cover, Dodge (+5), Mimetism (-3); Motorcycle.
- **Option 1:** **8 / 0** — Boarding Shotgun, Pistol, PARA CC Weapon (-6), Heavy Riotstopper.
- **Option 2:** **9 / 0** — Submachine Gun, Chain-colt (+1B), Pistol, PARA CC Weapon (-6).
- **Option 3:** **16 / 0.5** — Red Fury, Breaker Pistol, PARA CC Weapon (-6).

### Samekh Rebots — `samekh-rebots`

- **Stats:** `15-10 13 12 10 13 0 3 1 3`; AVA 1, REM/STR.
- **Rules:** Remote Presence, Courage.
- **Option 1:** **16 / 1.5** — Missile Launcher, PARA CC Weapon (-3); BS Attack (Guided). Not FTO.
- **Option 2 — SAMEKH Rebot FTO:** **15 / 1.5** — Missile Launcher, Flash Pulse, PARA CC Weapon (-3). **Wildcard profile.**

### John Hawkwood — `john-hawkwood-mercenary-officer`

- **Stats:** `10-10 22 13 11 14 3 6 1 2`; AVA 1, MI.
- **Rules:** Martial Arts L1, BS Attack (+1SD), Courage, Immunity (Shock), Mimetism (-3), NWI, Stealth, Total Terrain.
- **Option 6:** **35 / 1** — K1 Sniper Rifle, Nanopulser (+1B), MULTI Pistol, DA CC Weapon (PS=7).
- **Option 7:** **40 / 0** — Combi Rifle (+1B), Nanopulser (+1B), MULTI Pistol, DA CC Weapon (PS=7); X-Visor, Chain of Command.
- **Fireteam:** Wildcard only in the Bounty Hunter family; no FTO restriction in the chart.

### Optimate Agent Maximus — `optimate-agent-maximus`

- **Stats:** `15-5 22 13 13 13 3 3 1 2`; AVA 1, MI.
- **Rules/equipment:** CC Attack (-6), Courage, Dodge (+2.5), Natural Born Warrior, Immunity (ARM), Number 2, Specialist Operative, Tactical Awareness, NWI; Albedo (-3).
- **Option 1:** **48 / 1** — AP Thunderbolt (+2B), E/M Carbine, Heavy Pistol, AP+DA CC Weapon (PS=6); includes Minimus. Not FTO.
- **Option 2 — MAXIMUS AGENT FTO:** **45 / 1** — same weapons; TinBot (Repeater), no Minimus. FTO.
- **Option 3 Lieutenant:** **48 / +1 SWC** — option 1 weapons; Lieutenant; includes Minimus. Not FTO.
- **Option 4 — MAXIMUS AGENT FTO Lieutenant:** **45 / +1 SWC** — option 2 equipment; Lieutenant. FTO.
- **Minimus MateBot:** `15-10 21 9 11 12 0 3 1 1`, REM/Peripheral; Repeater, Peripheral (Synchronized), CC Attack (-6), Courage, Dodge (+3/+5 source entries), Mimetism (-3). Flash Pulse, E/Marat, DA CC Weapon (PS=7), PARA CC Weapon.
- **Army relation:** mutually exclusive with the Maximus TAG normal-roster entry.

### Garuda Tacbots — `garuda-tacbots`

- **Stats:** `20-5 13 12 11 13 0 3 1 2`; AVA 3, REM/STR.
- **Rules:** Remote Presence, Courage, Mimetism (-3), Parachutist, Combat Jump, Super-Jump (Jet Propulsion).
- **Option 3:** **18 / 0** — Boarding Shotgun, Chain-colt (PS=6 source modifier), PARA CC Weapon (-3).
- **Option 4:** **25 / 1.5** — Spitfire, PARA CC Weapon (-3).
- **Option 5 FO:** **20 / 0** — Combi Rifle, Flash Pulse, PARA CC Weapon (-3); Forward Observer.

### Tarkshya Interception Wing — `tarkshya-interception-wing`

#### Interception Wing

- **Stats:** `20-5 — 13 12 13 4 6 3 7`; AVA 1, VH/STR.
- **Rules/equipment:** Remote Presence, Aerial, BS Attack (SR-1), Courage, Dodge (-3 source modifier), Mimetism (-6), No Cover, Super-Jump (+7.5; Jet Propulsion), Tech-Recovery, Total Terrain, Transmutation (Escape System -2), GizmoKit (PH=13); ECM Hacker (-3), MSV1.
- **Option 1:** **41 / 1.5** — MULTI Red Fury, Chain Rifle.
- **Option 2:** **38 / 0** — MULTI Marksman Rifle, AP Submachine Gun.
- **Option 3:** **34 / 0** — MULTI Marksman Rifle, Chain Rifle (+1B).

#### Tarkshya Operator alternate state

- **Stats:** `15-5 13 13 10 13 3 3 3 2`; HI/STR.
- **Rules/equipment:** Remote Presence, Courage, Mimetism (-6), Forward Observer (+1SD), Super-Jump (Jet Propulsion); ECM Hacker (-3), MSV1.
- Disabled/internal operator loadouts correspond to the selected primary option and add Flash Pulse (+1SD), MULTI Pistol, and CC Weapon to the carried gun package.

### Pilot-X Team — `pilot-x-team`

**Dependency:** a Pilot-X Team is **1 Pilot-X plus 0–2 RacerBots Mk-III**. RacerBot Mk-III cannot be taken without Pilot-X, and all members of the team must belong to the same Combat Group.

#### Pilot-X

- **Stats:** `10-10 17 12 10 14 1 6 1 2`; LI.
- **Rules/equipment:** Immunity (Shock), RemDriver source modifiers; Hacking Device with Zero Pain.
- **Option 2:** **23 / 0.5** — E/Mitter, Flash Pulse, MULTI Pistol, PARA CC Weapon (-3); Hacker.

#### RacerBot Mk-III

- **Stats:** `20-10 13 11 12 11 0 3 1 2`; REM/STR, up to 2 within the team.
- **Rules/equipment:** Courage, Dodge (+5), No Cover, Remote Presence; Bangbomb (+4), ECM Hacker (-3), 360º Visor, Deployable Repeater.
- **Option 1:** **8 / 0** — Light Riotstopper, Mine Dispenser (PARA), Stun Pistol, PARA CC Weapon (-6).

### Shukra Consultants — `shukra-consultants`

- **Stats:** `10-10 16 12 11 14 1 3 1 2`; AVA 2, LI.
- **Rules/equipment:** Counterintelligence, Courage, Discover (+3); Biometric Visor.
- **Option 1 CoC:** **21 / 0** — Boarding Shotgun, Pistol, CC Weapon; Chain of Command.
- **Option 2 CoC:** **26 / 0** — MULTI Rifle, Nanopulser, Pistol, CC Weapon; Chain of Command.
- **Option 3 Lieutenant:** **24 / 0** — MULTI Rifle, Nanopulser, Pistol, CC Weapon; Lieutenant, Strategos L1.

### Riksha Tacbots — `riksha-tacbots`

- **Stats:** `15-5 13 13 10 13 3 3 1 2`; AVA 2, REM/STR.
- **Rules/equipment:** Remote Presence, Courage, Dodge (+5), Mimetism (-3), Total Terrain; ECM Hacker (-3).
- **Option 1:** **18 / 0** — Boarding Shotgun, Chain-colt (PS=6 source modifier), PARA CC Weapon (-6).
- **Option 2:** **20 / 1.5** — Heavy Rocket Launcher, Light Shotgun, PARA CC Weapon (-6).
- **Option 3:** **24 / 1** — Red Fury, PARA CC Weapon (-6).
- **Option 4 FO:** **20 / 0** — Combi Rifle, Flash Pulse, PARA CC Weapon (-6); Forward Observer.

### Zayin Rebots — `zayin-rebots`

- **Stats:** `15-10 13 11 10 13 0 3 1 3`; AVA 1, REM/STR.
- **Rules/equipment:** Remote Presence, Courage, Total Reaction, Climbing Plus; 360º Visor.
- **Option 1:** **24 / 1** — HMG, PARA CC Weapon (-3).
- **Option 2:** **19 / 0** — Thunderbolt (+1B), PARA CC Weapon (-3).

### Warcors — `warcors-war-correspondents`

- **Stats:** `10-10 11 9 11 13 0 0 1 2`; AVA 1, LI; Irregular.
- **Option 1:** **3 / 0** — Flash Pulse, Stun Pistol, PARA CC Weapon (-3); 360º Visor.
- **Option 2:** **3 / 0** — same weapons; Sixth Sense.

### Yadu — `yadu`

- **Stats:** `15-5 15 13 11 14 3 6 1 2`; AVA 5, MI.
- **Rules/equipment:** Courage, Immunity (Shock), Number 2, NWI, Warhorse; Albedo (-6).
- **Option 1:** **28 / 0** — MULTI Rifle, E/Marat, Drop Bears, Heavy Pistol, CC Weapon.
- **Option 2:** **26 / 1.5** — Heavy Rocket Launcher, Submachine Gun, E/Marat, Heavy Pistol, CC Weapon.
- **Option 5:** **28 / 0** — MULTI Rifle, E/Marat, Disco Baller, Heavy Pistol, CC Weapon; Deactivator.
- **Option 6 Hacker:** **27 / 0.5** — Boarding Shotgun, E/Marat (+1B), Heavy Pistol, CC Weapon; Hacking Device with Carbonite (PS=6).
- **Option 7 FO:** **27 / 0** — MULTI Rifle, E/Marat, Flash Pulse, Heavy Pistol, CC Weapon; Forward Observer.
- **Option 8 NCO:** **34 / 1.5** — HMG, E/Marat, Heavy Pistol, CC Weapon; NCO.
- **Option 9 Lieutenant:** **28 / 0** — option-1 weapons; Lieutenant.

### Sophotects — `sophotects`

- **Stats:** `15-10 13 11 11 15 2 3 1 2`; AVA 2, MI.
- **Rules/equipment:** Courage, Engineer (ReRoll -3), Doctor, NWI, Immunity (Shock), Dodge (+2.5), Jump (+7.5); Deployable Cover, GizmoKit (+1B), MediKit.
- **Option 1:** **25 / 0** — Submachine Gun, Pulzar, Flash Pulse, D-Charges, Pistol, CC Weapon.
- **Option 3:** **32 / 0** — Combi Rifle, Pulzar, D-Charges, Armed Turret (Combi Rifle), Pistol, CC Weapon.
- **Option 4:** **30 / 0** — Submachine Gun, Pulzar, D-Charges, Armed Turret (Mk12), Pistol, CC Weapon.

### Rudras GunBots — `rudras-gunbots`

- **Stats:** `15-5 11 13 11 12 4 6 2 4`; AVA 2, REM/STR.
- **Rules/equipment:** Remote Presence, BS Attack (-3), BS Attack (SR-1), Courage, Immunity (AP), Tech-Recovery, Climbing Plus; ECM Hacker (-3), Repeater.
- **Option 2 — RUDRA FTO:** **35 / 0** — K1 Marksman Rifle, Pulzar, Panzerfaust, Heavy Pistol, PARA CC Weapon (-3). FTO.
- **Option 3:** **38 / 1** — Red Fury, Pulzar, Panzerfaust (+1SD), Heavy Pistol, PARA CC Weapon (-3). Not FTO.
- **Option 4 — RUDRA FTO:** **37 / 1** — Red Fury, Pulzar, Panzerfaust, Heavy Pistol, PARA CC Weapon (-3). FTO.

### Sharvara HoundBots — `sharvara-houndbots`

- **Stats:** `15-15 22 11 12 12 0 3 1 3`; AVA 2, REM/STR.
- **Rules:** Remote Presence, CC Attack (-6), Courage, Forward Deployment (+10), Dodge (+3/+5 as separate source entries), Natural Born Warrior, Mimetism (-3), Stealth, Super-Jump.
- **Option 1:** **17 / 0** — Light Shotgun, Heavy Riotstopper, E/Marat, DA CC Weapon (PS=7), PARA CC Weapon.
- **Option 2:** **19 / 0** — Adhesive Launcher Rifle, Light Shotgun, E/Marat, DA CC Weapon (PS=7), PARA CC Weapon.
- **Option 3:** **15 / 0** — Adhesive Launcher Rifle, Heavy Riotstopper, E/Marat, DA CC Weapon (PS=7), PARA CC Weapon.

### Yaksha Tacbots — `yaksha-tacbots`

- **Stats:** `15-5 14 13 10 13 4 3 1 2`; AVA 2, REM/STR.
- **Rules/equipment:** Remote Presence, Surprise Attack (-3), Camouflage (1 Use), Courage, Forward Deployment (+20), Mimetism (-3), Total Terrain; ECM Hacker (-3).
- **Option 1:** **23 / 0** — AP Submachine Gun, Light Flamethrower, Mine Dispenser (Shock), PARA CC Weapon (-6).
- **Option 2:** **25 / 0.5** — E/M Carbine (+1SD), Light Flamethrower, MadTraps, PARA CC Weapon (-6); Minelayer.
- **Option 3 Specialist:** **27 / 0** — Boarding Shotgun (+1SD), Light Flamethrower, Mine Dispenser (Shock), PARA CC Weapon (-6); Specialist Operative.
- **Option 4 Specialist:** **31 / 1** — Red Fury, Light Flamethrower, D-Charges, PARA CC Weapon (-6); Specialist Operative.

### Dr. Claire Lazhari — `dr-claire-lazhari-genephilosopher-and-optimate`

- **Stats:** `15-5 16 13 10 14 1 3 1 2`; AVA 1, LI; Non-Hackable.
- **Rules/equipment:** BS Attack (Continuous Damage), MediKit (PH=17), Dodge (+3 and +2.5 source entries), Immunity (Enhanced), NWI; Albedo (-3), MediKit.
- **Option 1 — CLAIRE LAZHARI:** **33 / 0** — Breaker Combi Rifle, Nanopulser (+1B), Disco Baller, Viral Pistol (+1B), PARA CC Weapon (-3); Doctor (2W). Not FTO, but legal in chart rows that name Claire without an FTO restriction.
- **Option 2 — CLAIRE LAZHARI FTO:** **33 / 0** — same weapons; Doctor (+3). FTO; required for Asuras and MAX-OP access.

### Dikpala Tacbots — `dikpala-tacbots`

- **Stats:** `15-10 13 11 10 13 0 3 1 2`; AVA Total, REM/STR.
- **Rules/equipment:** Remote Presence, Courage, Mimetism (-3); ECM Hacker (-3).
- **Option 1:** **13 / 0** — Combi Rifle, PARA CC Weapon (-3).
- **Option 2:** **21 / 1** — HMG, PARA CC Weapon (-3).
- **Option 3:** **19 / 1** — MULTI Sniper Rifle, PARA CC Weapon (-3).
- **Option 4:** **15 / 0** — Combi Rifle, PARA CC Weapon (-3); Commlink, Specialist Operative.
- **Option 5:** **13 / 0** — Submachine Gun, Akrylat-Kanone, PARA CC Weapon (-3); Repeater.
- **Option 6:** **15 / 0** — Combi Rifle, PARA CC Weapon (-3); MediKit, Paramedic.

## Fireteams

This section is authoritative for OSS Fireteam legality. The reverse index below is derivative.

### FT-01 — OperationS Fireteams

**Types:** Duo, Haris, Core  
**Required-source set:** at least one legal member from the `DIKPALA` / `DEVA (Dikpala)` required rows.

| Member | Unit ID | Required set | Min | Max | Counts as | FTO restriction | Allowed loadout IDs | Notes |
|---|---:|---|---:|---:|---|---|---|---|
| Dikpala Tacbots | 1898 | yes | 0 | 5 | Dikpala | — | all | native source row |
| Deva Functionaries | 109 | yes | 0 | 5 | Dikpala | — | all | required-choice alternative |
| CSU | 122 | no | 0 | 2 | — | — | all | — |
| Sharvara HoundBots | 1899 | no | 0 | 2 | Dikpala | — | all | — |
| Artalis Unit | 1771 | no | 0 | 1 | Dikpala | — | all | — |
| Danavas Hackers | 950 | no | 0 | 1 | — | — | all | — |
| Riksha Tacbots | 1769 | no | 0 | 1 | — | — | all | — |
| Dawon Tacbots | 1770 | no | 0 | 1 | — | — | all | — |
| Chandra Spec-Ops | 1922 | no | 0 | 1 | — | optional mode | optional-mode profiles | Spec-Ops placeholder |

### FT-02 — Samarthan Fireteams

**Types:** Duo, Haris, Core  
**Required-source set:** at least one legal member from `YADU`, `RIKSHA (Samarthan)`, or `DAWON (Samarthan)`.

| Member | Unit ID | Required set | Min | Max | Counts as | FTO restriction | Allowed loadout IDs | Notes |
|---|---:|---|---:|---:|---|---|---|---|
| Yadu | 1129 | yes | 0 | 5 | Yadu | — | all | native source row |
| Riksha Tacbots | 1769 | yes | 0 | 2 | Samarthan | — | all | required-choice alternative |
| Dawon Tacbots | 1770 | yes | 0 | 2 | Samarthan | — | all | required-choice alternative |
| Artalis Unit | 1771 | no | 0 | 1 | Samarthan | — | all | — |
| Sharvara HoundBots | 1899 | no | 0 | 1 | Samarthan; Yadu Troops | — | all | — |
| Kyra Sharma | 1897 | no | 0 | 1 | Samarthan | **FTO** | `1` | exact FTO row |
| Shakti | 1191 | no | 0 | 1 | Yadu Troops | — | all | — |
| Claire Lazhari | 1894 | no | 0 | 1 | — | — | `1,2` | chart does not say FTO here |
| Deva Functionaries | 109 | no | 0 | 1 | — | — | all | — |
| Satrah Unit | 1772 | no | 0 | 1 | — | — | all | — |
| Apsaras | 1174 | no | 0 | 1 | — | — | all | — |
| Chandra Spec-Ops | 1922 | no | 0 | 1 | — | optional mode | optional-mode profiles | Spec-Ops placeholder |

### FT-03 — Asuras Fireteams

**Types:** Duo, Haris

| Member | Unit ID | Required | Min | Max | Counts as | FTO restriction | Allowed loadout IDs | Notes |
|---|---:|---|---:|---:|---|---|---|---|
| Asuras | 584 | no | 1 | 3 | Asura | — | all | at least 1 Asura |
| Yadu | 1129 | no | 0 | 2 | Asura | — | all | — |
| Shakti | 1191 | no | 0 | 1 | Asura | — | all | — |
| Deva Functionaries | 109 | no | 0 | 1 | — | — | all | — |
| Claire Lazhari | 1894 | no | 0 | 1 | — | **FTO** | `2` | chart explicitly says FTO |
| Chandra Spec-Ops | 1922 | no | 0 | 1 | — | optional mode | optional-mode profiles | Spec-Ops placeholder |

### FT-04 — Bounty Hunters Fireteams

**Types:** Duo, Haris  
**Required-source set:** at least one legal member from `BOUNTY HUNTER` or `MOTORIZED BOUNTY HUNTER (Bounty Hunter)`.

| Member | Unit ID | Required set | Min | Max | Counts as | FTO restriction | Allowed loadout IDs | Notes |
|---|---:|---|---:|---:|---|---|---|---|
| Authorized Bounty Hunters | 49 | yes | 0 | 3 | Bounty Hunter | — | all | required-choice source |
| Motorized Bounty Hunters | 1565 | yes | 0 | 2 | Bounty Hunter | — | all | required-choice alternative |
| Miranda Ashcroft | 51 | no | 0 | 1 | Bounty Hunter | — | all | — |
| Father Lucien Sforza | 198 | no | 0 | 1 | Bounty Hunter | **FTO** | `2,3` | exact FTO profiles only |
| Deva Functionaries | 109 | no | 0 | 1 | — | — | all | — |
| Chandra Spec-Ops | 1922 | no | 0 | 1 | — | optional mode | optional-mode profiles | Spec-Ops placeholder |

### FT-05 — MAX-OP Fireteam

**Type:** Duo  
**Required-source set:** at least one legal member from `MARUT` or `MAXIMUS OPTIMATE (Max-Op)`.

| Member | Unit ID | Required set | Min | Max | Counts as | FTO restriction | Allowed loadout IDs | Notes |
|---|---:|---|---:|---:|---|---|---|---|
| Maruts | 585 | yes | 0 | 1 | — | — | all | required-choice source |
| Maximus (TAG) | 1720 | yes | 0 | 1 | Max-Op | — | all | required-choice alternative |
| Johnny Kao | 1892 | no | 0 | 1 | Max-Op | — | all | — |
| Claire Lazhari | 1894 | no | 0 | 1 | Max-Op | **FTO** | `2` | exact FTO profile only |
| Yadu | 1129 | no | 0 | 1 | — | — | all | — |
| Deva Functionaries | 109 | no | 0 | 1 | — | — | all | — |
| Artalis Unit | 1771 | no | 0 | 1 | — | — | all | — |
| Sharvara HoundBots | 1899 | no | 0 | 1 | — | — | all | — |
| Chandra Spec-Ops | 1922 | no | 0 | 1 | — | optional mode | optional-mode profiles | Spec-Ops placeholder |

### FT-06 — OPTIMATES Fireteam

**Types:** Duo, Haris, Core  
**Required-source set:** at least one legal member from `JOHNNY KAO`, `CLAIRE LAZHARI`, or `KYRA SHARMA FTO`.

| Member | Unit ID | Required set | Min | Max | Counts as | FTO restriction | Allowed loadout IDs | Notes |
|---|---:|---|---:|---:|---|---|---|---|
| Johnny Kao | 1892 | yes | 0 | 1 | Optimates | — | all | required-choice source |
| Claire Lazhari | 1894 | yes | 0 | 1 | Optimates | — | `1,2` | chart does not say FTO here |
| Kyra Sharma | 1897 | yes | 0 | 1 | Optimates | **FTO** | `1` | required-choice source; FTO only |
| Pilot-X Team | 1903 | no | 0 | 1 | Optimates | — | team profile | Pilot-X dependency still applies |
| Sharvara HoundBots | 1899 | no | 0 | 2 | — | — | all | — |

### Wildcards

| Unit | Unit ID | Max | Counts as / context | FTO/profile restriction | Notes |
|---|---:|---:|---|---|---|
| Rudras GunBots | 1197 | 2 | unrestricted chart Wildcard | **RUDRA FTO**, options `2,4` | may join any otherwise legal OSS family unless another rule prevents it |
| Arjuna Unit | 1178 | 2 | unrestricted chart Wildcard | **ARJUNA FTO**, options `1,7,10` | — |
| Samekh Rebots | 592 | 1 | unrestricted chart Wildcard | **FTO**, option `2` | — |
| Optimate Agent Maximus | 1862 | 1 | **Samarthan, Optimates only** | **FTO**, options `2,4` | context-limited Wildcard |
| John Hawkwood | 1556 | 1 | **Bounty Hunter only** | all normal OSS Hawkwood profiles | context-limited Wildcard |

## Unit → Fireteam access index

This reverse index resolves direct chart rows plus Wildcard access. Canonical tables above win if any inconsistency is found.

| Unit | Effective OSS Fireteam access | Profile restriction |
|---|---|---|
| Apsaras | Samarthan | all |
| Arjuna Unit | Wildcard into all OSS families | FTO options `1,7,10` only |
| Artalis Unit | OperationS; Samarthan; MAX-OP | all |
| Asuras | Asuras | all |
| Authorized Bounty Hunters | Bounty Hunters | all |
| Claire Lazhari | Samarthan; Asuras; MAX-OP; Optimates | Asuras/MAX-OP opt `2` only; Samarthan/Optimates opts `1,2` |
| CSU | OperationS | all |
| Danavas | OperationS | all |
| Dawon | OperationS; Samarthan | all |
| Deva | OperationS; Samarthan; Asuras; Bounty Hunters; MAX-OP | all |
| Dikpala | OperationS | all |
| Hawkwood | Bounty Hunters Wildcard | all |
| Johnny Kao | MAX-OP; Optimates | all |
| Kyra Sharma | Samarthan; Optimates | FTO opt `1` only |
| Marut | MAX-OP | all |
| Maximus, Optimate TAG | MAX-OP | all |
| Miranda Ashcroft | Bounty Hunters | all |
| Motorized Bounty Hunters | Bounty Hunters | all |
| Optimate Agent Maximus | Samarthan/Optimates Wildcard | FTO opts `2,4` only |
| Pilot-X Team | Optimates | team dependency applies |
| Riksha | OperationS; Samarthan | all |
| Rudra | Wildcard into all OSS families | FTO opts `2,4` only |
| Samekh | Wildcard into all OSS families | FTO opt `2` only |
| Satrah | Samarthan | all |
| Sharvara | OperationS; Samarthan; MAX-OP; Optimates | all |
| Shakti | Samarthan; Asuras | all |
| Sforza | Bounty Hunters | FTO opts `2,3` only |
| Yadu | Samarthan; Asuras; MAX-OP | all |
| Chandra Spec-Ops | optional-mode hooks in OperationS/Samarthan/Asuras/Bounty Hunters/MAX-OP | optional-mode only |

Units not listed in this reverse table have no main-chart Fireteam access in the pinned OSS chart.

## Dependencies, exclusivity, and composite-profile notes

### Posthumans

- Select 2–3 Proxy models from the Posthuman record.
- Only one Proxy per model.
- All selected Proxies are in the same Combat Group.
- Together they count as one G:Jumper trooper for the Army relation.

### Pilot-X Team

- Requires exactly one Pilot-X when RacerBot Mk-III models are selected.
- Allows 0–2 RacerBot Mk-III.
- RacerBot Mk-III cannot be selected independently of Pilot-X.
- All members of the Pilot-X Team must be in the same Combat Group.

### Maximus exclusivity

- `Maximus, Optimate and HexaDome Legend` (`1720`) and `Optimate Agent Maximus` (`1862`) are source-linked as mutually exclusive normal-roster versions.
- The Maximus TAG is also source-linked to a separate Reinforcement counterpart; Reinforcement data is not merged into this main roster.

### Parent/peripheral and alternate-state handling

- Marut includes **Karkata**.
- Arjuna profiles may include **KiranBot 1/2**.
- Dart option 4 includes **Sharvara_K-9**.
- Deva profiles may include **Devabot**.
- Optimate Agent Maximus non-FTO profiles may include **Minimus**.
- Maximus TAG has an **Operator Maximus** alternate state.
- Tarkshya has an **Interception Wing** primary state and **Tarkshya Operator** alternate state.
- Pilot-X Team contains its dependent RacerBot Mk-III models inside the same logical team record.
- These subordinate/alternate profiles are not extra independent roster entries unless their parent relation expressly permits selection.

## Reinforcements boundary

The Army source links OSS to Reinforcement army **799**. Reinforcement units, profiles, and any Reinforcement Fireteam chart are a separate force context and are not mixed into the canonical main OSS Fireteam definitions above.

## Validation notes

- Source snapshot: `n5/operations/7.26246.159.json` at `massayoshi/infinity-army-backup` commit `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b`, blob `a37001ab696082155005eea050bbf013c702a7ac`.
- Army version: `7.26246.159`.
- Army ID: `703`; parent ALEPH ID: `701`; Reinforcement army ID: `799`.
- Fireteam chart limits verified as Core `1`, Haris `1`, Duo `256`.
- Six named/direct Fireteam families plus a Wildcard table are represented.
- Required-choice semantics are preserved rather than interpreting every `required: true` row as simultaneously mandatory.
- Exact chart-level FTO restrictions are preserved for Kyra, Claire, Sforza, Rudra, Arjuna, Samekh, and Optimate Agent Maximus.
- Context-limited Wildcards are preserved for Optimate Agent Maximus and Hawkwood.
- The standard roster count excludes Chandra Spec-Ops, ALEPH Team-Ops, and generic `factions: []` Soldier-of-Fortune catalog records.
- Faction-listed mercenary-origin records are retained when the OSS source explicitly assigns faction `703`.

## Mission specialists — N5.3 apex and value cross-reference (2026-10-23)

**Mission benchmark:** **Posthuman Mk.1 Doctor/Engineer 13, Mk.5 FO13/.5** give G:Jumper slot-efficient task coverage; don't treat them as two independent Orders. **Dasyu FO29/Naga FO25** are Camo scoring; **Deva KHD20/FO21** WIP15 NWI, **Artalis Doctor/Engineer23** is NCO frontline support, **Riksha FO20**, **Daleth FO15/TA18** provides cheap mobile sensor/button work. **Asura HD+** combines gun/hacker/score but can starve independent routes. Source MAX-OP requirements still govern linked scoring.

[Cross-game specialist and button-pusher tiers](../../notes/list-building/mission-specialists-and-button-pushers-apex-value.md). **Current profile options and Fireteam chart in this file remain authoritative.**

## Active-turn gunfighter cross-reference (2026-10-23)

**Active-turn shooting choices:** **Posthuman Mk.4 HMG30/1.5** is an extraordinary BS14/ARM5/2W **non-TAG** gun only inside its required **2–3 Proxy G:Jumper package**; Mk.1 Engineer can make the package useful even if the HMG fails. **Asura AP Spitfire61/1.5** wins anti-armor/Mimetism mids, while **HD+ MULTI MMR63/0.5** is a different hack/mission build; **Marut86/1.5** is the much more expensive **TAG** long-lane MSV2 solution. **A 2026 OSS podcast disagreement:** Asura revision raised practical floor, some say reduced ceiling; Mk.4 remains an efficient purchased package. [Gunfighter combat tiers, TAG separated](../../notes/list-building/active-turn-gunfighters-apex-and-value.md).

## TAG tactical cross-reference (2026-10-23)

**Marut** is the premier MSV2 big gun, with an optional Strategos LT price/risk tradeoff. **Maximus TAG** is a tougher close-range/CC answer but gives up Marut's visor/long-range efficiency. Both fill high-priced required-choice slots in their permitted MAX-OP team; check canonical members and do not infer extra legal links from name alone. OSS's REM/specialist support can justify either without replacing the objective plan.

Across all factions, compare **apex power** separately from **points value**, counterplay and mission fit: [N5.3 TAG guide](../../notes/list-building/tags.md). The current unit profiles and canonical Fireteam chart above take precedence over tactical opinions.

## Vehicle (VH) tactical cross-reference (2026-10-23)

**Tarkshya AVA1:** **34/0 MULTI MMR+Chain Rifle(+1B)** gives OSS exceptional low-SWC **MSV1/Mimetism(-6) aerial angle creation** and retains a strong **post-shell FO(+1SD) Operator** after the correct transition. **38/0 MMR+AP SMG** covers close armor, **41/1.5 MULTI Red Fury** takes valuable SWC. The **Garuda is a REM**, not a VH (despite aerial-style movement), and RacerBots are REMs. The **2025 global VH ranking predates Tarkshya**; high tier is provisional, based on the pinned current roster and OSS tactical note.

See [VH apex/value tier list and matchup guide](../../notes/list-building/vehicles-vh.md). **Current profiles, AVA and canonical Fireteam chart above remain authoritative.**

## Hacker and KHD tactical cross-reference (2026-10-23)

**Asura HD+ + Trinity(+1SD) 63/0.5** (or **LT(+1 Order) 67/0** where printed) is an apex **WIP15, ARM5/NWI, MSV3** active and reactive cyber duelist with White Noise. **Danavas HD+ + Oblivion(+1B) 22/0.5** is superior *cost value* for stationary network/visors. **Apsaras KHD + Firewall(-3)/Deployable Repeater 17/0**, optional TAGCom18 or RemDriver20, is a highly efficient defensive/specialist hybrid; **Deva KHD 20/0**, **Satrah KHD 20/0** and **Naga KHD27/0** provide different cover/mission plans. **Shakti KHD 35/0** brings a real gun and survival at higher cost. An **Asura / Danavas / Apsaras** combination covers anti-HI, White Noise and Trinity with redundancy; the expensive Asura is not automatically best value.

See the [cross-game apex/value Hacker/KHD tier guide](../../notes/list-building/hackers-and-killer-hackers.md). **The sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative; device upgrades are profile-specific.**


## Cheerleader / Order-generation tactical cross-reference (2026-10-23)

For cross-faction **apex** and **points-value** rankings, the Order types, situational counterexamples and transcript-backed disagreements, see [Cheerleaders and Order Generators — N5.3](../../notes/list-building/cheerleaders-and-order-generators.md). Roster profiles/AVA/Fireteam legality above take precedence.

- **6pt Netrod**: cheapest Regular pool Order where roster-legal, but its mandatory deployment and stationary non-combat body are a risk
- **Authorized Bounty Hunter**: choose cheap Regular profiles for Booty and a close-range threat; do not assume all Bounty Hunter variants have the same price or link access

**List-building test:** count *transferable* Regular Orders by Combat Group after deployment; include required link members/command enablers, physical DZ footprint, and the unit's actual ARO/mission contribution. Do not treat Irregular, Tactical, Lieutenant or Peripheral activations as interchangeable generic Orders.


## ARO apex/value cross-reference (2026-10-23)

See [ARO units: N5.3 apex/value tiers, hidden-versus-visible and deployment/matchups](../../notes/list-building/aro-units-apex-and-value.md). The **current profile details here** control exact cost/SWC, Training and Fireteam eligibility; do not import another faction's link or specialist upgrades.

- **Zayin Thunderbolt TR** — 19pt/0SWC reactive volume and regular Order; protected Engineer/Yudbot route makes defeating it a repeat job
- **Riksha HRL** — 20pt/1.5SWC launcher, inexpensive but limited durability; Fireteam source permissions control bonus dice
- **Samekh FTO ML** — linked launcher only when the canonical chart permits this precise profile; Guided version is not automatically a linked ARO
- **Dikpala Mimetism Repeater/akrylat** — backstop/Fireteam troop with reactive control and support, not a generic passive TR piece
- **Posthuman/Proxy screen** — distributed positions and cheap Engineer recovery can outvalue a single static sniper; remember G: Jumper ARO restrictions

**Choose by circumstance:** a hard long gun matters only when the opponent must cross its arc; cheaper mines, Camo markers, templates, Flash, DTWs and hacking force movement or risk without committing an entire attack plan. Budget a second layer and preserved counterattack, check pie-slicing, hidden Order cost, anti-visual bypass and repair routes.

## N5.3 midfield area denial / speed bumps (tactical synthesis)

**Highest-threat passive mines:** **Dasyu 30/.5 Viral Minelayer (2)** combines Hidden/Infiltration(ReRoll)/Mimetism(-6), but Viral is matchup-sensitive and Hidden loses its Order. **Naga 26/.5 Monofilament Minelayer** punishes elite passage (25/.5 Shock is cheaper for ordinary troops); **Kinnara 25/.5** adds E/M Mine/Decoy(2)/Sensor; **Yaksha 25/.5** brings FD(+20) ARM4 MadTraps plus E/M Carbine. **Disagreement:** durable Yaksha vs cheaper RacerBots/Pilot-X or Naga/Dasyu/Dart—buy the body only when its defensive position and weapon reach actually add value. **Yaksha 23/0 Mine Dispenser is not a zero-Order Minelayer**.

[Cross-game apex/value, matchups, and video/podcast disagreements](../../notes/list-building/midfield-area-denial-and-speed-bumps-apex-value.md). Qualitative tactics; the unit profile tables above remain authoritative.

## Doctor / Engineer / Recovery cross-reference (2026-10-23)

**Sophotect25 WIP15 + Yudbot3** is excellent mixed **Posthuman/REM + Asura** recovery: 75% first-roll WIP and fast 15-10 reposition. **Parvati36** earns its higher price when **Doctor(2W), advanced Engineer and mobility** all matter. **Proxy Mk.1 Engineer** adds repair and objective capability *inside the paid legal 2–3 Proxy/G:Jumper package*, not a standalone extra Order. [Recovery support tiers, probabilities and transcript disputes](../../notes/list-building/doctors-engineers-and-recovery-apex-value.md).
