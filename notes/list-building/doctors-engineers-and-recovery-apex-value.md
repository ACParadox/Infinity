# Doctors, Engineers & Recovery Support — N5.3 Apex and Value Tiers

*2026-10-23 · 300-point context · cross-game comparative guide. **S/A/B are conditional editorial tiers**, not win-rate measurements. Checked against pinned [sectorial N5.3 profiles](../../sectorials/INDEX.md), [Doctor](../../rules/5b_Special%20Skills/Doctor.md), [Engineer](../../rules/5b_Special%20Skills/Engineer.md), [MediKit](../../rules/5c_Equipment/MediKit.md), [GizmoKit](../../rules/5c_Equipment/GizmoKit.md), [Peripheral](../../rules/5b_Special%20Skills/Peripheral.md), [Remote Presence](../../rules/5b_Special%20Skills/Remote_Presence.md) and [September 2026 FAQ](../../rules/5b_Special%20Skills/Peripheral_N5.3_Update.md). If a roster version disagrees, verify that exact Army profile.*

**Scope:** recover lost **VITA/STR** and cancel disabling states with *actual* Orders, reach, probability, and consequences. **Not** a list of general mission specialists or a command ranking. Compare Doctors, Engineers, and *complete packages* separately: their jobs are fundamentally different. For positioning and activation fundamentals see [Support Architecture](../Support%20Architecture%20-%20Doctor%20Engineer%20Servants%20and%20Recovery.md), [Peripherals](peripherals-synchronized-and-multi-body-troops.md), [TAGs](tags.md), [REM support](rems.md), and [Order efficiency](order-efficiency.md).

## Fast verdict: which support should I buy?

| Situation | First look | Why |
|---|---|---|
| **Best all-round support ceiling** | **Parvati36**, **Sophotect25**, **Med-Tech Obsidon21**, **Hakim24–29**, **Johnny Kao36** | High WIP, dual job / exceptional bonuses / deployment and movement; *which is best* depends on what needs recovery. |
| **Best Doctor success rate** | **Rouhani21, Hakim24–25, Avicenna28** (all WIP15+Doctor(+3) = 18); **Ghulam15** (WIP14+3 = 17) | 90% / 90% / 85% raw contact healing versus 65% on many WIP13 Doctors. |
| **Best 2-Wound medical return** | **Parvati36 Doctor(2W)**, **Claire Lazhari33 Doctor(2W) profile** | Valuable when an Unconscious elite VITA model needs to stand up with *two* Wounds removed in one roll. |
| **Best dual Doctor + Engineer value** | **Med-Tech21** (WIP14; 15-10 MOV), **Sophotect25** (WIP15; 15-10 MOV, NWI), **Kumotail21** (WIP14; Triad); **Parvati36** apex | One slot and support/Servant architecture cover *both* troop attributes. |
| **Best conventional Engineer value** | **Clockmaker18 WIP15**, **Lambda16 WIP14**, **Najjarun15 WIP14**, **Mech-Engineer14 WIP13**, **Dozer13 WIP13** | Need WIP and a safe Servant route, **not** a 30pt combatant, to revive a 70pt Remote Presence TAG. |
| **Best cheap engineering/trader** | **Irmandinho8 WIP13**, **Monstrucker12 WIP13 (Irregular)**, **Tokusetsu Engineer14** | Buy when smoke/trading/extra coverage is useful; **Irregular Order is not a free Regular Support Order**. |
| **Best recovery reach** | **Hakim parachutist incl. Nasmat A2**, **Tomcat22–26**, **Carlota28–32**, **NCA Blade Engineer** | Arrive at the endangered flank and recover where a DZ Servant would need 3+ Orders to travel. |
| **Best low-risk wide network** | **Controller + two 3pt Servants**; **Ariadnan Dozer + 2pt Remontnik** where rostered | Two protected recovery zones from one safe Controller, **one Servant activated at a time**. |
| **Best disabled-tech reset** | **Engineer in contact, high WIP; GizmoKit + Tech-Recovery for ranged access** | A successful Engineer removes **all** eligible Engineer-cancelable state tokens in **one** roll (N5.3), not one state per Order. |
| **Better to skip a Doctor** | Few recoverable VITA pieces, all disposable Dogged, deep enemy-DZ attacks, cheap Paramedic/Speedball suffices | Recovery is often a **conditional** action that never becomes reachable. Spend saved points on threats/scorers instead. |

**Apex** = greatest recovery capability once it can be brought to bear. **Value** = capabilities/actual reachable recoveries *relative to complete points, SWC, Regular/Irregular Orders, model survival and opportunity cost*. **S** unusually strong in its job, **A** strong, **B** conditional, **C** niche/overcosted for pure recovery. Each tier is *within its Doctor, Engineer, or dual-role group*, not a claim that Doctor outranks Engineer.

## 1) Recovery math — chance **and** Orders

**Exact unopposed d20 probability:** if the modified WIP/PH is N (and no other modifiers), the success rate is N/20. The following are **conditional on reaching legal contact, remaining eligible to recover and facing no ARO**. They are *not* actual whole-turn resurrection rates.

| Eligible roll | One attempt | One Command Token reroll **if eligible** | Example |
|---:|---:|---:|---|
| 12 | 60% | **84%** | PanO Machinist/Trauma-Doc **WIP12** |
| 13 | 65% | **87.75%** | ordinary WIP13 Doctor/Engineer |
| 14 | 70% | **91%** | Lambda/Najjarun/Med-Tech WIP14 |
| 15 | 75% | **93.75%** | Clockmaker/Sophotect/Parvati WIP15 |
| 17 | 85% | **97.75%** | Ghulam WIP14 + Doctor(+3) |
| 18 | 90% | **99%** | Rouhani/Hakim WIP15 + Doctor(+3); Parvati WIP15 + Engineer(+3) in applicable current roster |

**Formula:** with one *allowed* repeat of the failed same-target roll, \`P(success) = p + (1-p)*p\`. Built-in **Doctor/Engineer (ReRoll WIP=X)** instead uses \`p + (1-p)*q\`, where \`q=X/20\` and the second result replaces the first; subsequent Command Token reroll is separately possible **where the target qualifies** and the resource remains. These are not extra free Orders or universal rerolls. **Cubes** allow Command Token repeat of **Doctor**; **Remote Presence** allows it for **Engineer**. Both use the *actual qualifying target*, not every ally.

**Examples:**
- **Trauma-Doc12** on Cubed, reachable elite VITA: 60% normally, **84% with one Command Token**; **Ghulam(+3)17**: 85%, **97.75% with token**. On a **non-Cube** troop, that Doctor token reroll is unavailable.
- **Rouhani WIP18**: 90% on contact, **99% only if that patient has Cube and a token is spent**. **Doctor(2W)** improves Wounds restored, **not** success odds.
- **Engineer Clockmaker15** on Remote Presence TAG: 75% first roll; **93.75% with token**. A WIP12 Machinist: 60% / **84%**. Remote Presence also allows **one successful Engineer roll** to cancel either Unconscious level rather than require an extra revival roll.
- **Engineer(+3) WIP15 Parvati**: 90% first roll **where the exact +3 profile is legal**; do not automatically import this modifier to older/generalist source rows. Current pinned *Starmada* explicitly records (+3), but another O-12 reference summarizes (+1); treat that **source disagreement as requiring profile-level verification**, not a universally guaranteed 90%.
- **Contact MediKit:** **patient** rolls PH, not Doctor's WIP; **PH10 = 50%, PH11 = 55%, PH14 = 70%**. A failed MediKit PH kills Unconscious VITA patient.
- **Ranged MediKit:** first **hit with BS and actual Cover/range**, *then* patient PH. Example: BS12 shooter in 0–8in +3 band with no other MOD: 75% hit; PH11 recipient 55% succeeds; **41.25%** total for that *single* ranged application, with no relevant opposing ARO. The range-band/hit condition matters more than adding a second MediKit.
- **Contact GizmoKit:** target's printed GizmoKit-specific PH if applicable; **PH11 =55%** success, **failed PH inflicts a Wound** (could kill an already critical STR unit). Ranged GizmoKit also needs a **BS hit**. For Remote Presence, one successful GizmoKit PH can cancel either Unconscious level; **ordinary GizmoKit does not automatically clear IMM/Isolated**.
- **Repeated safe Engineer state clearing:** at WIP14 (70%) mean **1/0.70≈1.43 attempt Orders**; at WIP12 (60%) ≈**1.67**, *provided no enemy interrupts and each repeat is safe*. This arithmetic does **not** describe failed wound repair, which inflicts damage.

**Delivery changes everything.** If a 90% Doctor needs 4 travel Orders and then 1 healing Order, they bought a 90% attempt after 5 Orders. If a WIP13 Doctor with prepositioned Servant needs only one move + recovery (2 Orders), its cheaper, earlier contribution may be more valuable. Recovered troop must **still have Orders / line / mission relevance afterward**; an ARO troop standing into the same open lane often dies again.

### Recoverability thresholds — use before buying the doctor

| Casualty | **Useful recovery call** | Walk away instead |
|---|---|---|
| **70–120pt Remote Presence TAG** (Unconscious I or II) | Engineer/Servant ≤2 movement Orders, safe contact, token available; **single success stands it back up**, restoring threat. | TAG already **Dead**, enemy can kill Servant or immediately repeat ARO, or no Repair route. |
| **30–55pt Cubed HI / important ARO** | Doctor+3 or WIP15 with Servant behind corner; token can materially reduce terminal failure. | Lost to Shock/other no-Unconscious outcome, Dogged spent, patient not in reachable zone. |
| **15–30pt REM sniper / Repeater / Specialist** | Cheap Engineer + Servant next to protected ARO shelf; revive to reinstate Order tax or scoring. | A 4-Order detour to gain one cheap body near end of game. |
| **10–20pt LI** | Last available objective specialist or its return turns scoring decisively. | Pure 10–20pt cheerleader, no clear scoring job, requires 3+ Orders. |
| **Tech-Recovery VH (Redeye/Firebat/etc.)** | **Ranged** GizmoKit or Engineer route and one-hit Tech-Recovery state reset when the aircraft is disabled. | Airborne **No Cover** and enemy AROs prevent a safe delivery; contact is not assumed. |
| **NWI / Dogged** | Heal **recoverable NWI** before final decisive turn if actual Doctor access. | After **Dogged activated**, normal Doctor recovery is unavailable; don't pay for ambulance as if it were. |

## 2) Doctors — apex / points-value tiers

| Doctor / **exact profile** | Apex | Value | **What it beats, when and why** | Limitation / dissent |
|---|:---:|:---:|---|---|
| **Rouhani21/0**, WIP15, **Doctor(+3)** — Ramah/eligible Haqq | **S** | **S** | **90% contact**; NWI keeps the healer available, wildcard delivery into an already useful Fireteam; premium Cubed HI and objective specialists. | Less reach than Hakim and one Wound; when the roster has few salvageable VITA elites, **15pt Ghulam** can do enough. |
| **Hakim24–25/0**, WIP15 **Doctor(+3)**, Parachutist; **29/25 incl. Nasmat A2** — Ramah | **S** | **S/A+** | **90%** and can enter from the necessary board edge; **Parachutist Nasmat A2** lets recovery reach behind the main assault route. Boarding Shotgun(+1B) or SMG/E/Mitter does credible secondary work. | Does **not** automatically teleport into safe contact; entry timing, model survival, legal Servant placement and Irregular/Regular group Orders matter. More expensive than ordinary DZ Doctor. |
| **Avicenna28/0**, WIP15, **Doctor(+3)** — StarCo/Bakunin | **S** | **A+** | **90%** contact revival, **MOV15-5, NWI, Immunity(ARM)** and **Riot Grrl Fireteam** where legal; a durable forward doctor for expensive VITA assault models. | At **28pts**, expensive compared with Daktari14 or cheaper ordinary Doctors; no Engineer function, and reaching a dying TAG/REM never helps. |
| **Parvati36/0**, WIP15, **Doctor(2W)** — O-12/Starmada/ALEPH eligible | **S** | **A** | **Two Wounds restored** on Unconscious multi-Wound VITA; MOV15-5, Super-Jump, **STR2+Remote Presence**, and Engineer job in same durable model. Extraordinary dual-role **ceiling**. | 75% base *Doctor* roll, not 90%; heavy cost wasted if only one-Wound troops or a cheap Nurse is sufficient. Current pinned engineer bonus varies across source rows; verify exact roster. |
| **Dr. Claire Lazhari33/0 Doctor(2W)** or **FTO Doctor(+3)** — eligible ALEPH/OSS/Ramah/QK | **S/A+** | **B/A** | Choose **2W return** into multi-W VITA or **WIP14+3 =17** success into single-W patient; 15-5, NWI, Immunity, useful close guns and MediKit PH17 support. | Two advantages are **different mutually exclusive profiles**; **FTO** eligibility varies; 33pt commitment can be excessive for limited VITA targets. |
| **Sophotect25/0**, WIP15, MOV15-10, NWI — ALEPH/OSS | **A+** | **S** | **75%** Doctor contact plus high-WIP Engineer and rapid movement; ideal mixed VITA HI + REM/TAG list. Supports Yudbot zones where roster permits. | No Doctor(+3), prone/exposure/Fireteam constraints still matter; the **Engineer reroll** does not automatically reroll Doctor. |
| **Med-Tech Obsidon21/0**, WIP14, MOV15-10 — Combined/Shas/Onyx/Next Wave eligible | **A+** | **S** | **70%** medical plus Engineer in one 21pt fast, single-slot profile; two Slave Drones make a very broad doctor/technical web. | Doctor fail **kills**. Its tall S3 Controller can be harder to hide; don't substitute a 70% roll for Rouhani's 90% where both exist. |
| **Kumotail21/0**, WIP14 Doctor+Engineer, legal Triad — Tohaa | **A** | **S/A+** | One Triad-capable support piece moves with attack/scorers, plus **Chaksa Servant3** gives a remote recovery route for detached pieces. | 70% Doctor and no extraordinary intrinsic reroll; Fireteam cannot operate normally with deployed active Servants. |
| **Ghulam Doctor(+3)15/0**, WIP14 — Ramah/eligible Haqq | **A+** | **S** | **85%** base for merely +4 vs 11pt rifle Ghulam; legal Fireteam often delivers medical contact and an Order while buying an objective specialist. | Fragile, WIP17 rather than 18; if no relevant VITA patient nearby you bought a 15pt Order body. |
| **Bipandra23/0 or TacAware25/0**, WIP13, MediKit(+1B) — Kestrel/PanO | **A** | **B/A** | Fireteam wildcard who can travel with a gun, non-trivial BS weapons, optional personal Order; MediKit(+1B) at range improves chance **at least one hit**, not patient's PH. | **65% contact Doctor roll**; source roster does **not** show intrinsic Doctor(ReRoll). Kestrel podcast hosts strongly split on spending 25 when a cheap Fennec Paramedic / Speedball could meet scenario needs. |
| **112 Emergency Service11/0**, WIP13; **motorized19/0** — TAK/eligible Ariadna | **A (bike for reach)** | **S cheap / A bike** | **65%** plus **11pt** ordinary Doctor value; motorbike **20-10 + Smoke** catches mobile casualties without prepositioned bots. | Ordinary WIP13 and bikes can be exposed/limited Cover; **No-Cube Ariadnans** commonly lack Doctor token reroll. |
| **Tokusetsu Doctor14/0** / **Zhanshi Yīshēng14/0** / **Daktari14/0** — JSA/Yu Jing/Nomads | **B/A** | **A+** | Reliable *availability and cheap specialist Order* at WIP13; add the appropriate **3pt Servant** and avoid moving the Doctor into a firing lane. | 65% gamble can still kill critical patient; if you mostly run STR machines, buy Engineer first. |
| **Kazak Doktor12/0**, WIP13 — TAK/Kosmoflot | **B/A** | **S/A** | Cheap team-compatible recovery for 2W/medium infantry while keeping 300pt budget intact. | **65% with no Cube token on most Ariadnans** means irreplaceable target can die to heal attempt. |

### Doctor priority: success, *amount* or delivery?
1. **Need to revive a 2–3W VITA attacker?** Parvati/Claire **Doctor(2W)** may make one action save two Wounds. If merely one removed Wound matters, Rouhani/Hakim **Doctor(+3)** provides higher base success.
2. **Need to reach a casualty behind enemy midfield?** Hakim parachute/Servant A2 and Tomcat rescue may beat WIP18 that starts stuck in home DZ.
3. **Few Cubes and no 2W premium VITA?** A cheap Regular Doctor at 11–15, Paramedic, or **Speedball VitaPack** often dominates support spending.
4. **Doctor inside Fireteam:** it advances naturally **if legal**; deploying Servo bots can conflict with Fireteam membership. Do **not** assume both benefits coexist.

## 3) Engineers — apex / points-value tiers

| Engineer / **exact profile** | Apex | Value | **When better and why** | Limitation |
|---|:---:|:---:|---|---|
| **Parvati36**, WIP15 Engineer bonus (Starmada +3) | **S** | **B/A** | Highest roll reliability, **STR2 Remote Presence**, 15-5 Super-Jump, Doctor(2W); best when valuable VITA **and** a TAG/REM and scoring need the same mobile body. | 36pts for a 1–2 Order repair is overkill; verify +3 vs +1 O-12 pinned profile inconsistency. |
| **Johnny Kao36/0**, WIP14, **Engineer(ReRoll)**, GizmoKit(+1B), Mimetism−3, 2W — eligible ALEPH/Yu Jing | **S** | **A/B** | **Repeat of failed Engineer** reduces catastrophic repair failure; 15-5, durable, useful plasma/zapper and nonhackable anti-tech shooter. Best for hostile midfield STR recovery, not static DZ machine tending. | **ReRoll's printed WIP=X matters**; not a free certainty. 36pt combat engineer can die or get dragged into attacking instead of protecting TAG. |
| **Sophotect25/0**, WIP15 **Engineer(ReRoll WIP=X)** + Doctor — ALEPH/OSS | **S** | **S** | Fast MOV15-10, NWI, both patient types, accurate + possibly repeatable Engineer. Excellent **primary recovery hub** for expensive mixed list. | Built-in Engineer reroll not the same as Doctor reroll; Controller remains fragile to concentrated attacks. |
| **Clockmaker18/0**, WIP15 — Nomads/Corregidor/Tunguska eligible | **A+** | **S** | **75% Engineer**, up to 93.75% **with token on Remote Presence**; 18pts + one/two Zondbots can resurrect 30–70pt REM/TAG from either Unconscious level. | 1W rear model; if no recoverable STR or severe state threats, many points go unused. |
| **Chung-Hee Jeong31/0**, WIP14 Engineer(ReRoll) — IA/White Banner | **A+** | **A/B** | ReRoll, Repeater and long-term defensive toolbox with attack/deployable turret when the team uses all of it. | 31pts > normal Mech-Engineer14; only worth if cover/Repeater/link and recovery **all** matter. |
| **Krit Kokram37/0**, WIP14, 2W, MOV15-5 — IA/eligible YJ | **A+** | **B/A** | Tough HI engineer **inside a lawful HI team**, with useful shotgun/E/M; forward Engineer rescues TAG/STR nearer enemy. | Too expensive just to stand hidden behind a TAG; no free Servant inside Fireteam. |
| **Med-Tech Obsidon21/0**, WIP14, dual skill, MOV15-10 — Combined | **A+** | **S** | Combines 70% Engineer with 70% Doctor, fast enough to shift zones, compatible Slave Drones when taken outside teams. | S3 Controller harder to keep safe. |
| **Lambda16/0**, WIP14 — O-12/Starmada/Torchlight | **A** | **S** | **70%** recovery, inexpensive, readily adds Yudbot3; superior to costly multifunction model when only STR maintenance + scoring is required. | 1W/slow 10-10; pay attention to Fireteam legality if adding Yudbots. |
| **Najjarun15/0**, WIP14 — Haqq/Ramah | **A** | **S** | **70%**, cheap Regular Order and **Nasmat3** coverage for Maghariba/Shakush/REM while Doctors handle VITA; better pure TAG mechanic than Hakim. | Does not heal ordinary VITA. |
| **Kumotail21/0**, WIP14 dual role — Tohaa | **A** | **S/A+** | Covers mixed Tohaa VITA and STR, allows **Chaksa3** flank services when not in Triad. | Not maximum single-purpose Engineer odds; Triad/Servant tension. |
| **NCA Blade Engineer** (verify FTO/Parachutist) — Neoterra | **A (reach)** | **A+ when deployed right** | **Parachutist + Decoy** and current 2026 tactical interviews place an Engineer at a forward Redeye/REM casualty much faster than a rear Machinist; GizmoKit can help Tech-Recovery at a distance. | Deployment requirements/specific profile affect legality; no safe landing lane means wasted points. |
| **Tomcat Engineer22/0 (26 incl. Zondcat)**; **Carlota28/0 (32 incl. Moriarty)** — Corregidor | **S (reach)** | **A+** | **Parachutist/Climbing Plus** moves recovery near far-flank STR model; Zondcat option adds local reach. Carlota WIP14 vs basic Tomcat WIP13 and better close attack. | Pay extra only if casualty will be beyond rear Zondbot. Dropping after an exposed attacker already dies may be too late. |
| **Evader24/0 (BSG) / 29/0 (MULTI Rifle) / 35/1.5 (AP Spitfire)** — Corregidor | **A** | **A/B** | 2W-equivalent **NWI + Climbing Plus + TinBot/support** makes Engineer survivable inside legal combat-team assault; repair while moving forward. | Expensive *if used solely for repair*. Toolbox video praises strong dual roles, warns 25pt Wildcat Engineer may pay for unused gun/skill package. |
| **Mech-Engineer14/0**, WIP13 — Yu Jing/IA/White Banner | **B/A** | **S/A+** | **65%** but **87.75% with token on Remote Presence**; Yáozăo3 recovery zone, affordable alongside heavy TAG. | Slower and lower success than 18pt Clockmaker; can fail damaging WIP roll. |
| **Dozer13/0**, WIP13 + **Remontnik2** — Ariadna/TAK/Kosmoflot | **B/A** | **S** | **15pt** complete one-Servant package, cheap long-angle support even in mostly organic Ariadna; useful for Chernobog/REM and engineering states. | Support is less valuable if list barely includes STR and no debuff repair route. |
| **Irmandinho8/0**, WIP13, Impetuous/Irregular Engineer — Ariadna/TAK/Kosmoflot | **A (tempo/trading)** | **S contextual** | **8pts**, Smoke, Chain Rifle/E/M utility and Engineer: can trade or turn into a forward E/M-state fix **without buying a passive model**. | **Irregular** Order can't freely fuel other troopers; Impetuous No Cover exposure and low safe transport value make it a **bad replacement for dedicated rear TAG repair**. |
| **Monstrucker12/0 SMG**, WIP13, Irregular + Climbing Plus — Ramah/O-12/etc. | **B/A** | **S if needed** | Very cheap Engineer and climbing close support; useful on sparse STR list where a 25–36pt support hero is unjustified. | **Irregular**, fragile, no premium Doctor; must budget Regular recovery Orders separately if necessary. |
| **Tokusetsu Engineer14/0 / Yuriko Oda25/0 / Genbutai Engineer23/0** — JSA | **B/A** | **A+/A** | **Tokusetsu** cost-effective Yáozăo3 TAG/REM recovery; **Yuriko** brings mines/Mimetism to defend objective route; **Genbutai** adds Fireteam durability/utility. | More expensive Engineer only if its second job is actually used; O-Yoroi often needs hidden cheap recovery rather than forward fighter. |
| **Kosuil Engineer20–25/0** — Tohaa | **A (fireteam)** | **A** | K1/shotgun frontline assault Pioneer **can remain within Triad** and repair when attack team reaches danger area. | Not equivalent to cheap protected Kumotail+Chaksa network. |

**Engineer priority:** buy the **cheapest safe access to WIP14–15** plus a Servant for a vulnerable big Remote Presence piece; pay for fighter-Engineer, parachutist, ReRoll or dual skill *only when the battlefield forces you to use that second feature*. Clearing disabling states is often more valuable than restoring STR.

## 4) Recovery **packages** — apex versus whole-list value

| Package | Apex | Value | **Exact circumstance** |
|---|:---:|:---:|---|
| **High-WIP dual-role Controller + two Servants in two safe zones** (Sophotect25+Yudbots6, Med-Tech21+Slave6, Kumotail21+Chaksa6) | **S** | **S** | 27–31pt **actual network**, covers flank ARO + TAG/midfield; earns Orders if targets remain inside recovery radius. **One Servant at a time**, Controller shares group. |
| **WIP15 Engineer18 + Zondbot3 near TAG/REM** | **A+** | **S** | 21pt package, Remote Presence token reroll; opponent must kill damaged TAG or let it return. |
| **WIP14 Engineer15–16 + Servant3** | **A** | **S** | 18–19pt TAG/REM insurance with solid 70% first-roll; 91% token-assisted on Remote Presence. |
| **WIP13 Dozer13 + Remontnik2** | **B/A** | **S** | 15pt support cover in Ariadna. Best when serves both fragile gun REM and Chernobog/STR job. |
| **Rouhani21 or Ghulam15 near 2W Cubed HI team** | **S (reliability)** | **S/A** | 90%/85% Doctor success and potential Cube token; spending recovery Orders brings a key Wound/scorer back. |
| **Parvati36 with mixed elite VITA + STR** | **S** | **A+ here** | 2W Doctor + high-success Engineer, 15-5 and Super-Jump; one model can solve two expensive recovery problems. |
| **AD Hakim24–29 or Tomcat22–26** | **S (reach)** | **A situational** | Casualty **far from Servant net** but near safe flank entry. High entry/position value, risk of arriving after target eliminated. |
| **MediKit-only cheap Paramedic** | **B** | **S if otherwise no Doctor** | Has scoring Specialist job already; accepted 50–70% PH risk, or last-turn emergency at range. |
| **Request Speedball VitaPack / AutoRepairS / Switch On** | **A situational** | **Potentially S if infrastructure not worth buying** | **Two tokens**, Combat Jump **PH14 (70%) each**, one chosen item + other rolled; bearer must safely collect from token, then contact patient and spend Short Skill. **VitaPack/AutoRepairS apply without a Doctor/Engineer roll**, but only if drop/collection/contact succeeded; **not a free guaranteed revive**. [Current rules](../../rules/5a_Common%20Skills/Request_Speedball.md). |
| **GizmoKit + Tech-Recovery aerial/VH** | **A+ (state reset)** | **A situational** | Single *successful hit and resulting eligible PH outcome* helps clear multiple states at a distance. Important for **Redeye/Firebat** where contact with active aerial base may not be practical. |

**Important:** An Engineer can cancel **all** Engineer-removable disabling states simultaneously on a **single successful WIP roll** under N5.3. Tech-Recovery's niche is **remote GizmoKit interaction**, not turning several compulsory Engineer contact Orders into one. Earlier project Tech-Recovery commentary implying one state at a time is **obsolete**.

## 5) Servant positioning and true Order efficiency

- **Standard Servant 3pt**: **Palbot, Zondbot, Nasmat, Yudbot, Yáozăo, Slave Drone, Chaksa** as rostered. **Ariadna Remontnikbot 2pt** where rostered. Common movement **15-10**, tiny S1, Mimetism−3; no independent Order.
- **A Doctor/Engineer Controller may take at most two Servants** and activate only **one** at a time; Servant is not a new unit/Order, and **the Controller's WIP performs the skill roll**.
- Put **Servant A one protected Move away from expensive ARO shelf; Servant B one protected Move away from a TAG's likely fallback angle.** Do **not** leave both beside Controller, beside each other, or within a single template/repeater kill zone.
- **Turn 1** preposition while the expensive shooter moves in an orderly route; then use a second combat group's spare Orders for rescue where available. Two Servants in one combat group **do not** provide two support activations simultaneously.
- Do **not** assume Servant and Controller in legal Fireteam: [Peripheral](../../rules/5b_Special%20Skills/Peripheral.md) normally prevents Controller with deployed Peripherals participating in a Fireteam; **N5.3 Ancillary/Cyberplug exceptions and integrity changes** need exact application.
- **Doctor/Engineer and MediKit/GizmoKit are different rolls and functions.** Controller with Servant uses Controller's WIP Doctor/Engineer; **firing** a MediKit/GizmoKit requires a BS hit **followed by patient PH**. Multiple Medic/Gizmo successful hits in same Order can improve odds of at least one PH success, **not** multiple restored Wounds.
- **Tech-Recovery versus Unconscious:** Tech-Recovery state-clear **does not itself revive Unconscious**; a legal Engineer or successful GizmoKit on STR can revive first. If stunned/isolated/immobilized but *not Unconscious*, prioritize one safe Engineer state-clear.
- **Target evaluation:** Enemy may **finish off** an Unconscious model, forcing extra enemy Orders; **that alone can pay for some support investment**, but never automatically count an unattainable future resurrection.
- **After revival:** If target stands in enemy sight lines, plan suppress/Prone/safe reposition where legal; REMs/TAGs generally cannot Prone. Avoid increasing enemy ARO kill opportunities just to claim a recovered point value.

## 6) Contradictions, unpopular choices, and transcript-checked sources

Three real disputes:
1. **Expensive Doctor versus cheap Paramedic / Speedball.** [Irregular Order #52 Kestrel](https://open.spotify.com/episode/4RNxiaI1k5xXBVzVHxwnB9), approx **73–77m**: hosts explicitly disagree about spending **23–25pt on Bipandra** (the transcript mangles her name) versus a **Fennec Paramedic and Speedball**; one values tactical activation, Close support and reliability, another says few patients remain accessible enough to justify the 25pt. **Rule correction:** pinned Bipandra lists **Doctor, WIP13, MediKit(+1B)** but **not** Doctor(ReRoll), despite an apparent spoken claim to that effect. Judge the legal 23/25pt profile, not the speech transcription.
2. **Toolbox Engineer versus cheap support.** [Infinity the Dante — Toolbox Units Guide N5](https://www.youtube.com/watch?v=Q5kyCDufa8c) directly compares **Evader Engineer AP Spitfire / TinBot** as useful multi-role compression with **Wildcat Engineer25**, whose competing gunfighting/repair costs may pull in opposite directions. This is a **role/cost argument**, not a claim that WIP13 is bad.
3. **On-table Engineer placement: long-term backline or surprise flank?** [WIP12 E201 — NCA with Trent](https://open.spotify.com/episode/3FT1No7zFHzpj7WC63hcCb), approx **75–95m** describes a **Blade Parachutist Engineer** and accompanying **Palbot**, forward **Redeye Tech-Recovery** and Squalos/REM recovery; they stress short-path retrieval and specialist/attack utility. Counterpoint: Parachutist must actually *enter legally and safely*; a pre-positioned 3pt Servant may be more dependable.
4. **TAG repair investment versus tank doing work alone.** [Loss of Lieutenant #142 — N5 TAG tier discussion](https://open.spotify.com/episode/1h5CJfZC5zBPxdg66o7xIN) discusses Engineer WIP12 risk, the importance of Remote Presence and rerolls, tradeoffs with cheaper TAGs, and Speedball repairs (2025 episode: use latest N5.3 wording).
5. **Role overlap / Specialist slots.** [Corner Case — How To Build Your First Army List](https://www.youtube.com/watch?v=6elZA4pa_Po) notes that an Engineer is not just a repair roll but can score Classifieds/mission tasks; it often matters *which* mission tools the list already has.
6. **Very different use case:** [Robert Shepherd — Military Orders Faction Focus](https://www.youtube.com/watch?v=JrMTA91V7wc) reviews a cheap **Infirmarer of St Lazarus** joining support teams and a **Hospitaler Doctor** accompanying armored Knights. A linked Doctor may save 2–3 movement Orders that a theoretically higher-WIP backliner couldn't use at all.

**Not all videos above focus exclusively on medical recovery;** no authoritative general-purpose "all Doctors tier" transcript was found through the YouTube/podcast searches. Findings quoted here correspond to **MCP transcripts actually inspected**, with approximate times where available. Older shows discuss potentially outdated profiles; the repository's September 2026 unit data is authority. More specialized army podcast commentary remains linked in each sectorial file.

### Explicit disagreements with older project commentary

- [Support Architecture](../Support%20Architecture%20-%20Doctor%20Engineer%20Servants%20and%20Recovery.md) correctly emphasizes **Servant reach and Order availability**, but does **not** supply probabilities; the chance table above adds that second axis.
- The [Doctor skill](../../rules/5b_Special%20Skills/Doctor.md) unofficial commentary elsewhere claims Paramedics can use **WIP/PH−3**; **authoritative MediKit wording** instead requires BS hit at range then **patient PH** (or patient PH in contact) unless exact profile substitutes PH. Do **not** carry the obsolete shorthand into list math.
- The [Tech-Recovery skill](../../rules/5b_Special%20Skills/Tech-Recovery.md) unofficial explanation asserts normal Engineers clear one state at a time; **actual Engineer rule says all eligible states in one successful WIP roll**. Tech-Recovery still enables GizmoKit remote state reset.
- One pinned **Parvati** roster records Engineer (+3) while another summarizes (+1). **Do not silently resolve that conflicting roster data by assuming identical loadouts.** Confirm the exact selected army profile before quoting 90% in game.
- N5.2+ **ReRoll WIP=X** specifies the reroll threshold explicitly; old videos and historical **ReRoll−3** shorthand may not be exact after updates. No "free built-in token" can be assumed.

## 7) Sectorial quick-reference: what changes when choosing a healer

**PanO/Kestrel/NCA/MO/Varuna/WinterFor/Acontecimento:** 14pt **Trauma-Doc WIP12** with **Palbot3** is cheap but failure risk is real (60%; 84% Cube+token); **Machinist WIP12** similarly wants Remote Presence token support. **Bipandra23–25** helps in linked Kestrel, but not a universal upgrade. NCA **Blade Parachutist Engineer** recovers Redeye on far flank, where a DZ Machinist cannot. Hospitaler Doctor is better inside a moving MO Knight team; **don't assume Servant-equipped Controller remains linked**.

**ALEPH/OSS/Steel:** **Sophotect25 + Yudbot(s)** is among best whole-list returns on a 300pt mixed army; **Parvati36** is better where 2W Doctor or mobile high-end Engineer is actually needed; **Posthuman Mk.1 Engineer** creates extra slot/mission economy **only inside a legal 2–3 Proxy package**. Do not count a Mk.1 as independently fieldable cheap Engineer.

**Nomads/Tunguska/Corregidor/Bakunin:** **Clockmaker18 + Zondbot3** often beats a 30pt toolbox repairer for pure REM/TAG infrastructure. **Evader** or **Orphan Engineer** works when it is also gun/Repeater/link utility. **Tomcat22/26 + Carlota28/32** bypass a far-flank movement tax; **Wildcat Engineer25** is controversial toolbox spending when its team doesn't use MSV or gear.

**Combined/Shas/Onyx/Next Wave/Morat:** **Med-Tech21 + 3pt Slave Drones** is standout cheap dual hub, but tall S3 deserves concealment; **Gearhead Cyberplug** can project engineering differently and **cannot** also take Servants. **Kurgat** buys combat-ready Morat engineer; cheap regular alternatives should be measured against actual need to repair TAG/REM versus spending more on weapons.

**Haqq/Ramah/Hassassin/QK/Dahshat:** **Ghulam Doctor15(+3)** and **Rouhani21(+3)** deliver 85–90% with exact legal roster. **Hakim** wins where Parachutist/Nasmat A2 makes recovery physically possible; **Najjarun15** repairs STR; **Monstrucker12** sacrifices Regular Order for a cheaper technical specialist. **Claire** 33pt different **2W versus +3 FTO** profiles are situational, not interchangeable.

**Yu Jing/White Banner/IA/IS:** **Mech-Engineer14 + Yáozăo3** is efficient normal recovery; **Krit Kokram37** moves with HI gun team, **Chung-Hee Jeong31** buys ReRoll/Repeater specialist protection, **Johnny Kao36** more durable frontline anti-tech. Every expensive Guijia/Blue Wolf TAG benefits from deliberate fallback and remote repair position.

**Ariadna/TAK/Kosmoflot/USAriadna/Caledonia/FRRM:** **Irmandinho8** is an extraordinary cheap smoke/trading/engineering combination but not your only safe TAG mechanic; **Dozer13 + 2pt Remontnik** builds covered STR recovery cheaply. **112 Doctor11**, **Motorized112 19** and **Kazak Doktor12** are inexpensive medical choices, but **no-Cube** patients lose Doctor token re-roll security.

**O-12/Starmada/Torchlight:** **Lambda Engineer16 / Doctor variant** plus **Yudbot3** is enough for most Wrecker/Zeta/REM situations; **Parvati36** does something distinct with **2W Doctor, high Engineer, mobility, STR2**. **Kludger23**, **Vidocq FTO Doctor19**, **Delta forward support** win by arriving with legal team/route rather than by maximum backline WIP. For aerial **Firebat**, use ranged GizmoKit/Tech-Recovery when contact cannot be reached safely.

**Tohaa/JSA/Oban/Shindenbutai:** **Kumotail21** dual role with Chaksa3 supports mixed Tohaa attack Triads; **Kosuil20–25** trades cheap backline Doctor/Engineer economy for a K1 assault Engineer actually in the midfield. **Tokusetsu14**, **Yáozăo3**, **Yuriko25** form JSA's economical recovery plan for **Karakuri Remote Presence / O-Yoroi**; do not spend extra on forward engineer if patient remains near DZ.

### Final list-building test

1. **Recoverable patient:** Which VITA or STR units can actually enter eligible states rather than Dead/Dogged?
2. **Real chance:** What is **contact WIP**, and is a Cube/Remote Presence token reroll legal? If ranged, what are **BS hit × patient PH** and ARO hazards?
3. **Actual distance:** Where does the patient likely fall, and how many safe **Orders to contact, roll, and redeploy**? Are Servants prepositioned?
4. **Second job:** If no one needs recovery, does support still supply **Regular Order, scoring, Mine/Repeater, smoke, gun or Hacker protection**?
5. **Opportunity cost:** Is 6+ extra support points better than a second attacker, additional Specialist or protecting attack's retreat lane?

**Bottom line:** **Choose *reachability* first, *roll reliability* second, and *points cost* third** for a specific casualty. Then check whether not taking a healer at all scores more.
