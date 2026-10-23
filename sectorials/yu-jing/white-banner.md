---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 205
sectorial_slug: white-banner
sectorial_name: White Banner
parent_faction: Yu Jing
rules_baseline: N5.3
army_source_version: "7.26246.158"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-15
coverage: "Standard White Banner roster, standard loadouts, canonical Fireteam chart, and reverse Fireteam index. Guǐ Fēng Spec-Ops and Yu Jing Team-Ops are optional-mode hooks rather than ordinary matched-play roster entries."
---

# White Banner

## Overview and provenance

Repository-native reference for **White Banner** roster, profiles, points/SWC, AVA, and Fireteam access.

Sources used:

- Army-derived White Banner source revision `7.26246.158` from `massayoshi/infinity-army-backup` commit `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b`.
- InfinityDB Fireteam normalization/semantics at commit `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: N5.3 + N5 FAQ v0.1.

Coverage notes:

- Covers the **46-unit standard White Banner roster** and the complete White Banner `fireteamChart` in the pinned Army source.
- Soldier of Fortune / generic mercenary-catalog entries whose source faction list is empty are excluded from the base roster.
- `Guǐ Fēng Spec-Ops` and `Yu Jing Team-Ops` are optional game-mode content and are listed separately.
- Fireteam legality comes from the canonical chart below, not from an `FTO` loadout name by itself. Son-Bae and Pangguling both have FTO-labelled options but no White Banner Fireteam-chart row.
- Parenthetical Army-chart comments are treated as Counts-as / equivalence labels, not as join-scope restrictions.
- The structured `required: true` rows in White Banner and Shaolin Fireteams are preserved as required-choice sets; this file does not reinterpret them as requiring every marked unit type simultaneously.
- Profile restrictions are preserved: Gūdǎn and Beasthunter only join the Zhanshi team through their FTO profiles; Tian Gǒu and Léi Gōng are Wildcards only through their FTO profiles; Guǐ Fēng is a Spec-Ops-mode Zhanshi-team entry.
- Linked Reinforcement army ID: **299**. Reinforcement Fireteam rows are not merged into the main chart here.

## Sectorial summary

| Field | Value |
|---|---|
| Sectorial | White Banner |
| Parent faction | Yu Jing |
| Army ID | 205 |
| Rules baseline | N5.3 + FAQ v0.1 |
| Standard roster units | 46 |
| Optional-mode units | Guǐ Fēng Spec-Ops; Yu Jing Team-Ops |
| Reinforcement roster | Army ID `299` |
| Fireteam limits | Core 1; Haris 1; Duo unlimited |
| Fireteam chart | yes |

## Tactical research — White Banner N5 (2026-10-22)

> **Interpretation, not replacement Army data.** The canonical N5.3 roster and Fireteam chart below (Army 7.26246.158, September 2026) take precedence over speaker recollections, older points and N4 examples. Opinions are identified by source. In particular, the current White Banner roster has **Blue Wolf TAG (AVA 2), Gūijiă TAG (AVA 1), Fēiquán vehicle/VH (AVA 1)**, and *neither Son-Bae nor Pangguling FTO can Fireteam in this sectorial* despite their FTO names.

### The 30-second list-building plan

**White Banner wins by layering low-cost defensive problems in front of a versatile, objective-capable attack force.** It combines cheap Gūdǎn and Lóng Yá denial, Shaolin smoke/CC, midfield Camo, high-value mixed Fireteams, and several independent specialists. Its constraints are **costly premium solo pieces, limited MSV2, sometimes weak ranged answers to Mimetism, and competing demands on its single Core and Haris slots**.

1. **Buy a deployable defensive floor:** Usually 1–3 **Gūdǎn one-use Camo/forward deploy + Zapper or HFT**, optional **Lóng Yá Minelayer/Panzerfaust/Flammenspeer**, **Hùndùn Hidden Deployment HRL**, a 7-point Chaīyì or a Shaolin screen. Put templates/mines where enemies must cross, not where they can safely ignore them.
2. **Choose *one* major team plan:** **Jujak Firewall(-6) + Hwarang Disco Baller + Haetae HRL Guided/TacAware + Dokkaebi Pitcher/Spotlight** is the proven all-purpose package; or **Yě Māo + Yín-Shé** for MSV1/Mimetism plus **Albedo(-6)/K1 Sniper** versus enemy visors; or a smaller **Zhanshi/Shàng Jí** link with a reliable Doctor and more budget for independent operators. Those aren't equally suited to every mission.
3. **Reserve points to play objectives outside the main team:** **Guìláng** midfield FO/hacker/Minelayer, **Dàofěi** infiltrating two-Wound HI specialist (including LT options), **Shaolin + Liang Kai** to clear rooms in melee, **Kunai T2 Thunderbolt/Para Mine**, **Tiger Soldier** for true Combat Jump, or Léi Gōng for a fast flanking/anti-MSV role.
4. **Don't mistake maximum list size or maximum gun power for a plan:** a short burst of heavy attacks wins a lane, but missions need buttons/classifieds, dispersed board presence, an LT fallback and enough regular orders after casualties. WIP12's experienced tournament guest Axel specifically favors spreading abilities across inexpensive units over making one unanswerable death-star.
5. **Use smoke, Albedo and visors deliberately:** Shaolin smoke shields against normal LoF; Hwarang Disco Baller helps HI advance; **Yín-Shé Albedo(-6)** is an answer to enemy MSV troops *not* a generic Mimetism modifier against everyone. **Rui Shi MSV2** is White Banner's unusual smoke-shooting option, but is fragile and unlinked here. Against Mimetism(-6) MSV AROs, move around or attack with another tool instead of feeding a BS13 gun directly into them.
6. **Build legal teams:** **Core 1, Haris 1, Duos unlimited.** White Banner's Shàng Jí / Jujak / Yě Māo / Yín-Shé are a **required-choice set**, not an instruction to field all four. Jujaks count as Shàng Jí; Yín-Shé as Yě Māo; Hwarang as Jujak. **Blue Wolf Duo** needs 1 Blue Wolf and can include one Shàng Jí, or use two Wolves. **Shaolin Duo/Haris** starts from Shaolin or Liang Kai and can include Jing Qo Wildcard where allowed. **Tian Gǒu/Léi Gōng** are Wildcards on FTO profiles only. Standard Pangguling and Son-Bae, including FTO-labelled versions, remain unlinked here.

### Short unit decisions — with the why

| Piece | Why you take it | When not to / disagreement |
|---|---|---|
| **Gūdǎn 12–13pt Camo screen** | Regular cheap order, one-use Camo, forward Shock Mine, Zapper (stops TAG/HI/warbands) or HFT (punishes groups). Three can layer the whole DZ, preserving expensive turn-one pieces. Strong agreement across Shepherd, Irregular Order and Tactical Awareness. | A defensive picket is a *trade*, not an alpha-strike gun. Taking three is common but not compulsory when deploying many other hidden/independent units. The FTO **linkable** profiles differ from the Camo screen. |
| **Jujak + Hwarang + Haetae + Dokkaebi** | Jujak **27/28pt TinBot(-6)** gives hacking protection; **20pt Hwarang Disco Baller** gives LoF control and CC; **36pt Haetae HRL(+1B), Guided, Tactical Awareness** is a strong active/ARO shooter and targeter payoff; **22pt Dokkaebi KHD/Spotlight + Pitcher** or 23pt normal hacker/Carbonite projects hacking. Team has guns, smoke-like cover, hacking, templates and mission options. | Shepherd calls this the familiar default, but warns it can become the *only* list people build. **Dokkaebi normal HD vs KHD** is a real disagreement: HD/Carbonite/Oblivion give better nonlethal ARO control, while KHD/Spotlight creates the easy Haetae Guided pairing. Team members must stay alive/linked for bonuses. |
| **Haetae + network (independent of exact link)** | BS14/ARM5, TacAware, 36pt Guided Heavy Rocket Launcher, 40pt AP HMG. **Guided HRL with a Fireteam Special Die** is particularly strong because Guided sets ordinary Burst to 1 yet legal Fireteam Special Die applies; Spotlight can come from Dokkaebi/Guìláng/repeaters. | Not a substitute for objective pieces or for other LoF angles. WIP12's Axel prefers guiding vulnerable specialists and objective threats over sinking multiple orders into an almost unkillable TAG. Verify rules/FAQ and link composition in Army before relying on the Special Die interaction. |
| **Yě Māo + Yín-Shé** | Yě Māo brings Super-Jump, BS13, MSV1, Mimetism(-3), AP Spitfire/hackers/FO; Yín-Shé counts as Yě Māo and supplies **Albedo(-6), K1 Sniper 27pt with Marksmanship**, 22pt Boarding Shotgun Specialist or 24pt FD Minelayer and widespread E/M. A legal pair/Duo can attack visors, armour and objectives in different ways; smoke plus Albedo can be a strong *anti-visor* plan. | Shepherd and contributor Matamori: Yě Māo is **serviceable rather than elite**; single W and investment in short/mid guns makes long-range repositioning difficult. Some players prefer a Yín-Shé/K1 sniper Duo or small team over committing a whole Core. |
| **Shaolin + Liang Kai** | 5–6pt Shaolin provide smoke, Stealth/MA3/CC23 and expendable melee threats; **21pt Liang Kai** supplies FT Master, EXP CCW, Mimetism, NWI, Super-Jump. Cheap Duos/Haris can clear rooms late and allow Regular-order activity while keeping smoke. | Must manage Impetuous/No Cover and exposing monks. Jing Qo (32pt) can be a versatile alternative leader/CC piece, but Shepherd finds her overcosted for her usual MULTI Rifle outcomes; Irregular Order values her mission/CC flexibility. |
| **Guìláng / Dàofěi LT or Specialist** | **Guìláng** Camo/Infiltration, WIP14, MSV1: 25pt repeater Minelayer, 27pt FO, 31pt hacker, 23pt Camo LT. **Dàofěi** 52pt Camo Infiltrating ARM4/2W HI, AP Spitfire specialist/lieutenant or MULTI Rifle hacker/lieutenant; can gunfight, score and do many Classifieds. | **Sharp disagreement:** ITS winner Axel repeatedly plays Guìláng and even the Camo LT for board control, despite conceding points are high; Shepherd dislikes their expense/Spec-Trained classification and prefers cheaper DZ defence plus more offense. Dàofěi advocate BT Sherman values unusually broad mission/attack reach; Shepherd/Matamori say 52pt is too high unless its mission-specific toolkit earns those orders. |
| **Kunai / Hùndùn** | **25pt Kunai Thunderbolt (T2) + Para Mine** is a Hidden Deployment Mimetism(-6) surprise piece with unusual active-turn flanking; **22pt Hùndùn HRL/X-Visor** is cheap hidden long ARO and disguises whether a trooper might be off-table. | Axel rates Kunai highly from actual tournament use; one-Wound/BS12 and no link make an exposed firefight unreliable. Hùndùn is mainly *information/ARO*, not a durable long-term gun. |
| **Léi Gōng / Tiger Soldier** | Léi Gōng Parachutist 32pt or FTO Wildcard 29–34pt: Albedo(-6), MSV1, Super-Jump, NWI, E/Mitter/Zapper/CoC option. Cheap **20pt Tiger boarding-shotgun Combat Jump** threatens backline; hacker/paramedic variants score. | Irregular Order favors Léi Gōng's extra movement and NWI over an expensive Tiger Spitfire; WIP12's Axel often finds Tigers unnecessary. Tiger has **actual Combat Jump** (Léi Gōng is Parachutist), so only Tiger offers that deployment geometry; EVO can improve the landing roll. |
| **Shàng Jí / Bìxié / Adil / Qiang Gāo** | Shàng Jí AP HMG+TinBot, Tactical Awareness (45pt) gives a protected heavy gun; Bìxié brings NCO/CC/Climbing Plus/FO independent mobility; Adil supplies elite fighting/leadership utility; Qiang's Warhorse/immunities handle some EM-heavy matchups. | Multiple players, notably Shepherd and Irregular Order, find Shàng Jí less efficient than Jujak/Haetae in *this* sectorial (very different from Invincible Army), and Bìxié NCO less valuable where LT+1 Order is rare. Choose for a missing role. |
| **Tian Gǒu FTO / Johnny Kao** | Tian Gǒu FTO Holomask/Jammer, Thunderbolt/E/M or KHD can hide what threatens opponents inside a legal team; unlinked Holoprojector/Minelayer creates marker-state bluff. **Johnny Kao** is a 36–42pt non-hackable, WIP14, 2W Engineer/repair or combat toolbox and can support multiple Lóng Yá or TAGs via servants. | Holomask requires real deception, not just a label. Johnny is expensive for support; Shepherd describes unusual repair reliability, but the *pinned file* only explicitly records Engineer/GizmoKit (no independent Engineer re-roll field): check current Army rules before assuming a re-roll. |
| **Cheap defence package** | White Banner can combine a reliable cheap defensive package (Gūdǎn, Lóng Yá, Chaīyì, occasional Hùndùn) with enough points for a high-value Fireteam and 1–2 midfield specialists. | Shepherd cautions Lóng Yá is somewhat dated relative to newer N5 REMs; Axel and Irregular Order consider the inexpensive mines/long-range disposables an excellent price for redundancy. |

### Vehicles, TAGs, remotes — Yu Jing cross-sectorial context

**Actual White Banner platforms:** **Blue Wolf TAG 70pt AVA2**, **Gūijiă TAG 77pt AVA1**, **Fēiquán VH 27/28pt AVA1**; plus Rui Shi, Lù Duān, Lóng Yá, Chaīyì, Wèibīng, Hùsòng, Son-Bae, Pangguling, Yáozăo. **Sù-Jiàn, Lóngwáng and other Yu Jing sectorial-specific armour are not available in the White Banner main roster.** The Shàngdiào accompanying Blue Wolf/Gūijiă is an ancillary remote, not a second TAG.

| Platform | Purpose: why it might earn its slot | Costs, opposition, and legality |
|---|---|---|
| **Blue Wolf TAG (70pt, 1.5 SWC)** | BS14, AP Spitfire, **BS Attack(+1B)** yields powerful five-dice Spitfire, threatening Heavy Flamethrower and Panzerfaust forks; 3W, ARM6, BTS6, TacAware, CC23/Berserk. **Blue Wolf + Shàng Jí** Duo can add TacAware/TinBot and, on the relevant Shàng Jí profile, a specialist; **double Blue Wolf** is an extreme brawling build. | **Opposed takes:** Shepherd calls it dangerous but very expensive and a niche over a HI Fireteam; **Aug 2026 Irregular Order** considers a 70pt ARM6 TAG with only Spitfire ranges too exposed to hackers and melee and prefers Gūijiă's range/ARM8/MA2; useful mainly where close-range high Burst creates a forcing threat. Standard unit has **no Martial Arts**—do not overstate its CC defence. |
| **Gūijiă TAG (77pt, 1.5 SWC; LT 2 SWC)** | BS14 MULTI HMG / HFT, **ARM8**, 3W, TacAware, **Super-Jump**, CC22 Martial Arts 2, DA CCW: much stronger long-range attack and counter-CC than Blue Wolf, with a mobile specialist ancillary and useful LT possibility. **Johnny/Engineer/servant** substantially changes its durability. | Irregular Order hosts prefer it to Blue Wolf because staying outside hacking/CC range is easier; Shepherd calls it a serviceable but costly main-battle TAG more compelling with reliable repair and occasional LT strategy; **Loss of Lieutenant TAG comparison** remains lukewarm against other factions' TAGs. **No White Banner Gūijiă Fireteam row**; unlike Blue Wolf, it is solo. Do not infer Remote Presence or similar TAG repair bonuses without source confirmation. |
| **Fēiquán VH (28pt E/M Carbine+Pitcher / 27pt MULTI Rifle+X-Visor)** | Aerial VH with MOV20-5, **Sensor**, Super-Jump and high mobility: a speedy extra angle on Camo, forward objectives and enemy hacks/HI. **Pitcher E/M variant** extends a Dokkaebi/Guìláng hacking net; **MULTI Rifle X-Visor** is a cheap independent mobile shooter. | Aug 2026 Irregular Order: White Banner already has good Pitcher/repeater access, so the **MULTI/X-Visor** variant may add more; they also note Sensor is scarce outside dedicated REM. Compared with ISS the network is less critical. **No Cover**, ARM3/2W, limited firepower and no FT access mean it is a disruptive tech piece, not a flying TAG. |
| **Lóng Yá (16–19pt; 17pt Minelayer)** | Camo, Forward Deployment(+10), AP Mines, **Panzerfaust(+1B)/Flammenspeer(+1B)**, 6-4 speed: cheap layered DZ/midfield screen and aggressive expendable ARO. Engineer+Yáozăo or Johnny permits reuse if recoverable; Baggage can replenish disposables. | Axel, Irregular Order and Shepherd all see uses, but differ in valuation: Axel and Irregular Order frequently build with 1–2; Shepherd feels N5 power creep makes it less efficient than newest REMs. **Not linkable** here, and BS11/1W means avoid long fair firefights. |
| **Rui Shi (MSV2 Spitfire 23pt / MSV1 Red Fury + Mine Dispenser 21pt)** | Only **MSV2** option for smoke shooting into uncovered or Mimetism targets; EVO Assisted Fire/Marksmanship improves it, mine variant controls lanes behind Shaolin smoke. | Fragile ARM1/1W, and **no White Banner Fireteam** (unlike Invincible Army and other Yu Jing sectorials). Irregular Order doubts its routine inclusion without EVO/support; Shepherd treats it as a specialist option, not the centerpiece. |
| **Lù Duān (24pt Mk12/HFT or 20pt Thunderbolt/E/M Carbine)** | Holoprojector/echoes, Surprise Attack(-3), MSV1 and BS Attack(+1B); can draw reactive fire, clear mines or place E/M denial from an independent angle. | Irregular Order is cautious: other White Banner utility is often more points-efficient and it is unlinked ARM1/1W. Shared Yu Jing sources describe its value in *other* sectorials as a secondary expendable assault, but that doesn't automatically make it a priority here. |
| **Wèibīng / Chaīyì** | **Wèibīng** (14pt, or 17pt TacAware) adds **Sensor + FO + Repeater** for Camo discovery, Spotlight, mission buttons. **Chaīyì** (7pt) gives cheap Flash Pulse regular Order and repeater lane. Ideal with a Haetae Guided or Son-Bae network. | Neither has White Banner Fireteam access. Paying 17pt for Wèibīng TacAware competes with cheap specialists and 12pt Gūdǎn; value rises with Sensor/FO demand. |
| **Hùsòng / Son-Bae** | Hùsòng Total Reaction long-lane denial complements Lóng Yá and Hùndùn. **16pt Guided Son-Bae** can capitalize on Spotlight; the 19pt +1B Missile is direct ARO fire. Haetae can provide its own linkable Guided HRL, changing guided-missile opportunity cost. | **Son-Bae FTO option 2 is NOT linkable here**: no White Banner chart row. Cannot use linked +1 SD for Son-Bae, unlike Haetae Guided HRL. Beware immobile AROs that can be bypassed. |
| **Pangguling / Yáozăo / Engineer / Qíshì** | Pangguling 8pt Baggage reloads Panzerfaust, Flammenspeer and deployable ammunition; 14pt EVO helps Tiger Combat Jump and REM Marksmanship; Yáozăo projects Engineer repairs, Qíshì **Blue Wolf Pilot** adds a 10pt TAGCom specialist/support option to the force. | **Pangguling FTO 12pt is NOT Fireteam legal** in this sectorial, even though the profile says FTO. WIP12's Axel reports taking EVO as a specialist/possible fake Tiger threat without always casting a program—reasonable but not mandatory. Plan the engineer's location before paying for a 70–77pt TAG. |

### Disagreements to keep visible

- **Is the Jujak/Hwarang/Haetae/Dokkaebi Core mandatory?** It solves mobility, guns, hacking, defence and Guided exceptionally efficiently; *but* Shepherd's actual N5 battle report experiments with **Yě Māo+Yín-Shé** combinations and stresses avoiding homogeneous list construction. Use enemy Mimetism/MSV and mission needs to choose, not habit.
- **Blue Wolf versus Gūijiă:** Shepherd finds both useful-but-expensive; **Irregular Order 2026** sharply prefers Gūijiă (ARM8/MULTI HMG/Super-Jump/MA2 keeps it from entering enemy hacking/CC range) and calls Blue Wolf vulnerable at only Spitfire ranges. The counter-case is Blue Wolf's five-shot AP Spitfire and multi-weapon short-range fork, and unique Duo access.
- **Guìláng and Dàofěi costs:** **ITS Season 15 winner Axel** takes Guìláng LT/FO/Hacker for camo-based *mission board control*, despite knowing they're expensive; Shepherd finds Guìláng inefficient and Dàofěi 52pt too consuming except in Classified-heavy missions; BT Sherman strongly defends a mission-oriented Dàofěi LT/Specialist.
- **MSV versus Albedo plan:** Need direct MSV2 through smoke? Pay for **unlinked Rui Shi**. Expect opposing MSV AROs? Use **Yín-Shé Albedo(-6)** and/or Eclipse/Disco. Both do different jobs; neither universally supplants the other.
- **Hac Tao Hacker versus ordinary midfield piece:** 58pt Hidden Deployment Mimetism(-6) Trinity/ARM5 is hard to remove, but White Banner has **only that Hac Tao loadout**—no NCO HMG/ML—and cannot deploy it as cheaply or far forward as Guìláng/Dàofěi.
- **Lóng Yá and turrets:** Axel prizes cheap Lóng Yá and repeatedly fields them but questions spending multiple early orders on static turrets; other podcasters value layered AROs/recoverability. Avoid an architecture that collapses solely because deployment was lost.

### Source list and transcript status

| Source (ranked by specific practical value) | Transcript / useful focus |
|---|---|
| **[Robert Shepherd — N5 Faction Focus: White Banner](https://www.youtube.com/watch?v=-hB_mGBSuMY)** | **Full YouTube MCP transcript read**: faction strengths/weaknesses, detailed team math, Albedo + smoke, source-attributed **Dàofěi and Guìláng disagreements**, Blue Wolf/Gūijiă analysis, sample off-meta Yě Māo+Yín-Shé lists. Post-Oct-2025 N5 perspective. |
| **[Irregular Order Ep47 — White Banner Sectorial Guide](https://open.spotify.com/episode/2w4tX9v1goAozQSh7HqGUE)** (Aug 13, 2026) | **Full Podcast MCP transcript read**: most recent dedicated discussion found, Wildcards, Fireteam compositions, Jujak/Hwarang/Haetae core, Blue Wolf versus Gūijiă, Fēiquán VH, remote and starter-package evaluations. |
| **[WIP12 E183 — WhiteBanner with Axel](https://open.spotify.com/episode/5JPLqx5tJz0aduXl35WrYv)** (Apr 2025) | **Full Podcast MCP transcript read**: ITS S15 winner explains *why* he chooses unconventional two-list approaches, early board control, Guìláng LT, Kunai T2, two Lóng Yá, Liang Kai+Shaolin and Haetae Guided. Mission-specific N5 lists, not blanket must-takes. |
| **[Tactical Awareness S3 Ep21 — White Banner](https://open.spotify.com/episode/6kMFfOEsfoblAwlulWPEbd)** (May 2025) | **Full Podcast MCP transcript read**: independent list architectures, relative value of Jujak/Haetae/Dokkaebi, Shaolin, Guìláng, TAG versus HI and defensive REMs. Also [video version](https://www.youtube.com/watch?v=dk76kMCdxr8). |
| **[Infinity the Dante — White Banner Initial Reaction](https://www.youtube.com/watch?v=xHcogZAeg34)** (May 2025) | **Full YouTube MCP transcript read**; explains cheap pickets, complementary link Fireteams and limitations of MSV2 and long-range options. Archived earlier in [White Banner transcript](../../rules/Youtube%20factions/White%20Banner.txt). |
| **[Robert Shepherd — White Banner vs Corregidor: Yě Māo and Yín-Shé](https://www.youtube.com/watch?v=XQ58Ez86Vi8)** | **Full YouTube MCP transcript read**: on-table experiment with *two* Yě Māo/Yín-Shé pairs as an alternative to conventional Jujak-focused lists. |
| **[Loss of Lieutenant Ep142 — N5 TAG Tier List](https://open.spotify.com/episode/1h5CJfZC5zBPxdg66o7xIN)** (2025) | **Podcast MCP transcript read** for Gūijiă and related TAG tradeoffs against other factions; ranking is subjective and not a rules reference. |
| **[Robert Shepherd — N5 Vanilla Yu Jing](https://www.youtube.com/watch?v=mn4yHSNxsnA)** (Apr 2025) | **YouTube MCP previously reviewed** for shared Yu Jing TAGs/REMs; vanilla Fireteams and availability **must not** be copied into White Banner. |
| **[Corvus Belli community White Banner/Yu Jing N5 tactica index](https://forum.corvusbelli.com/threads/n5-recap-yu-jing-tacticas.43474/)** | Curated cross-check of video and podcast discovery; indexing ≠ transcript confirmation. |

**Refresh discipline:** Revalidate all tactical numbers against the pinned N5.3 table if Army/FAQ changes. Avoid propagating spoken transcription errors, prior-edition unit loadouts and apparently linkable FTO labels.

## Roster index

| Unit | ID | AVA | Type | Order | Fireteam access |
|---|---:|---:|---|---|---|
| Yáofáng Lóng Yá | 1537 | 2 | REM | Regular | — |
| Zhanshi Yīshēng | 137 | 1 | LI | Regular | Zhanshi; counts as Zhanshi |
| Tiger Soldiers | 126 | 3 | MI | Regular | — |
| Qíshì, StateEmpire TAG Support Pilots | 1838 | 1 | LI | Regular | Zhanshi |
| Beasthunters Free Guild | 1570 | 1 | SK | Irregular | Zhanshi, FTO profile only |
| Zhanshi | 124 | 5 | LI | Regular | Zhanshi |
| Hac Tao Special Unit | 131 | 1 | HI | Regular | — |
| Dokkaebi Cyberteam | 1756 | 1 | HI | Regular | White Banner |
| Shaolin Warrior Monks | 136 | 5 | WB | Irregular + Impetuous | Shaolin required-choice |
| Chaīyì Yáokòng | 142 | 2 | REM | Regular | — |
| Yáoxiè Lù Duān | 160 | 2 | REM | Regular | — |
| Blue Wolf Mongol Cavalry | 1495 | 2 | TAG | Regular + Tactical Awareness | Blue Wolf |
| Fēiquán Imperial Tactical Wing | 1842 | 1 | VH | Regular | — |
| Captain Qiang Gāo | 1498 | 1 | HI | Regular | Wildcard; counts as Shàng Jí |
| Hwarang Corps | 1752 | 2 | HI | Regular | White Banner; counts as Jujak |
| Sergeant So-ra Kwon | 1567 | 1 | HI | Regular | White Banner; counts as Jujak / Shàng Jí |
| Warcors | 50 | 1 | LI | Irregular | — |
| Jujak Regiment | 1494 | 4 | HI | Regular | White Banner required-choice; counts as Shàng Jí |
| Hùndùn Ambush Unit | 1492 | 3 | MI | Regular | — |
| Hùsòng Yáokòng | 140 | 3 | REM | Regular | — |
| Gūdǎn Troops | 1841 | 3 | LI | Regular | Zhanshi, FTO profiles only; counts as Zhanshi |
| Jing Qo | 1499 | 1 | MI | Regular | Wildcard; counts as Shaolin |
| Gŭiláng Skirmishers | 134 | 4 | SK | Regular | — |
| Tian Gǒu, Orbital Activity Squad | 1536 | 3 | LI | Regular | Wildcard, FTO profiles only |
| Yáozăo | 161 | 3 | REM | Peripheral | — |
| Gūijiă Squadrons | 133 | 1 | TAG | Regular + Tactical Awareness | — |
| Léi Gōng | 1497 | 1 | HI | Regular | Wildcard, FTO profiles only; counts as Shàng Jí |
| Chief Mech-Engineer Chung-Hee Jeong | 1539 | 1 | LI | Regular | Zhanshi; counts as Zhanshi |
| Bìxié | 1599 | 1 | HI | Regular | White Banner; counts as Shàng Jí |
| Johnny Kao | 1892 | 1 | MI | Regular | Wildcard |
| Son-Bae Yáokòng | 141 | 1 | REM | Regular | —; FTO-labelled option has no White Banner chart row |
| Naval Operations Group Sulyong | 1755 | 2 | MI | Regular | White Banner |
| Mech-Engineers (Zhanshi Gōngchéng) | 138 | 2 | LI | Regular | — |
| Yáopú Pangguling | 162 | 2 | REM | Regular | —; FTO-labelled option has no White Banner chart row |
| Liang Kai | 1500 | 1 | WB | Regular + Impetuous | Shaolin required-choice; counts as Shaolin |
| Silver Snakes, Yín-Shé Unit | 1840 | 3 | MI | Regular | White Banner required-choice; counts as Yě Māo |
| Dàofěi Tactical Section | 130 | 2 | HI | Regular | — |
| Imperial Agent Adil Mehmut (Crane Rank Armor) | 1540 | 1 | HI | Regular | Wildcard |
| Haetae Unit | 1754 | 1 | HI | Regular + Tactical Awareness | White Banner |
| Wèibīng Yáokòng | 139 | 2 | REM | Regular | — |
| Kunai Solutions Ninjas | 1502 | 1 | SK | Regular | — |
| Yě Māo Infantry | 1493 | 5 | MI | Regular | White Banner required-choice |
| Sulsa Warriors | 1753 | 1 | SK | Regular | — |
| Yáoxiè Rui Shi | 159 | 2 | REM | Regular | — |
| Oktavia Grímsdóttir | 1501 | 1 | LI | Regular | Zhanshi |
| Shàng Jí Invincibles | 150 | 5 | HI | Regular + Tactical Awareness | Zhanshi; White Banner required-choice; Blue Wolf |

Optional-mode units:

| Unit | ID | Mode | Fireteam relevance |
|---|---:|---|---|
| Guǐ Fēng Spec-Ops | 1914 | Spec-Ops | Zhanshi Fireteam row, max 1 when Spec-Ops mode is in use |
| Yu Jing Team-Ops | 1928 | Team-Ops | No ordinary White Banner Fireteam row |

## Unit details

### Yáofáng Lóng Yá

**ID 1537 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 12 | ARM 1 | BTS 3 | W 1 | S 3`. Remote Presence, Camouflage, Surprise Attack (-3), Courage, Forward Deployment (+10).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 16 | 0 | Panzerfaust (+1B), Flammenspeer (+1B), SMG, AP Mine, PARA CCW (-3) | — |
| 2 | 19 | 0 | Panzerfaust (+1B), Flammenspeer (+1B), Heavy Shotgun, AP Mine, PARA CCW (-3) | — |
| 3 | 17 | 0.5 | As Opt 1; Minelayer | — |

### Zhanshi Yīshēng

**ID 137 · AVA 1 · LI** — `MOV 10-10 | CC 15 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Doctor, MediKit.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 14 | 0 | Combi Rifle, Pistol, CCW | Zhanshi max 1; counts as Zhanshi |

### Tiger Soldiers

**ID 126 · AVA 3 · MI** — `MOV 10-10 | CC 17 | BS 13 | PH 12 | WIP 14 | ARM 2 | BTS 0 | W 1 | S 2`. Mimetism (-3), Parachutist, Combat Jump, Super-Jump, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 20 | 0 | Boarding Shotgun, D-Charges, Pistol, CCW | — |
| 4 | 29 | 1.5 | Spitfire, Pistol, CCW | — |
| 5 | 29 | 0.5 | Combi Rifle, Light Flamethrower, Pistol, CCW; Hacking Device, Hacker | — |
| 6 | 26 | 0 | Combi Rifle, Light Flamethrower, Pistol, CCW; MediKit, Paramedic | — |

### Qíshì, StateEmpire TAG Support Pilots

**ID 1838 · AVA 1 · LI** — `MOV 10-10 | CC 21 | BS 11 | PH 11 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 2`. Courage, Specialist Operative, Stealth, TAGCom.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 10 | 0 | **BLUE WOLF PILOT**; Light Shotgun, Pistol, Shock CCW (PS 7); GizmoKit, Terrain (Total) | Zhanshi max 1 |

### Beasthunters Free Guild

**ID 1570 · AVA 1 · SK** — `MOV 10-10 | CC 21 | BS 11 | PH 13 | WIP 12 | ARM 0 | BTS 0 | W 1 | S 2`. Mimetism (-3), Stealth, Super-Jump, Religious Troop, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 9 | 0 | **BEASTHUNTER FTO**; Heavy Flamethrower, Panzerfaust, AP Mine, Pistol, DA CCW | Zhanshi max 1 |
| 2 | 15 | 0 | Heavy Flamethrower, Tactical Bow, AP Mine, Pistol, DA CCW; Camouflage, Surprise Attack (-3), Forward Deployment (+20) | — |
| 3 | 15 | 0 | Heavy Flamethrower, Panzerfaust, AP Mine, Pistol, DA CCW; Camouflage, Surprise Attack (-3), Forward Deployment (+20) | — |
| 5 | 17 | 0 | Heavy Flamethrower, Panzerfaust, AP Mine, Pistol, EXP CCW (+1B); same camouflage package | — |

### Zhanshi

**ID 124 · AVA 5 · LI** — `MOV 10-10 | CC 15 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 10 | 0 | Combi Rifle, Pistol, CCW | Zhanshi 1–5 |
| 2 | 18 | 1 | HMG, Pistol, CCW | same |
| 4 | 16 | 1 | MULTI Sniper Rifle, Pistol, CCW | same |
| 5 | 15 | 1.5 | Missile Launcher, Pistol, CCW | same |
| 6 | 15 | 0.5 | Combi Rifle, Pistol, CCW; Hacking Device, Hacker | same |
| 8 | 11 | 0 | Combi Rifle, Flash Pulse, Pistol, CCW; Forward Observer | same |
| 9 | 12 | 0 | Combi Rifle, Pistol, CCW; MediKit, Paramedic | same |
| 10 | 10 | 0 | Combi Rifle, Pistol, CCW; Lieutenant | same |
| 11 | 12 | 0 | Combi Rifle, Pistol, CCW; Commlink (+1), Specialist Operative | same |

### Hac Tao Special Unit

**ID 131 · AVA 1 · HI** — `MOV 15-5 | CC 19 | BS 14 | PH 14 | WIP 14 | ARM 5 | BTS 6 | W 2 | S 2`. Camouflage, Hidden Deployment, Mimetism (-6), Surprise Attack (-3), Stealth.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 9 | 58 | 1 | MULTI Rifle, Nanopulser, Pistol, Shock CCW; Hacking Device with Trinity upgrade, Hacker | — |

### Dokkaebi Cyberteam

**ID 1756 · AVA 1 · HI** — `MOV 15-5 | CC 14 | BS 12 | PH 10 | WIP 13 | ARM 3 | BTS 6 | W 1 | S 2`. Structure, Remote Presence, Courage, No Wound Incapacitation.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 0.5 | Combi Rifle, Pitcher, MULTI Pistol (+1B), PARA CCW (-6); Hacking Device with Carbonite upgrade, Hacker | White Banner max 1 |
| 2 | 22 | 0 | Combi Rifle, Pitcher, MULTI Pistol (+1B), PARA CCW (-6), Cybermine; Killer Hacking Device with Spotlight upgrade, Hacker | same |
| 3 | 28 | 0.5 | Mk12, MULTI Pistol (+1B), PARA CCW (-6); Killer Hacking Device with Spotlight upgrade, Deployable Repeater, Marksmanship, Hacker | same |

### Shaolin Warrior Monks

**ID 136 · AVA 5 · WB** — `MOV 10-10 | CC 23 | BS 10 | PH 13 | WIP 14 | ARM 1 | BTS 0 | W 1 | S 2`. Martial Arts L3, Stealth, Religious Troop, Impetuous, No Cover.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 5 | 0 | Chain Rifle, Smoke Grenades, Pistol, Shock CCW | Shaolin required-choice, max 2 |
| 2 | 6 | 0 | Chain Rifle, Smoke Grenades, Pistol, DA CCW | same |
| 3 | 7 | 0 | Boarding Shotgun, Smoke Grenades, Pistol, Shock CCW | same |
| 6 | 10 | 0.5 | Combi Rifle, Smoke Grenade Launcher, Pistol, Shock CCW | same |

### Chaīyì Yáokòng

**ID 142 · AVA 2 · REM** — `MOV 15-15 | CC 13 | BS 8 | PH 11 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. 360º Visor, Remote Presence, Courage, Mimetism (-3).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 7 | 0 | Flash Pulse, PARA CCW (-3) | — |

### Yáoxiè Lù Duān

**ID 160 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 6 | W 1 | S 4`. Holoprojector, MSV1, Remote Presence, Courage, Surprise Attack (-3), BS Attack (+1B).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 24 | 0 | Mk12, Heavy Flamethrower, E/M Mine, PARA CCW (-3) | — |
| 2 | 20 | 0 | Thunderbolt, E/M Carbine, E/M Mine, PARA CCW (-3) | — |

### Blue Wolf Mongol Cavalry

**ID 1495 · AVA 2 · TAG** — `MOV 15-10 | CC 23 | BS 14 | PH 15 | WIP 13 | ARM 6 | BTS 6 | W 3 | S 6`. ECM: Guided (-6), Berserk, Courage, Tactical Awareness, Terrain (Total), BS Attack (+1B, SR-1).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 70 | 1.5 | AP Spitfire, Heavy Flamethrower, Panzerfaust, DA CCW; Regular + Tactical Awareness; includes Shàngdiào ancillary remote | Blue Wolf Duo, 1–2 |

### Fēiquán Imperial Tactical Wing

**ID 1842 · AVA 1 · VH** — `MOV 20-5 | CC — | BS 13 | PH 12 | WIP 13 | ARM 3 | BTS 3 | W 2 | S 7`. Aerial, Courage, Sensor, Super-Jump, No Cover, Tech-Recovery.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 28 | 0 | E/M Carbine (+1B), Flash Pulse, Akrylat-Kanone, Pitcher | — |
| 2 | 27 | 0 | MULTI Rifle (+1B), Akrylat-Kanone, Blitzen; X-Visor | — |

### Captain Qiang Gāo

**ID 1498 · AVA 1 · HI** — `MOV 15-5 | CC 17 | BS 13 | PH 12 | WIP 14 | ARM 5 | BTS 6 | W 2 | S 2`. TinBot: Firewall (-3), Warhorse.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 48 | 1.5 | HMG, Nanopulser, Breaker Pistol (+1B), CCW | Wildcard max 1; counts as Shàng Jí |
| 2 | 48 | 1 | Same; Lieutenant | same |

### Hwarang Corps

**ID 1752 · AVA 2 · HI** — `MOV 15-5 | CC 22 | BS 12 | PH 13 | WIP 13 | ARM 3 | BTS 3 | W 2 | S 2`. Albedo (-3), Martial Arts L3, Frenzy, Courage, Stealth, Combat Instinct.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 19 | 0 | Light Shotgun, Panzerfaust, Pistol, EXP CCW | White Banner max 2; counts as Jujak |
| 5 | 24 | 0 | Thunderbolt, Light Shotgun, Pistol, EXP CCW | same |
| 6 | 25 | 0 | Combi Rifle, Pistol, EXP CCW | same |
| 7 | 20 | 0 | Light Shotgun, Panzerfaust, Disco Baller, Pistol, EXP CCW; Deactivator | same |

### Sergeant So-ra Kwon

**ID 1567 · AVA 1 · HI** — `MOV 15-5 | CC 17 | BS 14 | PH 12 | WIP 13 | ARM 3 | BTS 3 | W 2 | S 2`. Courage, Minelayer, BS Attack (SR-1).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 32 | 0 | MULTI Marksman Rifle, Light Shotgun, E/M Mine, Breaker Pistol, CCW | White Banner max 1; counts as Jujak / Shàng Jí |
| 2 | 34 | 0 | Same; TinBot: Firewall (-6) | same |
| 3 | 31 | 0 | Combi Rifle (+1B), Heavy Flamethrower, E/M Mine, Breaker Pistol, CCW | same |
| 4 | 33 | 0 | Same; TinBot: Firewall (-6) | same |

### Warcors

**ID 50 · AVA 1 · LI** — `MOV 10-10 | CC 11 | BS 9 | PH 11 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Journalist.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CCW (-3); 360º Visor | — |
| 2 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CCW (-3); Sixth Sense | — |

### Jujak Regiment

**ID 1494 · AVA 4 · HI** — `MOV 15-5 | CC 16 | BS 13 | PH 12 | WIP 13 | ARM 3 | BTS 3 | W 2 | S 2`. Courage.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 25 | 0 | Combi Rifle, Heavy Flamethrower, Pistol, CCW | White Banner required-choice, max 4; counts as Shàng Jí |
| 2 | 26 | 0 | Breaker Combi Rifle, Heavy Flamethrower, Pistol, CCW | same |
| 3 | 28 | 0 | Breaker Combi Rifle, Heavy Flamethrower, Pistol, CCW; TinBot: Firewall (-6) | same |
| 4 | 29 | 1.5 | Missile Launcher, Light Flamethrower, Pistol, CCW | same |
| 5 | 31 | 1.5 | Spitfire, Heavy Flamethrower, Pistol, CCW | same |
| 7 | 27 | 0 | Vulkan Shotgun, Panzerfaust, Pistol, CCW; TinBot: Firewall (-6) | same |
| 8 | 29 | 0 | Vulkan Shotgun, Panzerfaust, D-Charges, Pistol, CCW; Engineer, Deactivator, GizmoKit | same |
| 9 | 25 | 0 | Combi Rifle, Heavy Flamethrower, Pistol, CCW; Lieutenant | same |

### Hùndùn Ambush Unit

**ID 1492 · AVA 3 · MI** — `MOV 10-10 | CC 15 | BS 13 | PH 11 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`. Camouflage, Hidden Deployment, Mimetism (-3), Surprise Attack (-3), Stealth.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 31 | 0.5 | MULTI Marksman Rifle, Pistol, CCW; MSV1 | — |
| 2 | 29 | 1.5 | MULTI Sniper Rifle, Pistol, CCW | — |
| 3 | 22 | 1.5 | Heavy Rocket Launcher, Pistol, CCW; X-Visor | — |

### Hùsòng Yáokòng

**ID 140 · AVA 3 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. 360º Visor, Remote Presence, Courage, Total Reaction.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 1 | HMG, PARA CCW (-3) | — |
| 2 | 18 | 0 | Thunderbolt (+1B), PARA CCW (-3) | — |

### Gūdǎn Troops

**ID 1841 · AVA 3 · LI** — `MOV 10-10 | CC 15 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Warhorse, Terrain (Mountain).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 11 | 0 | **GŪDǍN FTO**; Light Shotgun, Heavy Flamethrower, Pistol, CCW | Zhanshi max 2; counts as Zhanshi |
| 2 | 11 | 0 | **GŪDǍN FTO**; SMG, Zapper, Pistol, CCW | same |
| 3 | 13 | 0 | Light Shotgun, Heavy Flamethrower, Shock Mine, Pistol, CCW; Camouflage (1 Use), Forward Deployment (+10) | — |
| 4 | 12 | 0 | SMG, Zapper, Shock Mine, Pistol, CCW; Camouflage (1 Use), Forward Deployment (+10) | — |

### Jing Qo

**ID 1499 · AVA 1 · MI** — `MOV 15-5 | CC 23 | BS 13 | PH 12 | WIP 14 | ARM 3 | BTS 3 | W 1 | S 2`. Bangbomb (+4), Martial Arts L3, Berserk, FT Master (Shaolin), Mimetism (-3), No Wound Incapacitation, Stealth, Climbing Plus.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 32 | 0 | MULTI Rifle, Boarding Pistol, AP+DA CCW | Wildcard max 1; counts as Shaolin |

### Gŭiláng Skirmishers

**ID 134 · AVA 4 · SK** — `MOV 10-10 | CC 15 | BS 11 | PH 12 | WIP 14 | ARM 1 | BTS 0 | W 1 | S 2`. MSV1, Camouflage, Mimetism (-3), Surprise Attack (-3), Infiltration, Stealth, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 23 | 0 | Boarding Shotgun, Shock Mine, D-Charges, Pistol, CCW | — |
| 3 | 28 | 1.5 | MULTI Sniper Rifle, Shock Mine, D-Charges, Pistol, CCW | — |
| 4 | 31 | 0.5 | Combi Rifle, Shock Mine, D-Charges, Pistol, CCW; Hacking Device, Hacker | — |
| 5 | 25 | 0.5 | Boarding Shotgun, Shock Mine, D-Charges, Pistol, CCW; Deployable Repeater, Minelayer | — |
| 6 | 27 | 0 | Combi Rifle, Flash Pulse, Shock Mine, D-Charges, Pistol, CCW; Forward Observer | — |
| 7 | 23 | 1 | Boarding Shotgun, Shock Mine, D-Charges, Pistol, CCW; Lieutenant | — |

### Tian Gǒu, Orbital Activity Squad

**ID 1536 · AVA 3 · LI** — `MOV 10-10 | CC 16 | BS 12 | PH 10 | WIP 14 | ARM 2 | BTS 3 | W 1 | S 2`. 360º Visor, Warhorse, Terrain (Zero-G).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 22 | 0 | **TIAN GǑU FTO**; Combi Rifle, Jammer, Boarding Pistol, CCW; Holomask | Wildcard max 1 |
| 3 | 20 | 0 | **TIAN GǑU FTO**; Boarding Shotgun, Grenades, Jammer, Boarding Pistol, CCW; Holomask | same |
| 4 | 24 | 0 | **TIAN GǑU FTO**; Thunderbolt, E/M Carbine, Boarding Pistol, CCW; Holomask, BS Attack (+1B) | same |
| 6 | 22 | 0 | **TIAN GǑU FTO**; Combi Rifle, Boarding Pistol, CCW; Killer Hacking Device, Hacker | same |
| 8 | 26 | 0 | Thunderbolt, E/M Carbine, Boarding Pistol, CCW; Holoprojector + Holomask, BS Attack (+1B), Surprise Attack (-3) | — |
| 9 | 27 | 0 | Combi Rifle, MadTraps, Boarding Pistol, CCW; Killer Hacking Device, Holoprojector, Minelayer, Surprise Attack (-3), Hacker | — |

### Yáozăo

**ID 161 · AVA 3 · REM** — `MOV 15-10 | CC 11 | BS 8 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 1`. Peripheral (Servant), Courage, Mimetism (-3).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 3 | 0 | PARA CCW (-3); no Order, support Peripheral | — |

### Gūijiă Squadrons

**ID 133 · AVA 1 · TAG** — `MOV 15-10 | CC 22 | BS 14 | PH 16 | WIP 13 | ARM 8 | BTS 6 | W 3 | S 7`. ECM: Guided (-6), Martial Arts L2, Courage, Tactical Awareness, Super-Jump.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 77 | 1.5 | MULTI HMG, Heavy Flamethrower, DA CCW; Regular + Tactical Awareness; includes Shàngdiào ancillary remote | — |
| 2 | 77 | 2 | Same; Lieutenant | — |

### Léi Gōng

**ID 1497 · AVA 1 · HI** — `MOV 15-5 | CC 18 | BS 13 | PH 12 | WIP 14 | ARM 3 | BTS 6 | W 1 | S 2`. Albedo (-6), MSV1, Courage, No Wound Incapacitation, Super-Jump.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 32 | 0 | AP SMG, E/Mitter, Zapper, Breaker Pistol, CCW; Parachutist | — |
| 2 | 34 | 0 | **LÉI GŌNG FTO**; MULTI Marksman Rifle, Zapper, Blitzen, Breaker Pistol, CCW | Wildcard max 1; counts as Shàng Jí |
| 4 | 29 | 0 | **LÉI GŌNG FTO**; AP SMG, E/Mitter, Zapper, Breaker Pistol, CCW | same |
| 5 | 34 | 0 | **LÉI GŌNG FTO**; same AP-SMG package; Chain of Command | same |

### Chief Mech-Engineer Chung-Hee Jeong

**ID 1539 · AVA 1 · LI** — `MOV 10-10 | CC 17 | BS 12 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`. Engineer, Deactivator, GizmoKit, Repeater.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 31 | 0 | AP Combi Rifle, E/Mitter, D-Charges, Armed Turret (AP Marksman Rifle), Pistol, CCW | Zhanshi max 1; counts as Zhanshi |
| 2 | 27 | 0 | K1 Combi Rifle, D-Charges, AP Mine, Pistol, CCW | same |

### Bìxié

**ID 1599 · AVA 1 · HI** — `MOV 15-5 | CC 22 | BS 13 | PH 12 | WIP 13 | ARM 3 | BTS 6 | W 2 | S 2`. MSV1, Martial Arts L3, Courage, Forward Observer, Stealth, NCO, Super-Jump, Climbing Plus.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 41 | 0 | MULTI Rifle, Zapper, Flash Pulse, Pistol, E/M CCW | White Banner max 1; counts as Shàng Jí |

### Johnny Kao, Optimate and Technomancer Master

**ID 1892 · AVA 1 · MI** — `MOV 15-5 | CC 18 | BS 13 | PH 12 | WIP 14 | ARM 3 | BTS 6 | W 2 | S 2`. Engineer, Mimetism (-3), Deactivator, GizmoKit, X-Visor, Non-Hackable.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 36 | 0 | Plasma Carbine, Zapper, Monofilament Mine, D-Charges, MULTI Pistol, CCW | Wildcard max 1 |
| 2 | 40 | 0 | MULTI Rifle, Zapper, Drop Bears, D-Charges, MULTI Pistol, CCW | same |
| 3 | 42 | 0 | MULTI Rifle, Zapper, Monofilament Mine, D-Charges, Armed Turret (Plasma Carbine), MULTI Pistol, CCW | same |

### Son-Bae Yáokòng

**ID 141 · AVA 1 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Remote Presence, Courage.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 16 | 1.5 | Missile Launcher, PARA CCW (-3); Guided | — |
| 2 | 19 | 1.5 | **SON-BAE FTO**; Missile Launcher (+1B), PARA CCW (-3) | —; no White Banner chart row |

### Naval Operations Group Sulyong

**ID 1755 · AVA 2 · MI** — `MOV 10-10 | CC 17 | BS 12 | PH 11 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`. MSV1, NCO, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 24 | 0 | MULTI Marksman Rifle, Pistol, CCW | White Banner max 2 |
| 2 | 25 | 1 | Red Fury, Pistol, CCW | same |
| 3 | 22 | 0 | Light Shotgun (+1B), Thunderbolt, Flash Pulse, D-Charges, Pistol, CCW; Forward Observer | same |
| 4 | 21 | 0 | SMG, E/Mitter, Pistol, CCW; MediKit, Paramedic | same |

### Mech-Engineers (Zhanshi Gōngchéng)

**ID 138 · AVA 2 · LI** — `MOV 10-10 | CC 15 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Engineer, Deactivator, GizmoKit.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 14 | 0 | Combi Rifle, D-Charges, Pistol, CCW | — |
| 2 | 15 | 0 | Same; Deployable Cover | — |
| 3 | 17 | 0 | Combi Rifle, Armed Turret (Combi Rifle), Pistol, CCW | — |

### Yáopú Pangguling

**ID 162 · AVA 2 · REM** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 4`. Baggage, Remote Presence, Courage.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 8 | 0 | PARA CCW (-3); Deactivator, Repeater | — |
| 2 | 14 | 0.5 | PARA CCW (-3); EVO Hacking Device, Hacker | — |
| 3 | 17 | 0 | Combi Rifle, PARA CCW (-3); Repeater, Total Reaction | — |
| 4 | 12 | 0 | **PANGGULING FTO**; Light Shotgun, PARA CCW (-3); Repeater | —; no White Banner chart row |

### Liang Kai

**ID 1500 · AVA 1 · WB** — `MOV 10-10 | CC 23 | BS 11 | PH 13 | WIP 14 | ARM 1 | BTS 0 | W 1 | S 2`. Martial Arts L4, Berserk, Mimetism (-3), No Wound Incapacitation, Stealth, Super-Jump, Climbing Plus, Impetuous, FT Master (Shaolin).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 21 | 0 | Chain Rifle, Light Shotgun, Flash Pulse, Pistol, EXP CCW; Regular + Impetuous | Shaolin required-choice, max 1; counts as Shaolin |

### Silver Snakes, Yín-Shé Unit

**ID 1840 · AVA 3 · MI** — `MOV 10-10 | CC 17 | BS 13 | PH 11 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`. Albedo (-6), Courage, Stealth, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 22 | 0 | Combi Rifle, E/M Carbine, Panzerfaust, Boarding Pistol, CCW | White Banner required-choice, max 3; counts as Yě Māo |
| 2 | 26 | 0 | K1 Marksman Rifle, E/M Carbine, AP Mine, Boarding Pistol, CCW | same |
| 3 | 26 | 0 | MULTI Marksman Rifle, E/M Carbine, AP Mine, Boarding Pistol, CCW | same |
| 4 | 22 | 0 | Boarding Shotgun, E/Mitter, D-Charges, Boarding Pistol, CCW; BS Attack (+1B), Specialist Operative | same |
| 5 | 24 | 0.5 | Boarding Shotgun, E/Mitter, AP Mine, Boarding Pistol, CCW; BS Attack (+1B), Forward Deployment (+10), Minelayer | same |
| 7 | 27 | 0.5 | K1 Sniper Rifle, E/Mitter, Boarding Pistol, CCW; Marksmanship | same |

### Dàofěi Tactical Section

**ID 130 · AVA 2 · HI** — `MOV 15-5 | CC 19 | BS 13 | PH 14 | WIP 13 | ARM 4 | BTS 3 | W 2 | S 2`. Camouflage, Mimetism (-3), Surprise Attack (-3), Infiltration, Stealth, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 4 | 52 | 1.5 | AP Spitfire, D-Charges, Kobra Pistol, CCW; Specialist Operative | — |
| 5 | 52 | 0.5 | MULTI Rifle, D-Charges, Kobra Pistol, CCW; Hacking Device, Hacker | — |
| 7 | 52 | 1.5 | AP Spitfire package; Lieutenant, Specialist Operative | — |
| 8 | 52 | 0.5 | MULTI Rifle hacker package; Lieutenant | — |

### Imperial Agent Adil Mehmut (Crane Rank Armor)

**ID 1540 · AVA 1 · HI** — `MOV 15-5 | CC 23 | BS 13 | PH 13 | WIP 13 | ARM 4 | BTS 6 | W 2 | S 2`. Martial Arts L3, Courage, Warhorse, Sensor, Stealth, Specialist Operative, X-Visor, Deactivator.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 49 | 1.5 | AP Spitfire, Nanopulser, Disco Baller, Heavy Pistol, Monofilament CCW, PARA CCW (-6) | Wildcard max 1 |
| 2 | 49 | 1.5 | Same; Lieutenant | same |

### Haetae Unit

**ID 1754 · AVA 1 · HI** — `MOV 10-10 | CC 15 | BS 14 | PH 12 | WIP 12 | ARM 5 | BTS 6 | W 2 | S 5`. Tactical Awareness, Religious Troop, Warhorse.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 40 | 1.5 | AP HMG, Assault Pistol, PARA CCW (-6); Regular + Tactical Awareness | White Banner max 1 |
| 2 | 36 | 1.5 | Heavy Rocket Launcher (+1B), Assault Pistol, PARA CCW (-6); Guided; Regular + Tactical Awareness | same |

### Wèibīng Yáokòng

**ID 139 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Deactivator, Repeater, Remote Presence, Courage, Triangulated Fire, Forward Observer, Sensor.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 14 | 0 | Combi Rifle, Flash Pulse, PARA CCW (-3) | — |
| 2 | 17 | 0 | Same; Tactical Awareness; Regular + Tactical Awareness | — |

### Kunai Solutions Ninjas

**ID 1502 · AVA 1 · SK** — `MOV 10-10 | CC 21 | BS 12 | PH 12 | WIP 12 | ARM 1 | BTS 0 | W 1 | S 2`. Martial Arts L3, Camouflage, Hidden Deployment, Mimetism (-6), Surprise Attack (-3), Stealth, Climbing Plus, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 28 | 1.5 | MULTI Sniper Rifle, Pistol, Shock CCW | — |
| 2 | 26 | 0 | Shock Marksman Rifle, Pistol, Shock CCW; BS Attack (AP) | — |
| 3 | 25 | 0.5 | Thunderbolt, PARA Mine, Pistol, Shock CCW; BS Attack (T2) | — |

### Yě Māo Infantry

**ID 1493 · AVA 5 · MI** — `MOV 10-10 | CC 15 | BS 13 | PH 11 | WIP 13 | ARM 2 | BTS 6 | W 1 | S 2`. MSV1, Bangbomb (+4), Mimetism (-3), Super-Jump, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 0 | MULTI Rifle, Panzerfaust, Boarding Pistol, CCW | White Banner required-choice, max 3 |
| 2 | 28 | 1.5 | AP Spitfire, Boarding Pistol, CCW | same |
| 3 | 26 | 1.5 | Missile Launcher, Boarding Pistol, CCW | same |
| 4 | 27 | 0.5 | MULTI Rifle, Boarding Pistol, CCW; Hacking Device, Hacker | same |
| 5 | 25 | 0 | MULTI Rifle, Boarding Pistol, CCW; Killer Hacking Device, Hacker | same |
| 6 | 27 | 0 | MULTI Rifle, Panzerfaust, D-Charges, Boarding Pistol, CCW; Engineer, Deactivator, GizmoKit | same |
| 7 | 24 | 0 | MULTI Rifle, Panzerfaust, Flash Pulse, Boarding Pistol, CCW; Forward Observer | same |

### Sulsa Warriors

**ID 1753 · AVA 1 · SK** — `MOV 10-10 | CC 23 | BS 11 | PH 12 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Martial Arts L3, Camouflage (1 Use), Infiltration, Mimetism (-6), Stealth, Berserk, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 28 | 0 | Boarding Shotgun, Shock Mine, Pistol, DA CCW | — |
| 3 | 31 | 0 | SMG, Pistol, DA CCW; Killer Hacking Device, Hacker | — |
| 4 | 29 | 0 | SMG, Shock Mine, Pistol, DA CCW; Deployable Repeater, Minelayer | — |
| 5 | 29 | 0 | SMG, Shock Mine, Flash Pulse, Pistol, DA CCW; Forward Observer | — |

### Yáoxiè Rui Shi

**ID 159 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 6 | W 1 | S 4`. Repeater, Remote Presence, Courage.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 1 | Spitfire, PARA CCW (-3); MSV2 | — |
| 2 | 21 | 0.5 | Red Fury, Mine Dispenser, PARA CCW (-3); MSV1 | — |

### Oktavia Grímsdóttir

**ID 1501 · AVA 1 · LI** — `MOV 10-10 | CC 17 | BS 12 | PH 10 | WIP 13 | ARM 2 | BTS 0 | W 1 | S 2`. Albedo (-3), BS Attack (+1B), Courage, Combat Instinct, Dogged.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 30 | 1.5 | Missile Launcher, Contender, Heavy Pistol, CCW | Zhanshi max 1 |
| 2 | 26 | 1.5 | Heavy Rocket Launcher, Contender, Heavy Pistol, CCW; Sixth Sense | same |

### Shàng Jí Invincibles

**ID 150 · AVA 5 · HI** — `MOV 15-5 | CC 19 | BS 13 | PH 14 | WIP 13 | ARM 4 | BTS 6 | W 2 | S 2`. Tactical Awareness, Number 2, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 37 | 0 | MULTI Rifle, Boarding Pistol, AP CCW; TinBot: Firewall (-6); Regular + Tactical Awareness | Zhanshi max 2; White Banner required-choice max 5; Blue Wolf max 1 |
| 7 | 40 | 0.5 | MULTI Rifle, Flash Pulse, D-Charges, Boarding Pistol, AP CCW; Hacking Device, Hacker; Regular + Tactical Awareness | same |
| 10 | 36 | 0 | MULTI Rifle, Flash Pulse, Boarding Pistol, AP CCW; Forward Observer; Regular + Tactical Awareness | same |
| 11 | 45 | 1.5 | AP HMG, Boarding Pistol, AP CCW; TinBot: Firewall (-6); Regular + Tactical Awareness | same |
| 13 | 34 | 1.5 | Heavy Rocket Launcher, Light Shotgun, Boarding Pistol, AP CCW; Regular + Tactical Awareness | same |
| 16 | 45 | 1 | AP HMG, Boarding Pistol, AP CCW; TinBot: Firewall (-6), Lieutenant; Regular + Tactical Awareness | same |

## Canonical Fireteam chart

Fireteam limits in the pinned source: **Core 1; Haris 1; Duo unlimited** (`DUO: 256` sentinel).

### Zhanshi Fireteams

**Types:** Core, Haris

| Entry | Min | Max | Required-choice | Counts as / note |
|---|---:|---:|---|---|
| ZHANSHI | 1 | 5 | no | — |
| GŪDǍN FTO | 0 | 2 | no | Zhanshi |
| SHÀNG JÍ | 0 | 2 | no | — |
| Zhanshi YĪSHĒNG | 0 | 1 | no | Zhanshi |
| CHIEF JEONG | 0 | 1 | no | Zhanshi |
| QÍSHÌ | 0 | 1 | no | — |
| BEASTHUNTER FTO | 0 | 1 | no | — |
| OKTAVIA | 0 | 1 | no | — |
| GUǏ FĒNG | 0 | 1 | no | Spec-Ops mode only |

### White Banner Fireteams

**Types:** Core, Haris, Duo

| Entry | Min | Max | Required-choice | Counts as / note |
|---|---:|---:|---|---|
| SHÀNG JÍ | 0 | 5 | yes | — |
| JUJAK | 0 | 4 | yes | Shàng Jí |
| YĚ MĀO | 0 | 3 | yes | — |
| YÍN-SHÉ | 0 | 3 | yes | Yě Māo |
| SULYONG | 0 | 2 | no | — |
| HWARANG | 0 | 2 | no | Jujak |
| HAETAE | 0 | 1 | no | — |
| DOKKAEBI | 0 | 1 | no | — |
| SO-RA KWON | 0 | 1 | no | Jujak, Shàng Jí |
| BÌXIÉ | 0 | 1 | no | Shàng Jí |

The four `required-choice` rows are a required-choice set from the Army chart; they are not interpreted here as requiring one of every row simultaneously.

### Blue Wolf Fireteams

**Types:** Duo

| Entry | Min | Max | Required-choice | Counts as / note |
|---|---:|---:|---|---|
| BLUE WOLF | 1 | 2 | no | — |
| SHÀNG JÍ | 0 | 1 | no | — |

### Shaolin Fireteams

**Types:** Haris, Duo

| Entry | Min | Max | Required-choice | Counts as / note |
|---|---:|---:|---|---|
| SHAOLIN | 0 | 2 | yes | — |
| LIANG KAI | 0 | 1 | yes | Shaolin |

The two `required-choice` rows form the Shaolin required-choice set.

### Wildcards

| Entry | Max | Counts as / profile restriction |
|---|---:|---|
| TIAN GǑU FTO | 1 | FTO profiles only |
| LÉI GŌNG | 1 | FTO profiles only; Shàng Jí |
| JING QO | 1 | Shaolin |
| QIANG GĀO | 1 | Shàng Jí |
| ADIL CRANE RANK | 1 | — |
| JOHNNY KAO | 1 | — |

Wildcards use the global Wildcard row of the White Banner chart and may join otherwise eligible White Banner Fireteams, subject to the chart and the profile restrictions above.

## Reverse Fireteam access index

| Unit / profile | Fireteam access | Counts as / restriction |
|---|---|---|
| Beasthunter FTO | Zhanshi | FTO profile only |
| Bìxié | White Banner | Shàng Jí |
| Blue Wolf | Blue Wolf | 1–2 Blue Wolves required by row minimum |
| Chief Jeong | Zhanshi | Zhanshi |
| Dokkaebi | White Banner | — |
| Gūdǎn FTO | Zhanshi | FTO profiles only; Zhanshi |
| Guǐ Fēng Spec-Ops | Zhanshi | Optional Spec-Ops mode only |
| Haetae | White Banner | — |
| Hwarang | White Banner | Jujak |
| Jing Qo | Wildcard | Shaolin |
| Jujak | White Banner | Required-choice; Shàng Jí |
| Liang Kai | Shaolin | Required-choice; Shaolin |
| Léi Gōng FTO | Wildcard | FTO profiles only; Shàng Jí |
| Oktavia | Zhanshi | — |
| Qiang Gāo | Wildcard | Shàng Jí |
| Qíshì | Zhanshi | — |
| Sergeant So-ra Kwon | White Banner | Jujak, Shàng Jí |
| Shaolin | Shaolin | Required-choice |
| Shàng Jí | Zhanshi; White Banner; Blue Wolf | White Banner required-choice |
| Sulyong | White Banner | — |
| Tian Gǒu FTO | Wildcard | FTO profiles only |
| Yě Māo | White Banner | Required-choice |
| Yín-Shé | White Banner | Required-choice; Yě Māo |
| Zhanshi | Zhanshi | Native 1–5 row |
| Zhanshi Yīshēng | Zhanshi | Zhanshi |
| Adil Mehmut (Crane Rank) | Wildcard | — |
| Johnny Kao | Wildcard | — |

All standard roster units not listed in this reverse index have no Fireteam access in the pinned White Banner chart.

## TAG tactical cross-reference (2026-10-23)

**Blue Wolf** supports direct attack/CC deterrence and legal White Banner Fireteams, while **Gūijiă** is the more straightforward sustained heavy gun. Pick Blue Wolf when movement/pressure/close angles matter, Gūijiă for conventional ranged trading. Check the actual Fireteam-required member/profile; neither TAG automatically gains the other's access.

Across all factions, compare **apex power** separately from **points value**, counterplay and mission fit: [N5.3 TAG guide](../../notes/list-building/tags.md). The current unit profiles and canonical Fireteam chart above take precedence over tactical opinions.

## Vehicle (VH) tactical cross-reference (2026-10-23)

**Fēiquán AVA1:** **28/0 Pitcher/E/M/Sensor** creates high-angle hacking access; **27/0 X-Visor MULTI Rifle** buys modest ranged damage instead. **Irregular Order #47 (Aug 2026)** argues that White Banner already has useful ground Repeaters, making Pitcher less essential here than in **Imperial Service**, where it opens the network. Use only if the hacker payoff or Sensor matters; both versions are very vulnerable at S7/ARM3/No Cover.

See [VH apex/value tier list and matchup guide](../../notes/list-building/vehicles-vh.md). **This sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative.**
