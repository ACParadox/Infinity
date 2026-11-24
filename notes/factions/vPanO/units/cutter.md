# Cutters, Varuna Naval Chasseurs — Vanilla PanOceania (Infinity N5.3)

**Sources:** [Pinned vanilla roster](../../../../sectorials/panoceania/panoceania.md) · [Source sectorial roster](../../../../sectorials/panoceania/varuna-immediate-reaction-division.md) · [Source unit analysis](../../Varuna/units/cutter.md) · [Vanilla listbuilding](../vanilla-pano-listbuilding.md) · [Fireteams](../vanilla-pano-fireteams.md). Adapted 24 November 2026.

## Vanilla differences

- **AVA:** 2 in Varuna → 1 in vanilla.
- **Option IDs and prices (pts/SWC):** same listed numeric option IDs and prices as source roster. Printed-roster comparison, not a new raw Army skill audit.
- **Fireteams (24 November 2026 corrected chart):** Not listed in either corrected vanilla chart; remains independent.

## Pinned vanilla profiles

**ID 12 · AVA 1 · TAG** — `MOV 15-10 | CC 18 | BS 15 | PH 15 | WIP 12 | ARM 8 | BTS 6 | W 3 | S 7`. ECM: Guided (-6), Camouflage, Hidden Deployment, Surprise Attack (-3), Mimetism (-6), Remote Presence, Courage, Dodge (PH=11), GizmoKit (PH=13), Terrain (Aquatic), BS Attack (SR-1).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 97 | 2 | MULTI HMG, CCW (PS=5); NCO; Crabbot |
| 2 | 95 | 2.5 | MULTI HMG, CCW (PS=5); Lieutenant; Crabbot |

## Vanilla selection and use

**A+ NCO97/2; B− LT95/2.5, usually avoid.** NCO Cutter97 + Magistrate Strategos LT19 = 116/2, vs Cutter LT95 + Magistrate CoC21 = 116/2.5: equal points, half SWC saved, flexible Strategos and separate command. Alternatively double Fusilier20 + Cutter97 = 117/2, two backfield Regular Orders and one LT Order for the Cutter; with a dedicated NCO this is preferred when troop slots permit. Cutter lacks TA; do not count an LT Order twice or assume Cutter generates a pooled Order while in Hidden Deployment.

**S+ raw conventional apex / A+ overall listbuilding value.** 97/2 MULTI HMG NCO is preferred; 95/2.5 LT sacrifices NCO and exposes command. BS15, Mim-6, Camouflage, Hidden Deployment, ARM8 and three STR deliver the highest conventional gun ceiling; no printed TA. Swiss56, Tik69 and Squalos66 leave more room for scoring. Cutter +31 points over Squalos equals an entire Nisse HMG; Bolt MSR/KHD + Karhu Feuerbach/Engineer (two FT2 Duos) costs 107/3, only 10 more than Cutter, with four Regular bodies and two specialists but less concentrated resilience. Choose deliberately.

## Original Varuna analysis — retained reference copy

The original is retained for transferable mechanics and reasoning. Sectorial ratings, profiles, AVA and linked packages are historical source-context only. The vanilla profile and notes above take precedence. Links retain original destinations.

### Cutter — Varuna Immediate Reaction Division (Infinity N5.3)

**Verdict: S+ tier apex conventional gunfighter, A-tier value. Must-own, not must-field. Prefer the 97-point NCO profile.** The Cutter is an exceptional primary ranged attack engine combining BS15, Mimetism (-6), MULTI HMG, repeatable Camouflage, Hidden Deployment and ARM8. Take it when the mission or matchup wants an apex TAG, not merely because Varuna historically equals Cutter. The 70-point Uhlan remains the better general army-building asset in a hypothetical cross-sectorial comparison.

**Authority:** [Pinned Varuna roster](../../../../sectorials/panoceania/varuna-immediate-reaction-division.md#cutters-varuna-naval-chasseurs) · [Listbuilding](../../Varuna/varuna-listbuilding.md) · [Fireteams](../../Varuna/varuna-fireteams.md) · [References](../../Varuna/varuna-references.md) · [NCA Uhlan analysis](../../NCA/units/uhlan.md) · [Weapon chart](https://infinitythewiki.com/Weapons_Chart). Reviewed 24 November 2026; tactical ratings are judgments. Cutter shared skills and option Orders checked against the [exact pinned Army JSON](https://github.com/massayoshi/infinity-army-backup/blob/6b79f39a3abbf5cd3d837fb9dc65e411fc35244b/n5/varuna-immediate-reaction-division/7.26246.158.json).

#### Profiles

AVA2, Regular TAG, MOV 6-4", CC18, BS15, PH15, WIP12, ARM8, BTS6, STR3, S7. Camouflage, Hidden Deployment, Surprise Attack (-3), Mimetism (-6), Remote Presence, Courage, ECM: Guided (-6), Terrain (Aquatic), BS Attack (SR-1), Dodge (PH=11), GizmoKit (PH=13). Both options carry MULTI HMG, CC Weapon (PS=5) and Crabbot. No Tactical Awareness, Warhorse or Fireteam access.

| Opt | Pts/SWC | Difference | Rating |
|---:|---:|---|---|
| 1 | **97/2** | NCO | **S+** |
| 2 | 95/2.5 | Lieutenant | A |

NCO reallocates an existing Lieutenant Order; it does not generate an extra Order. The LT version generates one ordinary Lieutenant Order, not an LT (+1 Order) bonus. Varuna has no Chain of Command profile in the pinned roster.

#### Gunfighting and weapon

| Mode | Active B | ARO B | Ammo | Effective PS (SR-1) |
|---|---:|---:|---|---:|
| MULTI HMG burst | 4 | 1 | AP or Shock | 4 |
| MULTI HMG anti-materiel | 1 | 1 | EXP | 4 |

BS Attack (SR-1) penalizes Saving Rolls rather than Face-to-Face Rolls; effective PS is shorthand for that calculation. AP provides sustained anti-ARM fire, Shock helps against eligible infantry, and EXP offers a powerful B1 reactive threat. There is no secondary ranged gun, disposable E/M, pistol, direct template or mine. The Cutter can use Suppressive Fire, but not simultaneously with Camouflaged State.

##### Illustrative asymmetric engagements

Conventional BS14 HMG opponent without MSV or other special MODs, both in Partial Cover, active TAG opening from Camouflage. Surprise Attack is active-turn only.

| Range | Cutter active | Enemy vs Cutter | Uhlan active | Enemy vs Uhlan |
|---|---|---|---|---|
| 16–32" | B4 on 15 | B1 on 5 | B3 on 15 | B1 on 8 |
| 32–48" | B4 on 9 | B1 on 2 | B3 on 12 | B1 on 2 |

At 32–48", the Cutter's opponent would nominally suffer -15 total MOD but the [rules cap total MOD at -12](../../../../rules/1_Basic%20Rules/Rolls.md), leaving BS2 rather than an impossible roll. The Feuerbach retains a neutral range MOD where an HMG is at -3. After Surprise Attack is spent, the enemy's numbers in the 16–32" band become 8 against Cutter and 11 against Uhlan. MSV, Combat Instinct, Sixth Sense and other conditions can alter these examples. These are target numbers, not complete probabilities.

The Cutter is strongest at conventional ranged engagements, especially against opponents without MSV. ARM8 (normally effective ARM11 in Partial Cover against unmodified ARM saves), three STR and Remote Presence make a lost Face-to-Face less likely to end its attack run. Against MSV2 the Mimetism advantage over Uhlan disappears; range, Burst, ammunition and resilience still matter.

#### Hidden Deployment and repeatable Camouflage

Three distinct defensive layers:

- **Avoidance:** Hidden Deployment and repeatable Camouflage. The opponent cannot see the initial hidden position and must plan around uncertainty. Sensor and other explicit counters remain relevant.
- **Evasion:** Mimetism (-6), which persists after the Cutter reveals.
- **Resilience:** ARM8, STR3, Remote Presence and Engineer repair.

Hidden Deployment is particularly attractive when going second; the Cutter can wait until its active turn or reveal into a favorable legal ARO. It does not gain Surprise Attack in ARO. Hidden Deployment cannot be regained. While hidden at Order counting, its Regular Order is not added to the pool, but is retained for the Cutter's own active-turn reveal under the [Hidden Deployment rules](../../../../rules/8_Game%20States%20and%20Glossary/Hidden_Deployment_State.md). An ordinary Camouflage deployment is also a valid choice when shared Order flexibility is more important.

**Attack–retreat–re-camouflage** is the defining repeated cycle: use the opening Surprise Attack, win the key engagements, reserve movement and an Order to return to Camouflaged State outside enemy LoF and relevant Sensor restrictions, and restore Surprise Attack eligibility next turn. Do not leave the TAG exposed just because its ARO is strong. Suppressive Fire is an alternative end state when the position and range justify it. Neither Camouflage nor Hidden Deployment makes the TAG universally immune to indirect threats.

#### Vulnerabilities

- **Hacking / E/M:** Mimetism and ECM: Guided (-6) do not defend against ordinary Comms Attacks. BTS6 helps but Isolation, Immobilization and Possession are serious threats. No Warhorse or native Firewall. Clear enemy repeaters or their supporting hackers and retain a repair route.
- **Close assault:** no pistol, template, mines or special melee defenses. CC18 and a PS5 CC Weapon are not enough against dedicated CC specialists. Avoid tight midfield areas and screen approach routes with other troops.
- **Mobility:** 6-4" is good but S7 needs space; no Climbing Plus and no broad Terrain (Total). It cannot go Prone or use Cautious Movement as a TAG. Plan retreat routes.
- **Order economy and opportunity cost:** roughly one-third of a 300-point army before support, no Tactical Awareness or Fireteam, and few spare points for redundancy and distributed objectives. Every failed attack run matters more.

The Cutter is a long-range hunter, not a self-contained midfield assault TAG. The Crabbot may help with eligible mission tasks but cannot replace several mobile specialists.

#### Cross-sectorial comparison — Uhlan, Tikbalang and Squalos

Sources: [Uhlan analysis](../../NCA/units/uhlan.md) · [Kestrel Tikbalang](../../kestrel/units/Tikbalang.md) · [Varuna Squalos](../../Varuna/units/squalos-mk-ii.md). Uhlan and Tikbalang are cross-sectorial benchmarks, not legal Varuna options.

| Capability | Cutter NCO | Uhlan Feuerbach | Kestrel Tikbalang | Squalos NCO |
|---|---|---|---|---|
| Pts/SWC | 97/2 | **70/1.5** | 69/1.5 | 66/1.5 |
| BS / ARM / BTS / STR | 15/8/6/3 | 15/6/6/3 | 15/6/6/3 | 15/6/6/3 |
| CC / WIP / S | 18/12/7 | 15/12/6 | 17/13/6 | 18/13/6 |
| Main gun | B4 MULTI HMG | B3 AP+DA Feuerbach | B4 HMG | B4 MULTI HMG |
| Effective main PS (SR-1) | 4 | 5 | 4 | 4 |
| Mimetism | -6 | -3 | -3 | — |
| Camouflage / Surprise Attack | Yes / -3 | Yes / -3 | — | — |
| Hidden Deployment | Yes | — | — | — |
| Tactical Awareness | — | Yes | Yes | Yes |
| NCO | Yes | — | — | Yes |
| Warhorse | — | Yes | — | — |
| Secondary ranged weapons | None | Panzerfaust, Blitzen, MULTI Pistol | HFT, Shock Mine | MULTI Pistol (+1B) |
| Suppressive Fire | Yes | — | Yes | Yes |
| Climbing Plus | — | — | Yes | — |
| Fireteam | None | None | ARMORED Duo | Cavalry Duo |

##### Cutter versus Uhlan — detailed comparison

Both share BS15, 6-4" MOV, BTS6, three STR, SR-1, repeatable Camouflage, Surprise Attack (-3), Remote Presence and guided ECM. They solve similar ranged engagements but at very different army costs.

| Weapon characteristic | Cutter | Uhlan Feuerbach |
|---|---|---|
| Active sustained mode | B4 AP or Shock | B3 AP+DA |
| ARO primary modes | B1 AP or EXP | B1 AP+DA or EXP |
| Effective primary PS | 4 | 5 |
| 16–32" | +3 | +3 |
| 32–48" | -3 | 0 |
| Secondary anti-heavy | None | Panzerfaust AP+EXP, Blitzen E/M |
| Close-range firearm | None | MULTI Pistol |
| CC weapon | PS5 | AP |

- **Cutter:** the superior conventional gunfighter. Extra Burst, Mimetism (-6), ARM8, Hidden Deployment and Suppressive Fire are real advantages. It performs especially well against ordinary infantry and attackers without MSV.
- **Uhlan:** the superior value and more versatile long-range hunter. AP+DA forces two saves against half ARM per ordinary hit; excellent anti-armour lethality, though exact outcomes depend on Face-to-Face odds and target saves. B1 ARO preserves the full ammunition effect. Panzerfaust/Blitzen add AP+EXP and E/M options; their active B2 consumes both standard disposable uses in one attack. MULTI Pistol provides an emergency close-range weapon.
- **Warhorse:** Uhlan resists Isolation, including Oblivion and the Isolated component of E/M, but is not immune to Immobilization, Possession or other hacking. This is important on an expensive TAG. S6 also makes terrain geometry easier.
- **Orders:** Uhlan generates a Tactical Awareness Order; Cutter uses an existing LT Order through NCO. Hidden Deployment can restrict the Cutter's first Regular Order to its own reveal instead of the pool. Both can re-camouflage.
- **Opportunity cost:** 27 points and 0.5 SWC saved by Uhlan. An NCA Blade-Ops Engineer (23/0, Tactical Awareness) plus Uhlan costs 93/1.5, with two Regular and two Tactical Awareness Orders when eligible. This is an independent support pair, not a Fireteam; their Tactical Orders are personal. An unsupported Cutter costs 97/2.

| Role | Cutter | Uhlan | Tikbalang | Squalos |
|---|---|---|---|---|
| Conventional gunfighting | S+ | A+ | A+ | A |
| Opening attack | S+ | S | A | A |
| Anti-armour lethality | S | S+ | B | A |
| Reactive deterrence | S | S | A | A |
| Weapon versatility | B | S+ | A | A |
| Raw durability | S+ | A | A | A |
| Defensive concealment | S+ | S | C | C |
| Overall survivability | S+ | S | A | B+ |
| Hacking resistance | B | A- | B | B |
| Mobility | A | A | S+ | A |
| Close-range defense | C | B- | S | B+ |
| Order economy | A | S | S | S+ |
| Value | A | S+ | S | A+ |

**If both were available in one sectorial, prefer the Uhlan for most lists.** The Cutter is worth its premium when absolute conventional gunfighting dominance, ARM8 and initial deployment uncertainty are central to the strategy. The Uhlan is the better general army-building asset.

##### Cutter versus Squalos — actual Varuna choice

- **Cutter NCO 97/2:** one premium independent attacker; superior asymmetric gunfighting, concealment and armour.
- **Squalos MULTI HMG NCO 66/1.5 + Kamau Paramedic Tactical Awareness 25/0:** 91/1.5, two Regular and two generated Tactical Awareness Orders, access to the LT Order, a specialist and a legal Cavalry Duo. The Kamau is a one-Wound infantry piece, not a second TAG. Personal Tactical Orders must be used by the eligible leader, not transferred to make the Squalos shoot. Neither unit requires remaining linked for every turn.

Prefer Cutter for killing-oriented missions when it must solve difficult gunfights. Prefer Squalos for broader objective and specialist requirements, better Order generation and greater list flexibility. Do not buy a second premium gun simply because there are points available.

#### Lieutenant architecture

| Package | Pts/SWC | Assessment |
|---|---|---|
| Cutter NCO + Fusilier LT + Fusilier decoy | **117/2** | Preferred default |
| Cutter NCO + Zulu-Cobra LT | 120/2 | Alternative if Camouflage and Sensor/Jammer utility matter |
| Cutter LT | 95/2.5 | Generally skip; deliberately all-in |

Two Fusiliers provide a cheap passive LT and decoy, plus two Regular Orders. The Zulu-Cobra LT costs 23/0; its Jammer/Sensor role can conflict with keeping the LT safe. With NCO there is no need to expose the LT to make productive use of its Order. Cutter LT saves only two points versus Cutter NCO in isolation and increases SWC by 0.5; it saves more by eliminating the separate LT package but also loses its bodies and Orders and concentrates command risk. Varuna has no CoC safety net.

#### Support and listbuilding

| Unit | Pts/SWC | Function |
|---|---|---|
| Machinist + Palbot | 20/0 | Repair, recovery of applicable states; keep a legal approach |
| Tech-Bee | 9/0 | TAGCom, specialist and Repeater; same Combat Group |
| Helot Camo SMG/LRL | 12/0 | Cheap reactive friction and approach screening; Irregular |
| Zulu-Cobra Sensor/Jammer | 23/0 | Midfield control, detection and approach denial |
| Zulu-Cobra KHD | 26/0 | Counter-hacking, Pitcher |
| Kamau MSV2 Sniper | 29/1.5 | Complementary MSV coverage |
| Kamau Hacker | 22/0.5 | Hacking network / control |

Tech-Bee TAGCom improves the Cutter's Dodge (PH=11) to 14 and GizmoKit (PH=13) to 14 while eligible in the same Combat Group. She is not an Engineer. The Cutter cannot borrow a Fireteam's TinBot through a nonexistent link; use Repeater control, counter-hacking, positioning and other legal protection instead. An EVO Fairy Dust package is optional where the mission and hacking meta warrant it.

##### Example starting shell (not a complete army)

| Piece | Pts/SWC |
|---|---|
| Cutter NCO | 97/2 |
| Fusilier LT + decoy | 20/0 |
| Machinist + Palbot | 20/0 |
| Tech-Bee | 9/0 |
| Zulu-Cobra Sensor/Jammer | 23/0 |
| Helot Camo SMG/LRL | 12/0 |
| **Subtotal** | **181/2** |
| **Remaining in 300/6** | **119/4** |

Use the remaining budget for Regular Orders, mobile specialists, counter-hacking and a qualitatively different secondary attack vector. Avoid an oversized reactive castle or multiple redundant expensive gunfighters. For broad classified packets, consider dropping the Cutter altogether for Croc Men, Echo-Bravo, Kamau specialists or Montesa.

**Final assessment:** S+ primary gunfighter and ranged counterattack, S+ survivability, S reactive deterrence, B midfield assault, C independent scoring, A Order economy and A value. One of the strongest reasons to play Varuna, but TAG Varuna remains a deliberate archetype rather than the faction default.
