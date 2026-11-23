# Varuna Immediate Reaction Division — Fireteams

**Varuna guides:** [Overview](varuna-overview.md) · [Sectorial Inventory](varuna-inventory.md) · [Listbuilding](varuna-listbuilding.md) · [Fireteams](varuna-fireteams.md) · [References](varuna-references.md) · [Unit analyses](units/).

**Authority:** [Pinned N5.3 roster and canonical chart](../../../sectorials/panoceania/varuna-immediate-reaction-division.md#fireteams). Exact audited rows below are reproduced from the roster for convenient reference; the roster wins if they diverge.

## Particularly strong or unusual Fireteams

**N5.3 audited profiles and FT levels (19 November 2026):** [Open the exact 2–5-member Fireteam selections, option IDs, individual/total pts/SWC, FT levels, restrictions, and evidence notes](../../../sectorials/panoceania/varuna-immediate-reaction-division.md#recommended-fireteam-compositions--n53-audited). This pinned-roster-based table is the detailed reference; the examples below remain qualitative tactical commentary.

Best starting tests: **four Fusiliers + Quinn Core 73/0.5 (FT5)** for TAG-support economy; **Patsy + Helot FTO LRL + Helot FTO Red Fury three-member Core 57/1 (FT3)** for Helot command/control; **Kamau HRL + two foot Montesa FTO + Pathfinder four-member Undertow Core 80/1.5 (FT3)** for midfield attack. The Patsy/Helots three-member group consumes the **Core** slot if you simultaneously field an Undertow Haris; a second Haris would be illegal.


- **Patsy + two Helot FTO Haris:** **Patsy Garnett 34 + two 10-point Helot FTO LRL = 54/0**, with **FT Master (Helots)** converting the two otherwise Irregular Helots at the *next Order Count* while a valid team exists. Useful mission/ARO shell, not cheapest possible Order farming. Non-FTO Camo Helots cannot join.
- **Undertow Core/Haris:** **Kamau or Varuna ORC** required-choice gun, with **foot Montesa FTO** for specialist assault and **Varuna Machinist** counting as Kamau; pressure can continue after the first shootout.
- **Cavalry Duo:** **Squalos Mk-II or motorized Montesa** is required-choice, with legal **Kamau/Bulleteer** support; a mobile alternative to a purely static Kamau shell.
- **Forward Montesa Duo:** exactly **two foot Montesas**; don't replace either with the motorized profile.

## Fireteam chart limits

| Constraint | Value |
|---|---|
| Core | 1 |
| Haris | 1 |
| Duo | unlimited (`256` in Army chart) |
| Main/Reinforcement mixing | not merged; use the separate Reinforcement chart |

## Fireteams

### FT-VAR-01 — Varuna Fireteams

**Types:** Core, Haris, Duo

| Member | Unit ID | Min | Max | Required choice | Counts as | FTO restriction |
|---|---:|---:|---:|---|---|---|
| Fusilier | 1 | 0 | 5 | Yes | — | — |
| Helot Militiaman | 1222 | 0 | 2 | Yes | — | **FTO options 1, 3, 4 only** |
| Kamau | 48 | 0 | 3 | No | — | — |
| ORC Varuna Division | 5 | 0 | 2 | No | — | — |
| Bipandra | 46 | 0 | 1 | No | Fusilier | — |
| Indigo | 1912 | 0 | 1 | No | Spec-Ops | Optional Spec-Ops mode |

Fusilier and Helot FTO are both marked `required: true` in the structured chart; they form the source required-choice set rather than this reference asserting that both unit types must be present simultaneously.

### FT-VAR-02 — Undertow Fireteams

**Types:** Core, Haris, Duo

| Member | Unit ID | Min | Max | Required choice | Counts as | FTO restriction |
|---|---:|---:|---:|---|---|---|
| ORC Varuna Division | 5 | 0 | 5 | Yes | Undertow | — |
| Kamau | 48 | 0 | 5 | Yes | Undertow | — |
| Knight of Montesa | 28 | 0 | 2 | No | Undertow | **FTO option 5 only** |
| Machinist Varuna Division | 15 | 0 | 2 | No | Kamau | — |

ORC Varuna and Kamau are both marked `required: true` in the structured chart; they form the source required-choice set rather than requiring both unit types simultaneously.

### FT-VAR-03 — Cavalry Fireteams

**Type:** Duo

| Member | Unit ID | Min | Max | Required choice | Counts as | FTO restriction |
|---|---:|---:|---:|---|---|---|
| Squalos Mk-II | 1651 | 0 | 2 | Yes | — | — |
| Motorized Knight of Montesa | 1209 | 0 | 2 | Yes | — | — |
| Bulleteer | 35 | 0 | 1 | No | — | — |
| Kamau | 48 | 0 | 1 | No | — | — |

Squalos Mk-II and Motorized Montesa are both marked `required: true` in the structured chart; they form the source required-choice set.

### FT-VAR-04 — Forward Montesa Fireteams

**Type:** Duo

| Member | Unit ID | Min | Max | Required | Counts as | FTO restriction |
|---|---:|---:|---:|---|---|---|
| Knight of Montesa | 28 | 2 | 2 | No | — | none in source row |

The source row requires exactly two Knights of Montesa and does not carry an FTO marker. This is distinct from the FTO-restricted Montesa row in Undertow.

### Wildcards

All rows below are in the chart's **Wildcards** row. Parenthetical values are Counts-as labels, not join-scope restrictions.

| Wildcard | Unit ID | Max | Counts as | FTO/profile restriction |
|---|---:|---:|---|---|
| Pathfinder Dronbot | 16 | 2 | — | all |
| Clipper Dronbot | 18 | 1 | — | **FTO option 5 only** |
| Richard Quinn | 1490 | 1 | Fusilier, Kamau | all Quinn loadouts |
| Uma Sørensen | 1491 | 1 | Fusilier, Kamau | **FTO options 2, 3, 4 only** |
| Patsy Garnett | 1225 | 1 | Undertow, Helot | all |

Wildcard status does not remove the native minimum/required-choice conditions of the Fireteam being joined.

## Recommended Fireteam compositions — N5.3 audited

**Non-canonical tactical overlay** checked against the pinned N5.3 chart and profiles (2026-11-19). Every row is an **alternative**, not a claim that the same models are simultaneously available for every proposed link. Exact pinned options and individual totals are in pts/SWC. FT level is based on same-Unit or chart *Counts-as* equivalence, **not raw team size** ([N5.3 bonuses](https://infinitythewiki.com/Fireteam_Bonuses)): FT2 BS Attack (+1 SD), FT3 +3 Discover/+1 Dodge, FT4 +1 BS, FT5 Sixth Sense.

**Legality checklist:** 1 Core, 1 Haris, unlimited Duos. *Varuna* needs **Fusilier or Helot FTO options 1/3/4** required-choice; *Undertow* needs **Kamau or Varuna ORC**; *Cavalry Duo* needs **Squalos Mk-II or motorized Montesa**; *Forward Montesa Duo* uses exactly **two foot Knights of Montesa**, different from motorized. Foot Montesa only **FTO option 5** in Undertow; Machinist counts as Kamau there. Patsy counts as Helot/Undertow but does not remove the Varuna Helot/Fusilier or Undertow ORC/Kamau requirement; Clipper is Wildcard **FTO option 5** only. When running Patsy + two Helots and another Undertow **Haris**, assign the Helot trio as a **three-member Core**, not a second Haris. FT Master (Helots) is conditional; it does not make every irregular Helot elsewhere a regular Order.

| Priority | Exact members (pinned option: individual pts/SWC) | Fireteam / size | FT level | Total pts/SWC | Benefit / caveat | Evidence |
|---|---|---|---|---:|---|---|
| **Best affordable FT5 TAG-support Core** | Fusilier Hacker (opt 6: 15/0.5)<br>Fusilier Paramedic (opt 9: 12/0)<br>Fusilier basic (opt 1: 10/0)<br>Fusilier basic (opt 1: 10/0)<br>Quinn FO/MSV1 (opt 1: 26/0) | Varuna Core · 5 | **FT5** | **73/0.5** | Four Fusiliers + Quinn (counts as Fusilier) deliver FT5 and retain budget for independent Cutter/Squalos. | [Report #203](../../battle-reports/201-210-n5-battle-report-tactical-analysis.md): this five-body unit mix explicitly fielded; modern options reconstructed. |
| **Best mixed midfield four-body Core** | Kamau HRL/MSV1 (opt 5: 23/1.5)<br>Foot Montesa FTO Blitzen/Paramedic (opt 5: 20/0)<br>Foot Montesa FTO Blitzen/Paramedic (opt 5: 20/0)<br>Pathfinder Tactical Awareness (opt 2: 17/0) | Undertow Core · 4 | **FT3** | **80/1.5** | Kamau and two Montesa FTO count as Undertow; Pathfinder is separate, so four members = FT3. | [Report #019](../../battle-reports/011-020-n5-battle-report-tactical-analysis.md): played Kamau/Montesa/Pathfinder shape; N5.3 profiles rebuilt. |
| **Best Helot command/control Core** | Helot FTO LRL (opt 4: 10/0)<br>Helot FTO Red Fury (opt 3: 13/1)<br>Patsy FT Master (opt 1: 34/0) | Varuna Core · 3 | **FT3** | **57/1** | Two Helot FTO and Patsy (counts as Helot) give FT3; FT Master (Helots) Order conversion is conditional. | [Report #226](../../battle-reports/221-230-n5-battle-report-tactical-analysis.md): played unit trio; use **Core 3** if also running one Undertow Haris. |
| **Best long-range Undertow Haris** | ORC Feuerbach (opt 13: 36/1.5)<br>Kamau HRL/MSV1 (opt 5: 23/1.5)<br>Kamau MSV2 MULTI Sniper (opt 6: 29/1.5) | Undertow Haris · 3 | **FT3** | **88/4.5** | ORC and two Kamau all count as Undertow (FT3), combining Feuerbach and two different ARO ranges. | [Report #226](../../battle-reports/221-230-n5-battle-report-tactical-analysis.md): three unit types explicitly reported together; modern options rebuilt. |
| **Best economy defensive Kamau Duo** | Kamau MSV2 MULTI Sniper (opt 6: 29/1.5)<br>Varuna Machinist Engineer (opt 3: 17/0) | Undertow Duo · 2 | **FT2** | **46/1.5** | Kamau MSV2 sniper plus Machinist (counts as Kamau) yields FT2, real Engineer recovery and spare Haris. | [Report #019](../../battle-reports/011-020-n5-battle-report-tactical-analysis.md): Kamau sniper + Machinist Duo played; current options reconstructed. |
| **Best TAG/specialist Cavalry Duo** | Squalos MULTI HMG NCO (opt 3: 66/1.5)<br>Pathfinder Tactical Awareness (opt 2: 17/0) | Cavalry Duo · 2 | **FT1** | **83/1.5** | Squalos MULTI HMG NCO paired with Tactical Awareness Pathfinder scores and repairs support indirectly; mixed FT1. | [Report #019](../../battle-reports/011-020-n5-battle-report-tactical-analysis.md): alternative list reports Squalos + Pathfinder Duo; modern options. |
| **Best cheap mobile Cavalry Duo** | Motorized Montesa Paramedic (opt 4: 23/0)<br>Kamau FO/Sensor (opt 7: 23/0) | Cavalry Duo · 2 | **FT1** | **46/0** | Motorized Montesa Paramedic provides mobility; Kamau FO provides sensors/longer scoring presence; FT1. | Constructed [N5.3 chart](https://github.com/ACParadox/Infinity/blob/main/sectorials/panoceania/varuna-immediate-reaction-division.md#fireteams) recommendation. |
| **Best forward specialist Duo** | Foot Montesa FD Red Fury (opt 2: 32/1.5)<br>Foot Montesa FD Paramedic (opt 3: 26/0) | Forward Montesa Duo · 2 | **FT2** | **58/1.5** | The actual two **foot** Montesas share the same unit and provide FT2; neither is the motorized S4 variant. | Constructed current-chart recommendation. |
| **Best 5-body elite anti-armor Core** | Kamau HRL/MSV1 (opt 5: 23/1.5)<br>Kamau MSV2 MULTI Sniper (opt 6: 29/1.5)<br>Kamau Tactical Awareness Paramedic (opt 4: 25/0)<br>ORC Feuerbach (opt 13: 36/1.5)<br>ORC Firewall TinBot BSG (opt 14: 28/0) | Undertow Core · 5 | **FT5** | **141/4.5** | Three Kamau with two ORC (all Undertow-equivalent) make FT5, but use substantial SWC and points. | Constructed current-chart apex skew; not the default efficient list. |

**Evidence boundary:** Reports #019, #203 and #226 support the linked **unit architecture**; some examples were played in *different army lists*. Option numbers/prices here are modern reconstructions, not postdated claims about those historical games. The [Varuna guide](varuna-overview.md) and [Brookhurst faction discussion](https://www.youtube.com/watch?v=WOvaahZlyQE) provide context, not confirmation of exact member options.

## Unit → Fireteam access index

## Fireteam architectures

The strongest current lesson is:

> **Do not start a Varuna list by deciding on a five-model Core. Start with roles and build the smallest team that improves them.**

### Kamau + Montesa Undertow

This is probably the most characteristic N5 Varuna pairing.

The division of labour is clean:

- Kamau provides the precision ranged piece;
- Montesa provides durability, specialist capability and Blitzen threat;
- the team can move rather than existing only to provide bonuses to one sniper.

This is particularly attractive when the rest of the army contains independent midfield and counterattack pieces.

---

### ORC + Kamau / Montesa package

Use when the Fireteam itself is supposed to advance.

Typical roles:

- ORC = durable leader / active gun;
- Kamau = precision / MSV / specialist / secondary gun;
- Montesa = resilient specialist / E/M threat;
- cheaper utility body = keep the team from becoming a giant points sink.

Do not fill every legal slot with an expensive elite model unless each one solves a different problem.

---

### Fusilier + Kamau Duo

A useful low-cost architecture when you want the Kamau gun without buying a full defensive brick.

Use when:

- the Kamau mainly needs mobility / team support;
- the list wants to spend points on Zulu, Montesa, ORC, TAG or midfield pieces instead;
- a larger team would be mostly filler.

---

### Montesa-focused teams

Advanced Montesa Fireteam access makes it reasonable to build around the Montesa as more than a support model.

Use when:

- mission scoring and resilient movement matter;
- the table is dense enough that a durable close/mid-range team is preferable to a static sniper package;
- you want Blitzen / E/M deterrence integrated into the main team.

---

## Battle-report-derived Fireteam and army spines (2026-11-03)

The [current Varuna Fireteam chart](../../../sectorials/panoceania/varuna-immediate-reaction-division.md#fireteams) allows **one Core, one Haris and unlimited legal Duos**. Historical video compositions are tactical evidence, **not substitutes for profile-level N5.3 legality**. The Undertow family needs an ORC or Kamau required-choice unit; linked foot Montesa must be **FTO option 5**.

- **Four-person Kamau/Montesa/Pathfinder Core — [#019 CanCon 2026](../../battle-reports/011-020-n5-battle-report-tactical-analysis.md):** a **Kamau HRL (alternative list: HMG) + two Knights of Montesa FTO + Pathfinder Tactical Awareness**. The player used this four-body attack structure with a separate **Kamau MULTI Sniper + Machinist** defensive Duo, or a **Patsy Garnett + two Helot FTO** defensive trio in the other list. The **Squalos Mk-II + Pathfinder Duo** is another played variant and fits the current *Cavalry* family when Squalos is the required-choice member and Pathfinder joins as Wildcard. These are **alternative lists**; do not duplicate the same Pathfinder across two formations.
- **Mixed five-person Core — [#011 MEGA 2025](../../battle-reports/011-020-n5-battle-report-tactical-analysis.md):** **ORC Lieutenant + Machinist + one foot Montesa FTO + two Tactical Awareness Pathfinders** (1+1+1+2 = five). Also described were a **Kamau HMG + Montesa FTO Duo** and a **Kamau MULTI Sniper + Quinn Duo**. In #011's **other** list the Core was **two Helot FTO + ORC Lieutenant + Patsy Garnett** (four), with a fifth Fusilier only a **possible addition**, not a verified deployed member. These are **two independent rosters**.
- **Cheap five-model Fusilier Core + two unlinked TAGs — [#203 Area of Interest](../../battle-reports/201-210-n5-battle-report-tactical-analysis.md):** **Fusilier Hacker + Fusilier Paramedic + two basic Fusiliers + Richard Quinn**, explicitly fielded as a **five-body Core**, plus separate **Cutter Camo TAG**, **Squalos Mk-II**, **Machinist/Palbot**, **Zulu-Cobra** and other utility. The **6–4** result rewarded zone control and cheap Camo weight; neither TAG joined the Core. Consider when the primary problem is **surviving objective Specialists**, not merely winning a shooting duel.
- **Two distinct three-body links — [#226 custom Crossing Lines](../../battle-reports/221-230-n5-battle-report-tactical-analysis.md):** **Patsy + Helot FTO SMG/Light Rocket Launcher + Helot FTO Red Fury**, supported by a separate **ORC Feuerbach + Kamau HRL + Kamau Sniper Haris**; Cutter NCO independent. **To field both three-body teams simultaneously under N5.3, assign the Patsy/Helots group to the single Core slot (as a three-model Core), not a second Haris.** This was a **one-combat-group, mandatory-TAG** event ending in concession amid a Line-of-Fire disagreement, **not an ordinary ITS efficiency trial**. Under N5.3, use eligible **Helot FTO options 1/3/4** and the actual ORC/Kamau Undertow anchor.

**List decision:** choose **Kamau/Montesa/Pathfinder Core of four** for aggressive midfield reach, **Fusilier/Quinn Core of five** for a cheaper TAG-support shell, or **Patsy/Helots with an ORC/Kamau Haris** when you want distinct attack and defensive lanes. Avoid merging choices from different published lists into a supposedly played six- or seven-person Fireteam. **No Chain of Command** exists in current Varuna; an attacking Lieutenant requires real protection, not a fictional Quinn/CoC backup.

**Terminology:** the canonical chart calls the two-foot-Montesa family *Forward Montesa*, not Advanced Montesa. The FTO-only restriction applies to Undertow, not the Forward Montesa Duo.
