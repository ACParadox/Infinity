# Doctors, Engineers & Recovery Support — N5.3 Apex and Value Tiers

*Updated 2026-11-05 · 300-point context · cross-game comparative guide. **S/A/B are conditional editorial tiers**, not win-rate measurements. Checked against pinned [sectorial N5.3 profiles](../../sectorials), [Doctor](../../rules/5b_Special%20Skills/Doctor.md), [Engineer](../../rules/5b_Special%20Skills/Engineer.md), [MediKit](../../rules/5c_Equipment/MediKit.md), [GizmoKit](../../rules/5c_Equipment/GizmoKit.md), [Peripheral](../../rules/5b_Special%20Skills/Peripheral.md), [Remote Presence](../../rules/5b_Special%20Skills/Remote_Presence.md) and [September 2026 FAQ](../../rules/5b_Special%20Skills/Peripheral_N5.3_Update.md). If a roster version disagrees, verify that exact Army profile.*

**Scope:** recover lost **VITA/STR** and cancel disabling states with *actual* Orders, reach, probability, and consequences. **Not** a list of general mission specialists or a command ranking. Compare Doctors and Engineers separately: their recovery jobs and deployment costs differ. For positioning and activation fundamentals see [Support Architecture](../Strategy/support-architecture-doctor-engineer-servants-and-recovery.md), [Peripherals](../Strategy/peripherals-synchronized-and-multi-body-troops.md), [TAGs](tags.md), [REM support](rems.md), and [Order efficiency](../Strategy/order-efficiency.md).

## Fast verdict: which support should I buy?

| Situation | First look | Why |
|---|---|---|
| **Best all-round support ceiling** | **Parvati36**, **Sophotect25**, **Med-Tech Obsidon21**, **Hakim24–29**, **Johnny Kao36** | High WIP, dual job / exceptional bonuses / deployment and movement; *which is best* depends on what needs recovery. |
| **Best Doctor success rate** | **Rouhani21, Hakim24–25, Avicenna28** (WIP15+Doctor(+3) = 18); **Ghulam15** (WIP14+3 = 17) | **90%** for each of the first three, **85%** for Ghulam, versus 65% on many WIP13 Doctors. |
| **Best frontline combat Doctor** | **Asawira Doctor35–37 — Hassassin; Machaon37/0.5 — Steel Phalanx** | Asawira brings Doctor(+3), 2W and gun/team pressure; Machaon brings WIP15, NWI, Mimetism(-6), normal Smoke and Myrmidon Core membership. Both need to **fight/score as well as heal** to justify their cost. |
| **Best 2-Wound medical return** | **Parvati36 Doctor(2W)**, **Claire Lazhari33 Doctor(2W) profile**, **Mother Agatha31 Doctor(2W)** | Valuable when an Unconscious elite VITA model needs to stand up with *two* Wounds removed in one roll. |
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

**Formula:**

- with one *allowed* repeat of the failed same-target roll, \`P(success) = p + (1-p)*p\`.
- Built-in **Doctor/Engineer (ReRoll WIP=X)** instead uses \`p + (1-p)*q\`, where \`q=X/20\` and the second result replaces the first; subsequent Command Token reroll is separately possible **where the target qualifies** and the resource remains.
- These are not extra free Orders or universal rerolls.
- **Cubes** allow Command Token repeat of **Doctor**
- **Remote Presence** allows it for **Engineer**.

Both use the *actual qualifying target*, not every ally.

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

**Ranking basis:** the number orders *overall practical recovery ceiling* in a 300-point list (reliability, reachable casualty, useful second job, survivability, Fireteam legality), **not** cheapest first. Apex and Value are assessed independently. A linked or airborne specialist earns its place only when the rest of that deployment plan is legal and useful.

| # | Doctor / **specific profile** | Apex | Value | **Why the rank holds** | **Cost / rules caveat** |
|---:|---|:---:|:---:|---|---|
| 1 | **Rahman Rouhani21/0** WIP15, Doctor(+3), NWI — **Ramah** | S | S | 90% contact healing plus Wildcard/Fireteam delivery; a 21pt recoverer for valuable Cubed HI and scorers. | Qapu Khalqi records a distinct **Doctor(+1)** profile; do not transfer Ramah's +3 to QK. One Wound and no far-flank entry. |
| 2 | **Hakim24–25/0** Doctor(+3), WIP15; **Nasmat A2 option** — Ramah | S | S/A+ | 90% healing coupled with Parachutist edge entry and a Servant route; can recover where a DZ doctor could never arrive in time. | Legal edge, safe arrival and compatible Servant placement are mandatory; not an automatic 1-Order revive. |
| 3 | **Parvati36/0** WIP15 Doctor(2W) + Engineer, Super-Jump — Starmada/eligible O-12/ALEPH | S | A | Best **two-Wound** medical return on a premium VITA target while doubling as durable STR2 repair/mission support. | Doctor is **75%**, not 90%; Engineer(+3) is confirmed in pinned **Starmada**, not necessarily every roster. Costs 36pts. |
| 4 | **Avicenna28/0** WIP15 Doctor(+3), NWI — Bakunin/StarCo, and other verified rosters | S | A+ | 90% healing with MOV15-5, survival, and legal Riot Grrl/Moderator-style team escort; outstanding forward doctor. | No Engineer; more than twice the price of a basic 11–14pt doctor if she never reaches an elite patient. |
| 5 | **Asawira Doctor(+3)35–37/0** — Hassassin Bahram | S | A | High-reliability Doctor on a **two-Wound** assault HI that can fight and score inside legal Bahram teams; demonstrated with Asawira/Lasiq and Muyib formations in #072/#091. | Not interchangeable with a cheap Ghulam; a valuable offensive member must survive and reach the patient. |
| 6 | **Sophotect25/0** WIP15 Doctor + Engineer, MOV15-10, NWI — ALEPH/OSS | A+ | S | 75% Doctor but also high-WIP Engineer and fast access to two casualty types; outstanding all-list support for HI+REM/TAG. | Does **not** have Doctor(+3); spare Servants cost points and do not supply Orders. |
| 7 | **Machaon37/0.5** WIP15 Doctor, Smoke, Mimetism(-6), NWI — Steel Phalanx | A+ | B/A | Forward Myrmidon Core participant with strong combat/mission utility; #190 actually fields Phoenix + Machaon + Myrmidon. | Normal Smoke, not Eclipse; 75% base Doctor and no +3 or 2W. Poor value as a rear-only medic. |
| 8 | **Med-Tech Obsidon21/0** WIP14 Doctor + Engineer, MOV15-10 — eligible Combined sectorials | A+ | S | Fast 70% dual-skill support with optional Slave Drones, useful for Q-Drone/Overdron and organic casualties alike. | S3 body needs safe cover and real Servant placement; a failed Doctor roll can kill the patient. |
| 9 | **Ghulam Doctor(+3)15/0** WIP14 — Ramah/eligible Haqq | A+ | S | 85% Doctor for 15pts, Regular Order and native link utility; #073 fields a Ghulam Doctor alongside Rouhani in a four-person Core. | One Wound and no movement trick; a cheap scorer/Paramedic can suffice for lists with few VITA patients. |
| 10 | **Kumotail21/0** WIP14 Doctor + Engineer — Tohaa | A | S/A+ | Dual-role Triad member with optional Chaksa Servant; named in Tohaa support Haris/Triad plans (#113/#119). | 70% Doctor; a deployed active Servant can conflict with Fireteam use, and 1W body is fragile. |
| 11 | **Mother Agatha31/0** WIP14 Doctor(2W), Mimetism(-6) — Bakunin | A+ | A | Two-Wound recovery, close defense and Reverend/Observance-team delivery; present in #085/#095 played links. | Costly 1W frontline doctor; **Doctor(2W)** changes wounds restored, not WIP odds. Do not buy solely as 31pt hospital. |
| 12 | **Dr. Claire Lazhari33/0** Doctor(2W) **or** separate FTO Doctor(+3) — roster-dependent | S/A+ | B/A | Pick 2W for wounded elites, or the **different** WIP14+3 FTO for 85% one-Wound reliability and team delivery. | These advantages do **not** coexist on a single selected profile; 33pts and FTO access need verification. |
| 13 | **Khawarij Doctor(+3)30/0** — Ramah | A+ | A | Super-Jump/15-5 delivery alongside Tarik; named Khawarij Doctor/Paramedic Haris in #061/#073. | Wounded assault group must still be reachable; one-Wound doctor is exposed and 30pt price is not cheap insurance. |
| 14 | **Muyib Doctor(+3)** — Hassassin Bahram | A | A+ in team | High-odds embedded healer on useful Muyib/Bahram gun or specialist teams; played with Asawira + Govad KHD in #205. | Specific roster price and formation required; a recorded **two-Haris** arrangement cannot be copied into N5.3. |
| 15 | **Tuareg Doctor** WIP15, Hidden Deployment — Ramah/eligible Haqq | A (reach) | A | Begins concealed closer to hostile midfield casualties; #073 reveals a Tuareg specialist for mission tasks. | Hidden state/deployment brings cost; reveal, contact and healing still take Orders; no automatic Doctor(+3). |
| 16 | **Hospitaller Doctor30** — Military Orders | A+ (team) | B/A | Stays with an advancing Knight team, reducing travel Orders and remaining a credible armored mission piece. | Usually overkill for unlinked rear support; expensive HI concentrated with the patient. |
| 17 | **112 Emergency Service11/0** or **motorized19/0** WIP13 — eligible Ariadna | A (bike reach) | S cheap / A bike | 11pt plain Doctor or smoke/mobility on motorcycle; strong alternative to expensive elite medical profiles. | 65% contact and most Ariadnan patients lack Cube-token Doctor rerolls; motorbike is more exposed. |
| 18 | **Bipandra23/0 or TacAware25/0** WIP13 Doctor, MediKit(+1B) — Kestrel/eligible PanO | A (team) | B/A | Legal linked specialist with personal Tactical Awareness option; #005 uses Bipandra/Crux/Fennec and Kestrel guides favor Griffin pairing conditionally. | 65% basic Doctor; **no verified Doctor(ReRoll)** on pinned profile. Many lists prefer Fennec Paramedic. |
| 19 | **Infirmarer of St Lazarus17–20** — Military Orders | B/A | A (linked) | Affordable linked Doctor on Order Sergeant/Velox-support routes; can cover mission scoring while Knights lead fights. | Support quality depends on exact Fireteam/profile; not elite WIP/Doctor(+3) recovery. |
| 20 | **Lambda Doctor** — O-12/eligible sectorials | B/A | A+ | Budget Regular medical coverage with Yudbot Servant network instead of paying Parvati36. | Doctor and **Lambda Engineer16** are distinct selections; do not assign both skills to one Lambda. |
| 21 | **Daktari14/0** — Nomads and other verified rosters | B/A | A+ | Cheap conventional Doctor plus Servant route; #211 includes a Daktari in Corregidor's linked infantry support. | WIP13/65% and 1W; **not** Yu Jing/JSA's generic doctor. |
| 22 | **Zhanshi Yīshēng14/0** — Yu Jing/IA | B/A | A+ | Low-cost Doctor specialist in Zhanshi/Haidào groups (#212), with Yáozăo options as legal. | 65% contact; exposure and legal roster requirements matter. |
| 23 | **Tokusetsu Doctor14/0** — JSA | B/A | A+ | Cheap JSA Doctor and legal Servant delivery for a supporting specialist role. | 65% success; mostly STR-based list might benefit more from Engineer. |
| 24 | **Kazak Doktor12/0** WIP13 — TAK/Kosmoflot | B/A | S/A | Inexpensive Regular Doctor, retains budget for more attacks and objectives. | Ariadna No-Cube casualty often cannot use Command Token repeat of a failed Doctor roll. |

**Evidence check:** [Ramah](../factions/ramah-taskforce.md) (#073 Ghulam/Rouhani and Tarik/Khawarij), [Hassassin](../factions/hassassin-bahram.md) (#072 Asawira Doctor Core; #091 Haris; #205 Muyib), [Bakunin](../factions/bakunin.md) (#085/#095 Mother Agatha), [Steel Phalanx](../factions/steel-phalanx.md) (#190 Machaon), and the [battle-report unit-effectiveness synthesis](../battle-reports/unit-value-role-effectiveness-n5.md). A played Fireteam demonstrates *delivery/role overlap*, not a measured Doctor success rate or proof the Doctor actually revived someone.

### Doctor priority: success, *amount* or delivery?
1. **Need to revive a 2–3W VITA attacker?** Parvati/Claire **Doctor(2W)** may make one action save two Wounds. If merely one removed Wound matters, Rouhani/Hakim **Doctor(+3)** provides higher base success.
2. **Need to reach a casualty behind enemy midfield?** Hakim parachute/Servant A2 and Tomcat rescue may beat WIP18 that starts stuck in home DZ.
3. **Few Cubes and no 2W premium VITA?** A cheap Regular Doctor at 11–15, Paramedic, or **Speedball VitaPack** often dominates support spending.
4. **Doctor inside Fireteam:** it advances naturally **if legal**; deploying Servo bots can conflict with Fireteam membership. Do **not** assume both benefits coexist.

## 3) Engineers — apex / points-value tiers

**Ranking basis:** the number orders *overall practical recovery ceiling* in a 300-point list (reliability, reachable casualty, useful second job, survivability, Fireteam legality), **not** cheapest first. Apex and Value are assessed independently. A linked or airborne specialist earns its place only when the rest of that deployment plan is legal and useful.

| # | Engineer / **specific profile** | Apex | Value | **Why the rank holds** | **Cost / rules caveat** |
|---:|---|:---:|:---:|---|---|
| 1 | **Sophotect25/0** WIP15 Engineer(ReRoll WIP=X) + Doctor — ALEPH/OSS | S | S | Fast dual-role NWI Controller, Yudbot reach and premium WIP for REM/TAG + VITA lists; #072 has Sophotect in OSS support. | Read exact printed reroll WIP=X; the Engineer reroll does not apply to Doctor. |
| 2 | **Parvati36/0** WIP15 Engineer(+3) in **Starmada** + Doctor(2W) | S | A | 90% first Engineer roll on **confirmed +3 Starmada** profile, durable STR2 Remote Presence, Super-Jump and two-patient classes. | Other pinned O-12 rows differ (+1); do not generalize +3. 36pt investment only justified with valuable targets. |
| 3 | **Johnny Kao36/0** WIP14 Engineer(ReRoll WIP=X), GizmoKit(+1B) — eligible ALEPH/Yu Jing | S | A/B | Durable mobile 2W repair and anti-tech tool, especially when advancing with TAG/MAX-OP or fighting across midfield. | A costly combat role competes with protected repair; the printed reroll threshold must be checked. |
| 4 | **Med-Tech Obsidon21/0** WIP14 Engineer + Doctor — Combined | A+ | S | 21pt fast 70% engineering and organic healing; Slave Drone routes cover Q-Drone/Overdron and other casualties. | Large S3 Controller and expensive-to-expose support network. |
| 5 | **Clockmaker18/0** WIP15 — Nomads/Bakunin/Tunguska/eligible | A+ | S | 75% WIP with Zondbot(s) and Remote Presence token repeat; repairs TAGs/REMs at bargain Regular-Order cost. | One Wound and ordinary rear movement; must preposition Servants near the actual fall-back route. |
| 6 | **Posthuman Mk.1 Engineer13/0** WIP15 — OSS (G:Jumper) | A+ | S in mandatory Proxy set | WIP15 repair from one location while another Proxy fights or scores; OSS #205 uses Mk.1 + two Yudbots and Mk.5. | **Not a standalone 13pt Regular engineer:** minimum legal 2–3 Proxy selection (e.g. Mk.1+Mk.5 =26/.5), **one shared Regular Order**. |
| 7 | **Kumotail21/0** WIP14 Engineer + Doctor — Tohaa | A | S/A+ | Triad specialist whose second skill genuinely matters in mixed VITA/STR Tohaa; #113/#119 use it with scoring teams. | 70% repair; Servant/active Fireteam restrictions and 1W survival still apply. |
| 8 | **Artalis Engineer23/0** — OSS | A (team) | A+ | Repairable Riksha/Rudra and specialist roles in OperationS; #072 played Artalis Haris, #145 describes a **tentative** Rudra/Dikpala/Artalis formation. | #145 named four-body formation is reconstructed, **not** proof of a certified current Army export. Not a cheaper 15pt repairer. |
| 9 | **Chung-Hee Jeong31/0** WIP14 Engineer(ReRoll) — IA/White Banner | A+ | A/B | Durable toolbox value from Repeater/turret and reroll when those defenses support the same STR targets. | 31pts over bare 14pt Mech-Engineer; reroll WIP=X and actual roster must be checked. |
| 10 | **Krit Kokram37/0** WIP14, 2W Engineer/NCO — IA/Yu Jing eligible | A+ (team) | B/A | Forward engineering with powerful HI fighting/Order utility; #068 uses Krit with Hǎidào/Zúyǒng. | 37pts is too much for a hidden backline TAG mechanic; verify specific FTO and link legality. |
| 11 | **Orphan Engineer17/0 or 21/0** (+Repeater/E/M mine) — Bakunin | A (delivery) | S/A+ | Excellent value embedded in 56pt Stigmata or Lizard **Armored Duo**; #110 plays distinct Orphan models in Haris and TAG Duo. | 17/21pt Engineer is **not** the 25pt MSV2 MMR shooter; linked model must match exact legal team. |
| 12 | **Lambda Engineer16/0** WIP14 — O-12/Starmada/Torchlight | A | S | 70% engineer plus 3pt Yudbot extends covered access to Zeta/REM; preferred when not paying for Parvati's second job. | WIP14 not 15; backline speed/low durability make early Servant positioning essential. |
| 13 | **Najjarun Engineer15/0** WIP14 — Haqq/Ramah/eligible | A | S | 70% protected repair for Shihab/other REMs and TAG with Nasmat, while cheap Ghulam/Rouhani provide VITA care. | Only STR and states, not Doctor; pay for reach rather than redundant forward combat loadout. |
| 14 | **NCA Blade Engineer23 FTO / 30 Parachutist** — NCA | A+ (reach) | A+ conditional | 23pt Fireteam repair follows Bulleteer; **distinct 30pt side-entry Decoy/EMitter** can find far-forward Redeye/REM (NCA guide and interview). | FTO and Parachutist cannot be merged; legal drop zone, Servant availability and safe contact can fail. |
| 15 | **Carlota28/0** or **32 incl. Moriarty** — Corregidor | A+ (reach) | A | Parachutist/Climbing Plus and WIP14 make far-flank repair credible when TAG/REM is past the rear Zondbot. | Higher price than Tomcat or ordinary engineer; no safe edge means poor recovery. |
| 16 | **Tomcat Engineer22/0** or **26 incl. Zondcat** — Nomads/Corregidor | A (reach) | A+ conditional | Parachutist/Climbing Plus produces short-path repairs on a distant flank and remains mission-capable. | WIP13, timing and entry safety; not guaranteed to recover a destroyed far-forward unit. |
| 17 | **Fiddler FTO Engineer29/0** or **separate 36/43 JackBot profiles** — Bakunin/eligible | A (combat/specialist) | A conditional | WIP14 engineering with Super-Jump in a legal Riot Grrl group or independent JackBot-enabled pressure, as roster permits. | **29pt FTO has no JackBots**; do not count bots as free independent Engineers or Regular Orders. |
| 18 | **Evader Engineer24–35** — Corregidor | A (midfield) | A/B | NWI/Climbing Plus, linkable combat gear and anti-hack coverage allow repair without abandoning an advancing unit. | Price rises sharply for active gun profiles; choose only if fighting/mission/Repeater role also justifies points. |
| 19 | **Firefly Engineer23/0** — Kestrel | A (team) | A | Useful linked Deactivator/Engineer in Griffin anti-armor Duo; #002 includes Griffin+Firefly and Kestrel guide ties it to TAG/REM support. | A linked 23pt specialist is not a cheap isolated WIP12 Machinist replacement. |
| 20 | **Hǎidào Engineer25/0** — IA/Yu Jing eligible | A (embedded) | A | Engineer Wildcard supports HI team/hacking-defense architecture; fits role-compression when no rear Servant route works. | The MSV2 sniper and KHD/Pitcher are **different** Hǎidào profiles. |
| 21 | **Mech-Engineer14/0** WIP13 — Yu Jing/IA/White Banner | B/A | S/A+ | 14pt conventional Regular engineer with Yáozăo and Remote Presence token repeat; strong for static Guijia/Long Ya infrastructure. | 65% first roll and exposed/slow route; #003 warns spent Long Ya may not justify a repair detour. |
| 22 | **Dozer13/0** WIP13; **2pt Remontnik** extra — Ariadna/TAK/Kosmoflot | B/A | S | 15pt with one Servant, cheap covered repair for Chernobog/REM and mission disabling-state clearance. | Not equivalent to elite WIP15; little return in a roster without STR or mission Engineering. |
| 23 | **Irmandinho8/0** WIP13 Irregular Engineer — Ariadna | A (trader) | S contextual | Remarkable 8pt Smoke/E/M/Chain Rifle trader who sometimes repairs or clears a state on the way to objective. | Irregular/Impetuous and No Cover exposure make it **poor dedicated protected TAG insurance**. |
| 24 | **Monstrucker12/0** WIP13, Irregular Engineer — eligible Haqq/O-12/etc. | B/A | S conditional | Climbing Plus and cheap utility/Drop Bears make sparse-list engineering possible; often backs cheap TR bots. | Irregular Order reduces passive Order value; actual Servant and active recovery movement still cost actions. |
| 25 | **Genbutai Engineer23/0** — JSA | B/A | A | Repair specialist plus Panzerfaust/Warhorse, useful when a JSA team needs front-adjacent recovery and a second tool. | 23pts is a big premium above Tokusetsu14 if no forward specialist job materializes. |
| 26 | **Tokusetsu Engineer14/0** — JSA | B/A | S/A+ | Cheapest conventional JSA TAG/Karakuri repair plus optional Yáozăo; reliable points value when hidden. | WIP13 first roll, needs patient near covered Servant rather than exposed far midfield. |
| 27 | **Yuriko Oda Engineer25/0** (verify FTO) — JSA | A (mission/denial) | B/A | Mines/Mimetism and forward specialist control while keeping Karakuri/O-Yoroi in play. | Expensive pure Engineer, exact team profile and minelayer tool vary. |
| 28 | **Kosuil Engineer20/0 or 25/0** — Tohaa | A (team/combat) | A | K1 or shotgun/anti-TAG weapon and Triad access make an Engineer useful in midfield combat/repair. | **Kosuil Minelayer is not Engineer**; do not assign both to a single profile. |
| 29 | **Wildcat Engineer25/0** — Corregidor | A (team) | B/A | Deepspace Gator support in a legal Duo (#211) where specialist mobility and anti-Stealth tools are relevant. | Too expensive versus independent Clockmaker for static REM or backline repair. |

**Evidence check:** [OSS](../factions/operations-subsection.md) (Posthuman Mk.1 and Artalis; #072/#145/#205), [Bakunin](../factions/bakunin.md) (Orphan TAG Duo in #110), [NCA](../factions/nca.md) (two distinct Blade Engineer routes), [Kestrel](../factions/kestrel.md) (Firefly), [Corregidor](../factions/corregidor.md) (#211 Wildcat/Gator), and [battle-report value analysis](../battle-reports/unit-value-role-effectiveness-n5.md) (#019 Squalos repair; #092 Cutter repaired before decisive REM scoring; #193 recovered ISS casualties). These cases favor **safe access and subsequent scoring**, not just paid WIP or a powerful on-paper loadout.

**Engineer priority:** select the cheapest legal *safe route* to a valuable recoverable STR target, usually WIP14–15 plus Servant. Upgrade to forward, reroll, linked, airborne, or dual-role Engineer only when its second function actually matters. For small already-expended REMs (e.g., the #003 Long Ya), sometimes **do not spend the repair Orders**.

## 4) Servant positioning and true Order efficiency

- **Standard Servant options** (as permitted by the selected roster):
  - **Palbot** — 3pt
  - **Zondbot** — 3pt
  - **Nasmat** — 3pt
  - **Yudbot** — 3pt
  - **Yáozăo** — 3pt
  - **Slave Drone** — 3pt
  - **Chaksa** — 3pt
  - **Ariadna Remontnikbot** — 2pt where rostered

  Common movement **15-10**, tiny S1, Mimetism−3; these do not provide an independent Order.
- **A Doctor/Engineer Controller may take at most two Servants** and activate only **one** at a time; Servant is not a new unit/Order, and **the Controller's WIP performs the skill roll**.
- Put **Servant A one protected Move away from expensive ARO shelf; Servant B one protected Move away from a TAG's likely fallback angle.** Do **not** leave both beside Controller, beside each other, or within a single template/repeater kill zone.
- **Turn 1** preposition while the expensive shooter moves in an orderly route; then use a second combat group's spare Orders for rescue where available. Two Servants in one combat group **do not** provide two support activations simultaneously.
- Do **not** assume Servant and Controller in legal Fireteam: [Peripheral](../../rules/5b_Special%20Skills/Peripheral.md) normally prevents Controller with deployed Peripherals participating in a Fireteam; **N5.3 Ancillary/Cyberplug exceptions and integrity changes** need exact application.
- **Doctor/Engineer and MediKit/GizmoKit are different rolls and functions.** Controller with Servant uses Controller's WIP Doctor/Engineer; **firing** a MediKit/GizmoKit requires a BS hit **followed by patient PH**. Multiple Medic/Gizmo successful hits in same Order can improve odds of at least one PH success, **not** multiple restored Wounds.
- **Tech-Recovery versus Unconscious:** Tech-Recovery state-clear **does not itself revive Unconscious**; a legal Engineer or successful GizmoKit on STR can revive first. If stunned/isolated/immobilized but *not Unconscious*, prioritize one safe Engineer state-clear.
- **Target evaluation:** Enemy may **finish off** an Unconscious model, forcing extra enemy Orders; **that alone can pay for some support investment**, but never automatically count an unattainable future resurrection.
- **After revival:** If target stands in enemy sight lines, plan suppress/Prone/safe reposition where legal; REMs/TAGs generally cannot Prone. Avoid increasing enemy ARO kill opportunities just to claim a recovered point value.

## 5) Contradictions, unpopular choices, and transcript-checked sources

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

## 6) Sectorial quick-reference: what changes when choosing a healer

**PanO/Kestrel/NCA/MO/Varuna/WinterFor/Acontecimento:**

- 14pt **Trauma-Doc WIP12** with **Palbot3** is cheap but failure risk is real (60%; 84% Cube+token)
- **Machinist WIP12** similarly wants Remote Presence token support.
- **Bipandra23–25** helps in linked Kestrel, but not a universal upgrade.
- NCA **Blade Parachutist Engineer** recovers Redeye on far flank, where a DZ Machinist cannot.

Hospitaler Doctor is better inside a moving MO Knight team; **don't assume Servant-equipped Controller remains linked**.

**ALEPH/OSS/Steel:**

- **Sophotect25 + Yudbot(s)** is among best whole-list returns on a 300pt mixed army
- **Parvati36** is better where 2W Doctor or mobile high-end Engineer is actually needed
- **Posthuman Mk.1 Engineer** creates extra slot/mission economy **only inside a legal 2–3 Proxy package**.

Do not count a Mk.1 as independently fieldable cheap Engineer.

**Nomads/Tunguska/Corregidor/Bakunin:**

- **Clockmaker18 + Zondbot3** often beats a 30pt toolbox repairer for pure REM/TAG infrastructure.
- **Multirole Engineer options:**
  - **Evader** — when its gun/Repeater/link utility matters
  - **Orphan Engineer** — for the same type of role compression.
- **Far-flank recovery:**
  - **Tomcat22/26**
  - **Carlota28/32**

  Both can bypass a long movement tax where their deployment modes are legal.
- **Wildcat Engineer25** is controversial toolbox spending when its team doesn't use MSV or gear.

**Combined/Shas/Onyx/Next Wave/Morat:**

- **Med-Tech21 + 3pt Slave Drones** is standout cheap dual hub, but tall S3 deserves concealment
- **Gearhead Cyberplug** can project engineering differently and **cannot** also take Servants.
- **Kurgat** buys combat-ready Morat engineer; cheap regular alternatives should be measured against actual need to repair TAG/REM versus spending more on weapons.

**Haqq/Ramah/Hassassin/QK/Dahshat:**

- **High-reliability Haqq Doctors** (check exact legal roster):
  - **Ghulam Doctor15(+3)**
  - **Rouhani21(+3)**

  Their recovery success probabilities span approximately 85–90% under the stated modifiers.
- **Hakim** wins where Parachutist/Nasmat A2 makes recovery physically possible
- **Najjarun15** repairs STR
- **Monstrucker12** sacrifices Regular Order for a cheaper technical specialist.
- **Claire** 33pt different **2W versus +3 FTO** profiles are situational, not interchangeable.

**Yu Jing/White Banner/IA/IS:**

- **Mech-Engineer14 + Yáozăo3** is efficient normal recovery
- **Krit Kokram37** moves with HI gun team
- **Chung-Hee Jeong31** buys ReRoll/Repeater specialist protection
- **Johnny Kao36** more durable frontline anti-tech.

Every expensive Guijia/Blue Wolf TAG benefits from deliberate fallback and remote repair position.

**Ariadna/TAK/Kosmoflot/USAriadna/Caledonia/FRRM:**

- **Irmandinho8** is an extraordinary cheap smoke/trading/engineering combination but not your only safe TAG mechanic
- **Dozer13 + 2pt Remontnik** builds covered STR recovery cheaply.
- **Inexpensive Ariadna medical choices:**
  - **112 Doctor11**
  - **Motorized 11219**
  - **Kazak Doktor12**

  **No-Cube** patients lack Doctor token reroll protection.

**O-12/Starmada/Torchlight:**

- **O-12 low-cost support package:**
  - **Lambda Engineer16** or the distinct **Lambda Doctor** variant
  - **Yudbot3** as the accompanying Servant

  This is sufficient for many Wrecker/Zeta/REM recovery needs.
- **Parvati36** does something distinct with **2W Doctor, high Engineer, mobility, STR2**.
- **Kludger23**
- **Vidocq FTO Doctor19**
- **Delta forward support** win by arriving with legal team/route rather than by maximum backline WIP.
- For aerial **Firebat**, use ranged GizmoKit/Tech-Recovery when contact cannot be reached safely.

**Tohaa/JSA/Oban/Shindenbutai:**

- **Kumotail21** dual role with Chaksa3 supports mixed Tohaa attack Triads
- **Kosuil20–25** trades cheap backline Doctor/Engineer economy for a K1 assault Engineer actually in the midfield.
- **Tokusetsu14**
- **Yáozăo3**
- **Yuriko25** form JSA's economical recovery plan for **Karakuri Remote Presence / O-Yoroi**; do not spend extra on forward engineer if patient remains near DZ.

### Final list-building test

1. **Recoverable patient:** Which VITA or STR units can actually enter eligible states rather than Dead/Dogged?
2. **Real chance:** What is **contact WIP**, and is a Cube/Remote Presence token reroll legal? If ranged, what are **BS hit × patient PH** and ARO hazards?
3. **Actual distance:** Where does the patient likely fall, and how many safe **Orders to contact, roll, and redeploy**? Are Servants prepositioned?
4. **Second job:** If no one needs recovery, does support still supply **Regular Order, scoring, Mine/Repeater, smoke, gun or Hacker protection**?
5. **Opportunity cost:** Is 6+ extra support points better than a second attacker, additional Specialist or protecting attack's retreat lane?

**Bottom line:** **Choose *reachability* first, *roll reliability* second, and *points cost* third** for a specific casualty. Then check whether not taking a healer at all scores more.

## Battle-report checks — observed unit effectiveness and combinations (2026-11-01)

**Observed enabling recoveries:**

- #003 Kestrel's **Engineer / Sensor REM recovery** restored access to a Frostbyte heater
- #004 **Trauma-Doc** recovered **Black A.I.R.** under Torchlight pressure
- #220 a recovered **Shikami** supported JSA's Hardlock winning route
- #205 fields **Muyib Doctor** in an Asawira/Govad team supporting cargo control (a played team, **not** a confirmed successful healing roll)
- #227 NCA **Shona/CSU/Blocker** converted cleared lanes while other pieces carried recovery duties. [#003–#004](../battle-reports/001-010-n5-battle-report-tactical-analysis.md) · [#205](../battle-reports/201-210-n5-battle-report-tactical-analysis.md) · [#220](../battle-reports/211-220-n5-battle-report-tactical-analysis.md).

**Marginal value:** Spending Orders to repair an expended **Long Ya** that has already lost first-use missiles and Camo threat (#003 player's question) may be lower value than a newly needed console/pickup. An **EVO** sacrificing itself to clear a mine for **Kurnau** (#212) shows how cheap technical bodies sometimes produce more OP as expendables than as survivors. Choose repairs by **future mission ability restored**, not model cost alone.

[Full cross-report analysis and source limitations](../battle-reports/cross-report-unit-effectiveness-and-combinations.md).
