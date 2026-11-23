# Padre-Inquisidor Mendoza — Military Orders (Infinity N5.3)

**Verdict: Mendoza FTO 40/0 — B+ generally, A− when his TinBot and elite short-range shooting are both needed; Heavy Shotgun + Forward Deployment (+8") 40/0 — B+ / situational A− as an independent hunter; MULTI Rifle + Forward Deployment (+8") 45/0 — B / usually skip. No profile is mandatory.** Mendoza's distinctive job in an army already saturated with close-range knights is **hunting difficult gunfighters and punishing tough targets with Continuous Damage**, backed by **Mimetism (−6), ARM4, W2, and genuinely dangerous DA close combat**. The 40pt FTO compresses that offense with **Firewall (−3) and Number 2**; it does **not** make him a Specialist or a Hospitaller-equivalent. **Hawkins BSG 26 is the better default-value close assault/scoring pick**, while Mendoza is the specialist-purpose premium killer.

**Sources:** [Pinned Military Orders N5.3 profiles](../../../../sectorials/panoceania/military-orders.md#padre-inquisidor-mendoza) · [Canonical Fireteams and Wildcards](../../../../sectorials/panoceania/military-orders.md#fireteams) · [MO Fireteams](../military-orders-fireteams.md) · [MO listbuilding](../military-orders-listbuilding.md) · [Kyle Hawkins analysis](kyle-hawkings.md) · [Hospitallers](hospitaller.md) · [De Fersen](de-fersen.md) · [Official N5.3 Weapon Chart](https://infinitythewiki.com/Weapon_Chart) · [Continuous Damage trait](https://infinitythewiki.com/Traits) · [Speculative Attack](../../../../rules/3_Combat/Speculative_Attack.md) · [Mimetism](../../../../rules/5b_Special%20Skills/Mimetism.md) · [Berserk](../../../../rules/5b_Special%20Skills/Berserk.md) · [Frenzy](../../../../rules/5b_Special%20Skills/Frenzy.md) · [Martial Arts](../../../../rules/5b_Special%20Skills/Martial_Arts.md) · [Number 2](../../../../rules/5b_Special%20Skills/Number_2.md) · [2026 Robert Shepherd MO review](https://www.youtube.com/watch?v=JrMTA91V7wc) · [2026 Ryan MO review](https://www.youtube.com/watch?v=xjs6rsspz8I) · [2026 Sneaky Snake MO review](https://www.youtube.com/watch?v=kRaambqovmw). **Reviewed 23 November 2026.** Ratings, targets and constructed Fireteams are qualitative judgments, not measured win rates.

## Exact pinned profiles and priority

**ID 1562 · AVA 1 · Regular HI · MOV 15–5 cm (6–2 in) · CC22 · BS14 · PH13 · WIP13 · ARM4 · BTS6 · W2 · S2.** All three options have **Martial Arts L2, Berserk (+3), Dodge (+3), Dodge (+2"), Frenzy, Mimetism (−6), Religious Troop, BS Attack (Continuous Damage), and CC Attack (Continuous Damage)**. Common weapons: **Grenades, Boarding Pistol, DA CC Weapon**. Neither the solo nor FTO profiles are Specialists, have Stealth/Combat Instinct, or have NCO/Tactical Awareness.

| Army option | Points / SWC | Exact distinguishing loadout | Role and rating |
|---:|---:|---|---|
| **4** | **40 / 0** | **MENDOZA FTO**: MULTI Rifle; **TinBot Firewall (−3), Number 2**; eligible Wildcard | **B+ overall; A− situational.** Durable linked close/mid-range gunfighter and hacking-defense provider |
| **2** | **40 / 0** | Heavy Shotgun; **Forward Deployment (+8"), Decoy (1)**; no TinBot, Number 2 or Fireteam eligibility | **B+; A− on dense tables.** Independent early short-range assassin with strong +6 weapon band |
| **3** | **45 / 0** | MULTI Rifle; **Forward Deployment (+8"), Decoy (1)**; no TinBot, Number 2 or Fireteam eligibility | **B / skip usually.** More reach than solo shotgun, but costs five more and overlaps several MO mid-range guns |

**Important pinned-source discrepancy — do not silently copy:** The pinned roster transcribes solo options 2 and 3 as **“Transmutation”**. Its cited underlying Army JSON actually lists **Decoy (1)** on both (skill ID 215), **not Transmutation**; FTO option 4 has neither. The source is [pinned Army-derived Mendoza JSON](https://raw.githubusercontent.com/massayoshi/infinity-army-backup/6b79f39a3abbf5cd3d837fb9dc65e411fc35244b/n5/military-orders/units/padre-inquisidor-mendoza.json). This file records the correction without changing the pinned roster.

**Weapon PS correction:** The pinned Army-derived weapon table and the N5.3 Weapon Chart list **DA CC Weapon PS8** for both Mendoza and Hawkins, not PS5/PS6. The weapons listed for these profiles contain **no PS override**. The Heavy Shotgun is **PS5** and Boarding Shotgun **PS6**; standard MULTI Rifle is **PS7** (AP/Shock B3, DA anti-materiel B1); Grenades are **PS7**; Boarding Pistol is **PS7**. In N5, **lower PS is more lethal**. Prior discussion assigning PS5 to Mendoza's DA CC Weapon should not be propagated.

## 1. His real role: elite short-range gunfighter, not another generic CC knight

**Mimetism (−6) is Mendoza's defining distinction.** In MO, Hawkins, Hospitallers, Teutonics, Santiago and many other attackers already have AP shotguns/rifles and strong melee. Mendoza instead makes **enemy BS Attacks requiring LoF −6** (and Discover harder), regardless of whether Mendoza is actively shooting. Unlike Hawkins's **BS Attack (−3)**, his Mimetism protects against shots while moving, standing on ARO, or Dodging. Partial Cover can add another −3 enemy BS until Frenzy changes its protection. **MSV, non-LoF attacks and Direct Templates are important counters.**

The complement is **BS Attack (Continuous Damage)**: successful attacks with his MULTI Rifle, Heavy Shotgun, Boarding Pistol and grenades can generate successive Saving Rolls after a failed one. Each failed Saving Roll inflicts a Wound/STR loss and repeats until a successful save or Dead State. **This improves damage conversion after winning an exchange, not the odds of winning the initial Face to Face roll.**

**Targets worth paying for:** elite non-MSV gunfighters, ARM-heavy two-Wound infantry, midfield defenders with favorable AROs, wounded TAGs, clustered troops reachable by grenades, and targets that need more than a single ordinary wound to remove. **Avoid assuming he is a universal TAG solution:** high-ARM targets still make Saving Rolls, he lacks a true long-range AP gun, and exposing a hackable 40pt HI to a TAG/repeater net is risky. Opponents with Immunity (ARM/Enhanced) can negate Continuous Damage and/or AP special effects.

**Targets that rarely justify him:** ordinary one-Wound line infantry or unarmored objectives. Hawkins BSG, Teutonics, Montesas, Bulleteers, etc. already clear them for much less.

## 2. Shooting by range: FTO versus Hawkins, correctly accounting for +6 shotguns

| Range | Mendoza FTO MULTI Rifle (40) | Hawkins BSG (+1B) (26) | Hawkins MMR (32) |
|---|---|---|---|
| **0–8"** | **+3**, B3, AP/Shock **PS7**, Continuous Damage | **+6**, B3, AP **PS6**, BS Attack (−3) | **−3**, B3, AP/Shock **PS7**, BS Attack (−3) |
| **8–16"** | **+3**, B3 | **0**, B3 | **+3**, B3 |
| **16–24"** | **−3**, B3 | **−3**, B3 | **+3**, B3 |
| **24–32"** | **−6** (up to 24"; no fire beyond) | Out of range | **+3**, B3 |

**Range boundary correction:** MULTI Rifle's effective maximum is **24"**. Its −6 band is **16–24"**, not 24–32"; the table's final row means **Mendoza is out of range there**. Hawkins MMR remains usable out to its actual longer maximum. The table emphasizes where each is strong; check [Weapon Chart](https://infinitythewiki.com/Weapon_Chart) for exact range cutoffs.

**0–8" comparison against a covered target, before other MODs:** Hawkins BSG BS14 +6 range −3 Cover = **17** on **B3**; Mendoza FTO BS14 +3 range −3 Cover = **14** on **B3**. Hawkins imposes **BS Attack (−3)** on an opposing Face to Face roll when shooting; Mendoza imposes **Mimetism (−6)** on enemy LoF-based shooting. Thus **Hawkins is more accurate at point blank and Mendoza is harder to hit**. Do not claim Mendoza universally wins this exchange without evaluating the opposing weapon/range/MSV/ARO.

**8–16" favors Mendoza FTO over Hawkins BSG** in range, passive protection and Continuous Damage. **16–24" favors Hawkins MMR**: same active B3, but much better range modifiers; MMR also has BS Attack (−3), Specialist Operative and a Pulzar. **Mendoza is not a replacement for MO's needed 16–32" long-range opener.**

**Solo Heavy Shotgun differs sharply from FTO:** at **0–8"**, BS14 +6 range −3 enemy Cover = **17** on **B2**, AP **PS5** with Continuous Damage. It gives up B3 but buys a much stronger base Saving Roll challenge and starts 8" forward.

## 3. CC and mobility: real threat, but Hawkins remains a great duelist

- **Mendoza:** CC22 +3 from MA2 = **CC25** before opposing MODs, and MA2 gives the opponent **−3**; his **DA CCW PS8 + CC Continuous Damage** starts with **two Saving Rolls per non-critical hit**, each with repeating Continuous Damage on failed rolls. His **Berserk (+3)** can move up to his total **8"** MOV and CC Attack as one Long Skill when requirements are met. Berserk does **not** automatically turn the ARO into an unopposed hit: valid enemy Dodge, BS or CC responses may produce a Face to Face roll. Mimetism does **not** apply to enemy CC Attacks.
- **Hawkins:** CC23 +3 from MA3 = **CC26** before opposing MODs, enemy **−3**, **MA3 grants +1 Success Die**; ordinary DA CCW **PS8** gives two saves but not Continuous Damage. Hawkins is typically the **more reliable technical duelist**; Mendoza has **greater high-end wound output** after a hit and extra reach through Berserk.
- **Dodge:** Mendoza's **PH13 +3 = 16**, with normal 2" Dodge movement increased by **+2" = 4"**. Hawkins has **Dodge (+1")** (3" movement) but no +3 PH bonus. Dodge can reposition Mendoza, bypass an undesirable shooting ARO, disengage or set up a subsequent engagement, but is not free movement without a valid Dodge opportunity.

**Why DA + Continuous Damage is significant:** Unlike ordinary DA's two saves, each failed save against Mendoza can initiate another save. Against a multi-Wound/STR target, one good CC hit can therefore cause substantial damage. However, the attack must first be delivered, it is **not AP**, and enemies with strong CC skills, templating or Immunity can be better handled by shooting or hacking.

## 4. Grenades, pistols, and other overlooked tools

**Grenades (PH13, PS7, Impact Template Circular, Continuous Damage) are situational but not pointless.** They permit **Speculative Attack** without LoF and can threaten targets hiding behind corners or clustered in a location. At **0–8"**, +3 grenade range −6 Speculative = **PH10**; at **8–16"**, −3 range −6 Speculative = **PH4**, before any unusual extra restrictions. Speculative Attack ignores target Mimetism/Cover shooting MODs but still requires a legal trajectory and costs a **Long Skill, B1**. Do not spend several Orders gambling with PH4 unless the reward is exceptional.

**Boarding Pistol:** provides **Hit Mode** and a **Direct Template Blast Mode** with Continuous Damage; the template is particularly useful when an opponent's high BS/Mimetism makes a conventional Face to Face contest unattractive. Consider opposing template trading and friendly Fireteam positioning.

**Frenzy applies to both Hawkins and Mendoza.** Once it triggers in the applicable States Phase, **Impetuous + Limited Cover** mean enemies no longer suffer the normal −3 BS MOD for Partial Cover against him, though the Partial Cover **+3 Saving Roll** benefit remains. Mendoza retains his Mimetism, but must not be treated as a permanent −9 cover/Mimetism bunker. An Impetuous activation may also break his Fireteam; do not count a free Impetuous Order as automatic Fireteam economy.

## 5. The 14-point Hawkins tax is the actual selection test

| Capability | **Hawkins BSG 26/0** | **Mendoza FTO 40/0** | Tactical verdict |
|---|---|---|---|
| Primary fire | BSG **B3 +6** at 0–8", AP PS6 | MULTI Rifle **B3 +3** at 0–16", AP/Shock PS7 or B1 DA | Hawkins wins point-blank accuracy; Mendoza covers 8–16" better and adds Continuous Damage |
| Opponent shooting MOD | **BS Attack (−3)** during his BS Attack FtF | **Mimetism (−6)** on qualifying LoF shooting and Discover | Mendoza has broader defensive protection; MSV can erase it |
| Damage after hit | Ordinary AP or DA CC | **BS and CC Continuous Damage** | Mendoza stronger against resilient targets, potentially multi-Wound/STR |
| Melee | **CC23, MA3 (+1SD), DA PS8** | CC22, MA2, **DA PS8 + Continuous Damage**, Berserk (+3) | Hawkins more reliable duel; Mendoza higher ceiling/longer CC approach |
| Survival | ARM3, BTS6, W2, Combat Instinct | **ARM4**, BTS6, W2, Mimetism (−6) | Mendoza stronger in most normal ranged matchups |
| Mobility/approach | **Stealth**, Dodge (+1") | **Dodge (+3), (+2")**, Berserk move | Different forms of mobility; Mendoza **lacks Stealth**, significant against Repeaters |
| Mission utility | **Specialist Operative** | **Not a Specialist** | Major Hawkins advantage |
| Fireteam status | Wildcard; **counts as Hospitaller** | Wildcard **FTO only**; **does not count as Hospitaller** | Hawkins increases Crusade FT level and can help achieve FT3+ |
| Support | Flash Pulse, Combat Instinct | **TinBot Firewall (−3), Number 2**, grenades | Mendoza earns points if the *same team* needs both Firewall and premium gun |
| Cost | **26** | **40** | **+14** for Mendoza: a substantial opportunity cost in 300pt MO |

**Hawkins MMR at 32pts is another serious alternative:** 8–24" +3 MULTI Marksman Rifle B3, BS Attack (−3), Specialist Operative, MA3, Stealth and Pulzar. Versus Mendoza FTO, its superior 16–24" band and **8-point savings** often outweigh Continuous Damage/TinBot unless a specific heavy target or hacking-defense need exists.

**Rule of selection:** **Hawkins BSG first** when you need an efficient close fighter who can press buttons and maximize Crusade equivalence. **Mendoza FTO** only if you need an unusually hard-to-shoot primary killer *and* his Firewall/Number 2 or special damage meaningfully pays for the 14–point premium. Do **not** take Mendoza merely as 'another melee knight' or another MULTI Rifle in an army full of medium-range weapons.

## 6. FTO Fireteams: legal partners, actual bonus levels, costs

**Mendoza is a Wildcard only on option 4.** His FTO tag does **not** satisfy a Fireteam family's native minimum (MO required-choice Crosier/Teutonic/Santiago FTO; Order Sergeants at least one actual FTO Order Sergeant; Crusade at least one actual FTO Hospitaller; Velox requires its specified native). Mendoza has **no Counts-as label**, so he never increases a Crusade/Hospitaller, Order Sergeant, or Crosier-equivalent Fireteam level just by being present. **FT2** is +1 Success Die (roll extra, discard one) on eligible BS Attacks, **not +1 Burst**; **FT3** adds +3 Discover/+1 Dodge, **FT4** +1 BS and **FT5** Sixth Sense, subject to actual count equivalence.

| Legal composition | Total pts / SWC | Type, level | Why / concern |
|---|---:|---|---|
| **Hospitaller FTO BSG 26 + De Fersen HD/MULTI Rifle 42 + Mendoza FTO 40** | **108 / 0.5** | **Crusade Haris, FT2** | Best premium thematic use: De Fersen's hacking + Mendoza's own TinBot/Number 2 + close fire. **Not FT3**; De Fersen and Hosp count as Hospitaller, Mendoza does not |
| **Teutonic NCO Spitfire 29/1.5 + Teutonic Specialist 19 + Mendoza FTO 40** | **88 / 1.5** | **Military Orders Haris, FT2** | NCO/LT-order engine, affordable specialist and premium short-range shooter; compare replacing Mendoza with Teutonic TinBot 19 (67 pts, FT3) |
| **Order Sergeant FTO Pitcher/Hacker 18/0.5 + Order Sergeant FTO HRL 15/1.5 + Mendoza FTO 40** | **73 / 2** | **Order Sergeants Haris, FT2** | Pitcher/forward hacking support, defensive HRL, Mendoza's short-range defense; higher cost and lower level than a same-family support trio |
| **Hospitaller FTO Doctor 30 + Mendoza FTO 40** | **70 / 0** | **Crusade Duo, FT1** | Durable recovery and Firewall but **no FT2**; compare **Doctor 30 + Hawkins BSG 26 = 56, FT2** |
| **Joan v2 LT 45/1 + Hospitaller FTO Doctor 30 + Mendoza FTO 40** | **115 / 1** | **Crusade Haris, FT2** | Expensive attacking team with Doctor/Firewall; Joan already has Number 2, and an efficient Hawkins substitution is often preferable |

**Do not double-pay Firewall:** two TinBots (-3) do **not** stack to -6 on the same protected target. If Mendoza is the Firewall carrier, consider **Hospitaller Doctor/BSG**, **De Fersen**, or another needed role rather than paying again for the Hospitaller TinBot or Santiago KHD/TinBot purely for identical Firewall coverage. **If you have no vulnerable Hacker traveling with him,** TinBot is still defensively useful to the other hackable team members but may not justify choosing Mendoza alone.

**Preferred practical companions:** **De Fersen** (protected Apex full HD and credible medium-range attacker), **actual Hospitaller Doctor** (recovery of expensive elite fighters; legal Crusade native), **Teutonic NCO Spitfire** (longer-range opener and Lieutenant-order conversion), **Order Sergeant Pitcher/Hacker** (delivery of the repeater/hacking game and a native link). **Joan/Hawkins** add offensive threat but often overlap Mendoza's role, increase cost and may cause unwanted FTO-level loss. **Knight of Justice** is a possible hacker/long-gun partner; its Number 2, if present on selected profile, makes that part of Mendoza's kit redundant.

## 7. Solo Forward Deployment (+8") and Decoy: is it worth it?

**Heavy Shotgun 40/0 is the more coherent independent attacker.** The +8" setup brings his +6 range, **AP PS5 B2 Continuous Damage** closer to targets from the opening turn; Decoy (1) makes early shooting decisions and deployment threat evaluation more awkward. It also gives an assault axis independent of the vulnerable main Knight Fireteam. **The downside:** 40 points invested in no Specialist, no Stealth, no TinBot or extra Order, on a model that must close to within 8" and remains Hackable. Decoy is **not** a Firewall or reliable substitute for Smoke/Repeater clearing. Dense tables and favorable missions are necessary.

**Solo MULTI Rifle 45/0 is less appealing**: +5 points gets the more flexible B3 rifle while retaining FD/Decoy, but that overlaps MO's many capable 0–16" attackers; if you want a MULTI Rifle Mendoza at all, the 40pt FTO normally provides better overall army value. Pick the solo rifle only for a plan that specifically combines **independent early positioning** with **8–16" B3 Continuous Damage** and does not need a legal Fireteam.

**Never assume the FTO starts forward or carries Decoy**; conversely the two FD/Decoy profiles **cannot join** Fireteams in this roster.

## 8. Evidence of use, not claims of pick-rate

- **[Observed]** Report **#020** reconstructs an **attacking Teutonic NCO Spitfire + Mendoza Duo**. [Battle reports #011–020](../../../battle-reports/011-020-n5-battle-report-tactical-analysis.md). Exact Mendoza option is not printed, but linked use requires FTO.
- **[Observed]** Report **#085** reconstructs **Crosier MSV2 HMG + Mendoza + Crosier Paramedic** as a deployed three-trooper shooting group. Fireteam type/level are not securely stated; Mendoza in the linked group is consistent with FTO. [#081–090](../../../battle-reports/081-090-n5-battle-report-tactical-analysis.md).
- **[Observed]** Another report names **solo Mendoza Heavy Shotgun** as a forward attacker; a custom four-player report also includes Mendoza, but its special conditions are not generalizable competitive evidence. [#121–130](../../../battle-reports/121-130-n5-battle-report-tactical-analysis.md) · [#131–140](../../../battle-reports/131-140-n5-battle-report-tactical-analysis.md).
- **[Player opinions, not measured rates]** [Robert Shepherd](https://www.youtube.com/watch?v=JrMTA91V7wc) calls him a fun but difficult-to-afford **luxury/vanity pick**; [Ryan's review](https://www.youtube.com/watch?v=xjs6rsspz8I) likes FTO as a **second-stage attacker + TinBot**, with the solo FD options more matchup-dependent; [Sneaky Snake](https://www.youtube.com/watch?v=kRaambqovmw) is especially positive about **FTO**, and recounts both a repeater-network failure and a devastating enemy-backline push in personal games.
- **Evidence limit:** these reports are selected MO appearances among many reports of other factions, **not a denominator of all MO lists or a profile-level usage sample**. They establish that **both linked and solo Mendoza are used**, not that FTO or FD has a verified tournament pick-rate.

## Final listbuilding decision

**Start with Hawkins BSG 26 in most balanced 300pt MO lists**, especially in a Crusade with a real Hospitaller anchor, De Fersen or Joan, where Hawkins's **Specialist Operative + Hospitaller equivalence** wins missions and improves FT levels. At **40 points**, Mendoza must do **two jobs simultaneously**: reliably remove awkward elite pieces in the 0–16" bracket *and* provide needed hacking protection/Fireteam robustness—or, as a solo FD HSG, open an independent lethal approach that the rest of the army cannot accomplish economically.

**Good Mendoza list:** sufficient other specialists, a real long-range opener, a route around Repeaters/MSV, no duplicate Firewall, and an important target that Continuous Damage can punish. **Bad Mendoza list:** too many expensive non-specialist short guns, no long-range opener, only one reliable scoring route, or another existing TinBot and a lack of Orders.

**Overall: not a must-take. FTO is the best all-around Mendoza; 40pt HSG FD8/Decoy is the most distinctive solo niche; 45pt solo MULTI Rifle is a luxury.**
