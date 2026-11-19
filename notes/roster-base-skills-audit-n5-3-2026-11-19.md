# N5.3 roster base-skill reconciliation — 19 November 2026

## Scope and authority

This is a **focused cross-roster audit of NCO and Forward Observer**, initiated after the Scots Guard base-skill transcription defect. It is **not** a complete inventory of every shared skill, weapon, equipment item, skill parameter, or all loadout-specific overrides.

- **Scope:** all **45** main `sectorials/<parent>/<army>.md` roster references on `main`, covering vanilla armies, sectorials and NA2.
- **Primary source:** the exact faction-specific `massayoshi/infinity-army-backup` GitHub JSON revision recorded in each roster's provenance: `n5/<army-slug>/<army_source_version>.json` at its stated commit. The file version/commit varies among armies.
- **Corroboration:** [InfinityDB pinned normalization](https://github.com/frankysan/InfinityDB), official [October 2025 Army update](https://infinityuniverse.com/en/news/army-update-october-25), and N5.3 rules as necessary.
- **Source fields:** `units[].profileGroups[].profiles[].skills` for underlying/base-profile skills; `units[].profileGroups[].options[].skills` (and applicable `units[].options[]`) for additional selected-loadout effects. Empty loadout skill arrays **do not negate** the base skill.
- **Cross-reference identifiers in the pinned Army source:** `59` = Forward Observer; `211` = NCO. These IDs were reconciled against named units and existing documented skills rather than inferred from an empty option field.

## Verified omissions and repairs

| Roster / guide | Verified source behavior | Correction |
|---|---|---|
| [Kosmoflot](../sectorials/ariadna/kosmoflot.md), [Caledonia](../sectorials/ariadna/caledonian-highlander-army.md) | Scots Guards have **NCO + Forward Observer** on the base profile; only eligible **FTO** options may enter their respective legal Fireteams | The existing pinned roster corrections were confirmed; [Kosmoflot reference analysis](factions/references/kosmoflot_refs.md) and [Caledonian references](factions/references/caledonia_refs.md) no longer deny NCO |
| [Vanilla ALEPH](../sectorials/aleph/aleph.md) | **Tarkshya Operator alternate state** has **Forward Observer (+1SD)**, but the primary **Tarkshya Vehicle does not** | Explicit Operator-versus-Vehicle distinction added; [Operations Subsection](../sectorials/aleph/operations-subsection.md) already documented the Operator skill |
| [Morat Aggression Forces](../sectorials/combined-army/morat-aggression-forces.md) | **Bultrak TAG** has **NCO** in its base skills; **Rakdron does not inherit it** | Added to the roster and [Morat tactical guide](factions/morat-aggression-force.md) |
| [Vanilla Haqqislam](../sectorials/haqqislam/haqqislam.md) | **Hassassin Nadhir** has **Forward Observer** on its base profile across its five loadouts | Added to the roster and [Haqqislam guide](factions/vanilla-haqqislam.md) |
| [Vanilla Nomads](../sectorials/nomads/nomads.md) | **Meteor Zonds** have **Forward Observer** on both loadouts | Added to the roster |
| [Vanilla Nomads](../sectorials/nomads/nomads.md) | **Π-Well FTO component** has **Forward Observer**; do not attribute it to Zoe or to separate Π-Well Sync profile | Added component-specific qualifier |
| [Vanilla Nomads](../sectorials/nomads/nomads.md) | **Szalamandra TAG** has **NCO**; Robbybot does not. **Gator and Szalamandra both have NCO**, while Gator additionally offers Tactical Awareness | Corrected the roster and [Vanilla Nomads comparison](factions/vanilla-nomads.md) |

## Coverage, exceptions and limitations

- All 45 roster references were considered against pinned source declarations of base-profile `NCO` and `Forward Observer`. Textual matching of unit sections was supplemented by manual inspection where unit names/headings differed.
- Checked unmatched names explicitly, including Knauf (Kestrel), Emily Handelman (White Company), Vidocq (Torchlight), Wèibīng (Imperial Service), and Bìxié/Sulyong/Wèibīng (White Banner). Their documented NCO/FO assertions do not require correction from this focused audit.
- [Vanilla Yu Jing](../sectorials/yu-jing/vanilla-yu-jing.md) is already marked `status: partial` because the full loadout tables are not yet inlined. Its pinned source has **Bìxié: NCO + FO**, **Sulyong: NCO**, and **Wèibīng: FO**; absence of these entries in the compact roster index is a known coverage limitation, not evidence of missing Army capabilities.
- **No claim of a complete all-skill audit is made.** Other underlying skills (e.g., Chain of Command, Doctor/Engineer, hacking devices, Tactical Awareness, Camouflage/marker/deployment, vision and terrain modifiers), equipment, and composite-profile inheritance still require a separate complete ID-resolved comparison against each `profileGroups[].profiles[]` and `options[]` record.
- A unit with multiple profile groups or component states must be compared **per group**, not by unioning every skill into a fictitious all-unit profile. The Tarkshya Operator and Π-Well FTO cases demonstrate why.
- Future roster refreshes and audits must follow [AGENTS.md](../AGENTS.md), using the pinned GitHub Army JSON as the primary source and recording any profile-specific scope or uncertainty.

## Result

The **confirmed NCO/Forward Observer omissions identified in this focused pass** are corrected in the affected roster and tactical documents. Do not infer that all other shared skills have been independently certified by this work.
