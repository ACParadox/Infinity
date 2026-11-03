# Guided Missile Strategy — Network, Spotlight, Tempo and Counterplay (N5.3)

**Scope:** Practical Infinity N5.3 play, **not** a ranking of missile REMs, Hackers, Pitchers or sectorials. The separate [Indirect Fire — Speculative Attack and Spotlight → Guided apex/value guide](../list-building/indirect-fire-speculative-guided-apex-value.md) evaluates purchases and loadouts; [Hacking and Network Projection](hacking-and-network-projection.md), [Speculative Fire](speculative-fire.md), [Target Priority and Attack Sequencing](target-priority-and-attack-sequencing.md) and [Mission Scoring](mission-scoring-and-specialist-strategy.md) cover adjacent topics.

**Evidence method (2 Nov 2026):** Current [N5.3 wiki](https://infinitythewiki.com/Guided), [Spotlight](https://infinitythewiki.com/Spotlight), [Targeted](https://infinitythewiki.com/Targeted_State), [Reset](https://infinitythewiki.com/Reset), [Forward Observer](https://infinitythewiki.com/Forward_Observer) and [Firewall](https://infinitythewiki.com/Firewall) govern rules. The repository's [241 numbered battle-report entries](../battle-reports/n5-battle-reports-and-tournament-reports.md) and [cross-report findings](../battle-reports/n5-what-works-what-fails-when.md) provide **qualitative** examples; selected [original YouTube reports](#8-source-notes--original-transcripts-and-evidence-grades) and [Spotify podcast transcripts](#8-source-notes--original-transcripts-and-evidence-grades) were checked. A report played under N5/N5.1/N5.2 is evidence for *decision making*, not authority for N5.3 odds, unit profiles, Fireteams, or mission scoring. Do not convert reported outcomes into matchup win rates.

> **Core principle:** Guided is a **scalpel, an area-denial threat, and an alternative to bad gunfights**. It is not automatically the best place to spend every remaining Order. The strongest missile system can win without firing by making an opponent spend Orders avoiding Repeaters, Resetting or taking a worse route. [#021](../battle-reports/021-030-n5-battle-report-tactical-analysis.md) is a player assessment of this deterrent value; [#118](../battle-reports/111-120-n5-battle-report-tactical-analysis.md) and [Loss of Lieutenant E155](https://open.spotify.com/episode/3bC5DmFnk3eFiNlZhBZBA3) show successful selective removal.

## Rules floor — check before attempting the sequence

| N5.3 rule | What changes on the table |
|---|---|
| **Spotlight** | A **Short Skill / ARO** and **Comms Attack** with **B2 in the Active Turn**. Successful WIP hits require **PS 5 AP Saving Rolls against halved BTS**; **a failed Saving Roll**, not merely a winning WIP Roll, gives **Targeted**. It can affect **non-Hackable** troops in Hacking Area. Targets can oppose with **Reset**. |
| **Forward Observer (FO)** | A **LoF-dependent WIP-based BS Attack**, printed **B2**, applying **Targeted directly on a successful attack** without a subsequent BTS Saving Roll. It has different range/visibility/ARO risks from Spotlight; it is not the same as a speculative or hacking attack. |
| **Targeted** | Grants **+3** to BS Attack, Comms Attack and Discover against the target; imposes **-3 WIP on its Reset** and disallows its Stealth/Cautious Movement. It remains until legally cancelled, rather than vanishing automatically at turn end. |
| **BS Attack (Guided)** | Requires **the actual BS Attack (Guided) skill** and a **Targeted enemy**. Active Turn only, **no LoF needed**, generally **B1**, **up to five Guided attacks per Active Turn**; the correct **Blast / Impact Template (Circular)** mode is required, not a freely chosen AP+EXP Hit Mode. It remains a **BS Attack Short Skill**, allowing a legal Move + BS Attack (Guided) combination. |
| **Range and geometry** | Measure **straight-line distance launcher-to-target** for the weapon's printed **Range MOD and maximum range**. A possible trajectory must exist: do not attack a target in an enclosed room. **No universal +6 Guided bonus.** Ignore negative Cover/Mimetism/visibility MODs except effects that specifically apply to Guided. The **Targeted +3** and weapon Range MOD still matter. |
| **Guided defence** | The target can **Dodge or Reset in Face to Face**. Without LoF to the attacker, Dodge normally suffers **-3**. A Targeted model's Reset normally suffers **-3**, but a **successful Reset also removes Targeted**; a successful Dodge avoids that shot **without clearing Targeted**. |
| **ECM / Firewall** | **ECM (Guided -X)** penalizes the Guided BS Attack; **ECM (Hacking -X)** penalizes applicable hacking; these are different protections. **Firewall (-3/-6)** penalizes relevant Comms Attacks and adds **+3 to the defender's Saving Roll**; **only one Firewall source applies**. Firewall does **not** protect against the subsequent missile BS Attack. |
| **Profiles** | **An FTO/+1B Missile Launcher is not automatically Guided.** Verify the exact N5.3 profile, BS, SWC, weapon mode, range, and Fireteam eligibility. A launcher being present in the list does not establish a valid Guided attack. |

Sources: [Guided/BS Attack](https://infinitythewiki.com/Guided), [Spotlight](https://infinitythewiki.com/Spotlight), [Targeted State](https://infinitythewiki.com/Targeted_State), [Reset](https://infinitythewiki.com/Reset), [FO](https://infinitythewiki.com/Forward_Observer), [ECM](https://infinitythewiki.com/ECM), [Firewall](https://infinitythewiki.com/Firewall), [Repeater](https://infinitythewiki.com/Repeater); corresponding local rules are under [rules/](../../rules).

## 1. Building and deploying a Guided Missile network

### Build a functioning chain, not three unrelated purchases

A robust package has **four jobs**, each of which should still contribute if the missile never fires:

1. **Access / projection:** a deployed native Repeater, Minelayer + Deployable Repeater, mobile Repeater, FastPanda, Pitcher carrier, or forward FO. Starting with coverage at Turn 0 is worth Orders and removes a dice-dependent setup step. Check legal Hacking Area, target position, range and enemy interference.
2. **Target acquisition:** at least one protected **Spotlight Hacker**; ideally a second legal marking path (another Hacker or **FO**) so assassination or a single lost Repeater does not shut the plan down. Prioritize good WIP, safe activation, suitable programs and anti-KHD protection over raw hacker count.
3. **Payload:** an actual **Guided** launcher whose firing position has legal range and trajectory to *likely* targets. Conceal it against flanking, airborne, and counterbattery play. Do not park it so far back that targets are outside range or forced into the weapon's poor band.
4. **Conversion:** normal gunfighters, specialist runners, smoke/White Noise, an Engineer, and **Orders reserved for objectives**. If Targeted improves an ordinary gun attack or the Repeater can Oblivion a blocker, the missile is an option, not a compulsory endpoint.

**Deployment rehearsal before choosing to go first/second:**

- Draw each relevant **8-inch ZoC / Repeater coverage area** and the opponent's plausible infiltration/Pitcher landing positions; do not assume an apparent wall protects a Hacker from an enemy Repeater around that corner.
- Deploy **cheap first-contact nodes** forward, valuable Hackers **behind** expendable screens with physical protection, and the launcher in a concealed but range-relevant position. Place a backup Hacker or FO in a *different* failure area where possible.
- Keep the **Pitcher, Hacker and launcher able to spend the Orders they need in their respective Combat Groups**. A second-group Guided bot with no available Regular Orders is not an offensive plan; adjust groups/Command Tokens legally rather than silently spending group-one Orders.
- Count how many Orders remain **after** specialist activations, movement, rebuilding a downed node, and a failed Pitcher shot. Decide the maximum acceptable missile investment before the turn begins.
- Deploy the army to survive **going second**: the attacker can arrive by a different path, remove the forward node, or kill a single vulnerable Hacker before your first active Order.

**Networks are not one-way invulnerability.** Friendly Repeaters extend friendly Hackers, but enemy hackers can exploit some repeater interactions against your Hackers; attacking through an enemy Repeater incurs Firewall penalties. Check the exact legal interaction, and never put all your Hackers where one enemy Pitcher can expose them simultaneously. **Loss of Lieutenant E176 (55:55–65:00)** discusses role-first Hacker deployment, cheap backfield Hackers, forward coverage, and the risk of reverse hacking through Repeaters: [YouTube](https://www.youtube.com/watch?v=UoYjrRvC5ic&t=3355s) / [Spotify](https://open.spotify.com/episode/109wmskmaxqFierHIG89kN).

**What not to buy exclusively for Guided:** a large suite of expensive Pitcher carriers that do little else; a Hacker that cannot project Hacking Area; a missile REM that needs to leave its safe position just to reach range; or an overfull cyber package that leaves too few scoring models. [Loss of Lieutenant E161 — Pitcher Tierlist](https://open.spotify.com/episode/1ZxuI8ZQ1zHJZ9aRPxYKft) repeatedly highlights the **Pitcher roll → Spotlight roll/Saving Roll → Guided roll/defence** chain as a meaningful source of wasted Orders.

## 2. Order-by-order execution: Repeater → Spotlight → Guided

### Standard offensive sequence

| Stage | Active player decision | Opponent's best plausible response | Go/no-go check |
|---|---|---|---|
| **0 — Identify the payoff** | Name a target whose removal or suppression opens a mission route: exposed Engineer, gun/ARO anchoring a lane, important Specialist, fragile Lieutenant/support, or a link member whose loss breaks useful support. | May reposition, hide, use alternate scoring bodies. | **Is this better than shooting, hacking to IMM/Isolated, or ignoring it?** |
| **1 — Project** | Use **already-live** Repeater coverage if possible; else fire a legal Pitcher, place a FastPanda/Deployable Repeater, or deliver a sacrificial mobile node. May instead use an FO to bypass the hacker setup entirely. | Shoot the carrier/node, oppose Pitcher placement where legal, threaten the Hacker through the network. | **How many Orders and Disposable charges remain if placement fails?** |
| **2 — Mark** | Activate a Hacker to **Spotlight** through valid Hacking Area, or FO with LoF; check WIP/Firewall/Reset, then **all Spotlight Saving Rolls**. Confirm Targeted *actually applied*. | Reset, engage Hacker, defend with Firewall/high BTS, move out of network on a later opportunity. | **If no Targeted: retry, switch to Oblivion/Carbonite, or stop?** |
| **3 — Fire** | Activate a verified **Guided** unit, select mandatory Blast/Circular mode and target; check **range, trajectory, ECM (Guided), five-attack cap**, legal AROs and template placement. | **Reset** to contest and potentially clear Targeted, or **Dodge** to avoid this shot, perhaps protect clustered models. | **Does the launcher now have favorable practical odds relative to other attacks?** |
| **4 — Reassess immediately** | After every Guided shot, check wounds, state, group Orders, remaining Guided cap and the mission clock. Move Specialists / clear a lane with a normal gun if that now yields more OP. | Successful **Reset** can require *re-marking* before the next missile. Successful **Dodge** leaves Targeted in place, so a further shot may remain available. | **Do not auto-queue a second or third missile.** |
| **5 — Convert** | Use the cleared corridor for a console, HVT, zone, cargo delivery, or safe attack into exposed support. Protect the marking route for the next turn only if the future value justifies it. | May sacrifice another defender, counter-pitch, counter-kill your Hacker, or abandon the route. | **Is there still time to score?** |

**Worked turn shape (illustrative, not a guarantee):** Turn 1 starts with one native midfield Repeater already covering an ARO defender. The Hacker spends **one or more Orders** seeking a real Targeted result. The launcher spends **one or more Orders** on Guided, respecting the cap and reacting to Reset. If the defender is disabled, a gunfighter uses the newly safe lane and a Specialist takes an objective. If the first Targeted attempt fails, **the turn can switch immediately to direct-fire/smoke/objective play**. A successful shot but successful Armor saves is not a justification to chase the target through your scoring reserve.

**Reactive-turn setup:** a Repeater/FO can make Targeted possible in **ARO**, allowing a follow-up Guided shot on *your* next Active Turn. The attacker may instead use another Hacker program in ARO; avoid automatically selecting Spotlight if Oblivion or Carbonite would stop a critical HI/TAG push now. Marking cheap non-Hackable bodies can still be valuable, but their mere existence in range does not make firing a missile worthwhile.

**Alternate FO line:** FO → Targeted → Guided skips the Pitcher/Hacker Orders, is not hindered by Firewall/BTS, and is often attractive with an infiltrated or objective-useful FO. But it requires **LoF** and a favorable WIP BS Attack after range/visibility/cover MODs, with serious exposure to opposing shooting/ARO. [Loss of Lieutenant E155](https://open.spotify.com/episode/3bC5DmFnk3eFiNlZhBZBA3) describes holding a Guided option behind midfield FOs and a possible late airborne Spotlight source rather than assuming a Pitcher is mandatory.

### Why Fireteam and combat-group sequencing matters

- An enemy Fireteam or clump invites **Circular-template collateral**, but do not invent free hits or treat every member's response as identical; resolve legal AROs, template reach and terrain separately.
- A **linked Pitcher +SD / X-Visor** may establish the node efficiently; that does *not* make an FTO missile version Guided. Team-leader choice, possible Fireteam changes, and which group funds the Hacker/launcher matter.
- **A Guided BS Attack is a Short Skill**, not Speculative Attack's Long Skill. A legal **Move + Guided** can adjust range or preserve cover, while active Guided remains **B1** and is capped. The original [#229 game](https://www.youtube.com/watch?v=843sIPoFsko) contains discussion correcting the mistaken “Guided is a Long Skill” assumption; current rules, not table talk, are authoritative.

## 3. Target selection and expected Order efficiency

### Select by *mission leverage per Order*, not by enemy points alone

| Target situation | Guided priority | Why / immediate follow-through |
|---|---|---|
| **Single ARO gun blocking the only scoring lane, behind Total Cover from your normal attacker** | **High**, if safely markable | Remove the exact blocker, then **use the lane**. Do not spend three more Orders killing nearby irrelevant bodies. |
| **Engineer, Doctor, TinBot/Firewall provider, isolated scoring Specialist, or key command piece** | **High**, when reachable and fragile enough | Destroy one enabling component, deny repair/mission access, then attack the main threat or score. |
| **Concentrated Fireteam with exposed edge / several legal template victims** | **High conditional** | Potential splash and forced defensive decisions. **Spread targets and check template geometry**; remember the first Targeted Saving Roll and subsequent FTF can both fail. |
| **Difficult Mimetism / suppressive defender that conventional shooting cannot efficiently remove** | **High conditional** | Guided ignores most ordinary visual/Cover penalties and may let you avoid a terrible Face to Face gunfight. |
| **Target already Targeted from a reactive Spotlight/FO** | **Often high** | The expensive **setup is already paid**. Recalculate launcher Range MOD, ECM, Dodge/Reset and number of wounds needed. |
| **TAG with high Wounds/ARM, ECM: Guided, and Engineer backup** | **Often low** for repeated missile spam | One B1 attack can require several high-variance attempts, while Reset can wipe Targeted. Consider Oblivion, E/M, AP guns, or scoring instead. |
| **Expendable 5–10pt warband in a safe but irrelevant location** | **Usually low** | Spotlight/Guided may cost more Orders than the model's useful contribution. Exception: it holds a critical switch/zone or its removal unlocks a winning turn. |
| **Enemy safely behind an enclosed room, out of weapon range, or not in legal Hacking Area/LoF for marking** | **Not legal as proposed** | Change firing position/network or abandon Guided for a different tool. |

**Mission clock overrides target value.** [#122 Tunguska–Neoterra](../battle-reports/121-130-n5-battle-report-tactical-analysis.md) reports very heavy Guided damage and Retreat, yet a narrow objective-point victory depended on an early **button press**. [#005 Kestrel–Combined](../battle-reports/001-010-n5-battle-report-tactical-analysis.md) includes a *player critique* that more Guided attacks distracted from consolidating control; this is not proof that a specific unplayed alternative would have won.

### Order-efficiency model (planning tool, not a claim about game-wide hit rates)

For a *fresh* missile kill plan, write these distinct probabilities from actual profile/position and likely AROs:

- **P(node)**: chance a Pitcher or other contested delivery succeeds per Order; count Move/Place Deployable Orders as well.
- **P(mark)**: chance one Spotlight/FO Order **actually produces Targeted**. Spotlight requires an attack success *and a failed AP/PS5 BTS Saving Roll*; a WIP hit alone is not enough.
- **P(payoff)**: chance one Guided Order produces the **specific desired effect** (wound, Unconscious, link break, etc.) after FTF defence and appropriate ARM Saves. This is *not* the same as launcher hit chance.
- **Cost of losing Targeted**: if the defender **successfully Resets** against Guided, the setup must be revisited; a successful Dodge avoids the attack but leaves Targeted.
- **Opportunity cost**: the direct-fire/smoke/FO route and the number of Orders needed to score after a kill.

A deliberately **optimistic lower-bound** estimate *if the Repeater stays in place and Targeted persists until the payoff* is:

- **Expected Orders to establish node and mark** ≈ **1/P(node) + 1/P(mark)**.
- **Expected additional firing Orders for one payoff** ≈ **1/P(payoff)**.
- **Illustration only:** with hypothetical **P(node)=0.80**, **P(mark)=0.50**, **P(payoff)=0.30**, the rough total is **1.25 + 2.00 + 3.33 = 6.58 Orders** before movement, re-marking, contested placement, differing Combat Groups or actual scoring. These are **not** claimed N5.3 profile probabilities. If a native Repeater is already established, remove the **1.25** setup term; if the target is already Targeted, remove both setup terms. If Resets repeatedly cancel Targeted, real expected cost becomes **higher**, and simple addition no longer models the sequence accurately.

Use the model as a **stop rule**, not to predict exact dice. Before firing, ask: *Will this target produce at least as much mission value as spending roughly 3–7 Orders positioning a Specialist or solving the lane another way?* There is no universal threshold: an Objective Point or eliminating the last delivery Specialist can be worth more than several enemy wounds.

**Fast turn decision tree:**

1. **Already Targeted and legal high-impact missile?** Consider **one Guided attack**, then reassess.
2. **Not Targeted but cheap, robust marking route?** Mark only if the resulting target matters to the mission or to several future attacks.
3. **Spotlight failed twice / defender high BTS+Firewall / ECM: Guided / required range poor?** Consider **switching targets or tools**, not feeding the whole group into the plan.
4. **Defender out of position or forced to Reset while your gunfighter has a safe route?** Attack/score **without needing the missile**.
5. **No Orders left after the hypothetical kill to claim an objective?** Stop or radically narrow the missile attempt.

## 4. Dealing with Reset, Dodge, ECM, Firewall and enemy Hackers

### Offensive adjustments, one defence at a time

| Defence | What it actually threatens | Better offensive answer |
|---|---|---|
| **Reset vs Spotlight** | WIP Face to Face can defeat marking; successful hacking rolls still need the Spotlight Saving Roll. | Improve Hacking Area/position, attack a more vulnerable source, threaten with a conventional gun from another angle, or use a legal FO. Avoid re-rolling into an expensive high-BTS Firewall target indefinitely. |
| **Reset vs Guided** | On a win, avoids the shot **and cancels Targeted**, forcing another marking cycle. | Prefer targets with poor effective WIP, one-shot mission-leverage kills, or **use the threat to force Reset while a gunfighter/scorer gains ground**. Re-mark only when mission value justifies it. |
| **Dodge vs Guided** | Face to Face can avoid the attack; no-LoF Dodge normally **-3**, but high PH/Dodge bonuses may still make it preferable. A successful Dodge **does not remove Targeted**. | Recalculate whether another missile is worth the Order; use Dodge movement/position changes to improve an ordinary attack or score. Do not assume the defender must Reset. |
| **ECM (Guided -6), bad launcher range** | Lowers the **Guided BS Attack** chance even after a successful Spotlight. | Mark for **ordinary gun +3**, choose another target, change launcher location/range, or pivot to E/M, Oblivion, FO or mission play. Avoid treating ECM: Hacking as ECM: Guided. |
| **Firewall / high BTS during Spotlight** | Penalizes **Comms Attack** and improves its Saving Roll; a Targeted token is less likely to appear. | Use FO, a target outside the protected bubble, another program/angle, or a direct shooter; do not assume two Spotlight hits equal Targeted. **Only one Firewall** applies. |
| **Enemy KHD/Trinity and counter-Pitchers** | Can kill or force your only Hacker away, making every Repeater a dead investment. | Separate and protect Hackers, retain KHD/Trinity protection where legal, remove hostile projected Repeaters, keep secondary marker/FO, and avoid revealing the whole package to one enemy node. |
| **Anti-projector shooting, stealthy bypass, dispersed troops** | Destroys network edges, avoids the trigger geometry, reduces valuable template overlaps. | Reposition a mobile node or use an alternative lane only if the Order budget makes sense; otherwise make them score under conventional AROs. |

**A critical distinction:** **Hacking/Spotlight and Guided are different attacks with different defences.** A TinBot Firewall may frustrate Spotlight but does not automatically apply to the missile. A TAG's **ECM (Guided -6)** may make missiles poor but does not, by itself, stop a conventional weapon. A target choosing **Dodge** versus **Reset** is choosing between surviving *this* shot and also potentially clearing future exposure.

**The package is a fork, not necessarily a damage loop.** Put an enemy where moving triggers possible hacking, standing still allows your attacker to advance, and approaching the Repeater exposes them to an ARO gun. [Loss of Lieutenant E166 — The Art of the Fork](https://open.spotify.com/episode/4AWYvbMuuQAeAYlaA26ghh) examines Mine/Koala + Hacker decisions: **Dodge** answers physical attacks, **Reset** answers Comms Attacks. Such mixed threats can matter more than repeatedly attempting a specific Spotlight + Guided kill. This does not mean a single model can evade every separate attack with one chosen ARO.

## 5. Coordinate Guided threats with conventional gunfighters

### Three practical combinations

**A. Guided opens a lane; gunfighter and Specialist cash it in.**

- Identify *one* long-range ARO/linked gun covering the button.
- Mark through a safe projected network; fire **Guided only if its expected cost is lower than exposing the attacker**.
- Advance the shooter after defender removal, threaten the next ARO from a new angle, then spend remaining Orders to **press the button or occupy the zone**.
- **Evidence:** [#118 Morats–WinterFor, Unmasking](../battle-reports/111-120-n5-battle-report-tactical-analysis.md): narrator projects linked Dartok Pitchers, then uses spare **Combat Group 2** Orders to Spotlight/Guided-remove a Varangian-like protected threat while **Rodoks** work mission objectives; in the [original video](https://www.youtube.com/watch?v=bvNTyBHsGXM), the narrator explicitly describes Guided as an optional 16-point tool and acknowledges a direct Thunderbolt Rodok shot could also have been viable. **Do not reinterpret the case as missiles winning by themselves.**

**B. Repeater threatens control; normal gun capitalizes on Reset / position.**

- Put a Repeater so a Hackable elite attacker's advance risks **Oblivion / Carbonite / Spotlight**, while an HMG/sniper watches the *useful* physical lane.
- If the defender makes safe moves or Resets to protect itself, use the time and new position to advance a second threat. If the hacking net has already isolated/immobilized the attacker, **a Guided shot may be unnecessary**.
- **Evidence:** [#003 Kestrel–White Banner](../battle-reports/001-010-n5-battle-report-tactical-analysis.md) shows the inverse: clearing the **hostile Pitcher** first let Kestrel's normal attackers move, flank and score. That is a reminder to defend the *physical route* opened by the network, not simply the missile model.

**C. Guided is the scalpel; off-axis assault punishes remaining support.**

- Mark an enemy **Doctor/Engineer, suppression piece, mission Specialist or link support** rather than the most expensive TAG by reflex.
- Use a missile for the hard-to-reach priority model, while **airborne, Camo, smoke/MSV or a regular gun** handles the accessible second target. Do not make both routes depend on one exposed Hacker.
- **Evidence:** In [Loss of Lieutenant E155 — Burn City Brawl 2025 winner interview](https://open.spotify.com/episode/3bC5DmFnk3eFiNlZhBZBA3), the Tunguska winner discusses **Spotlight + Guided into TAK Veteran Kazaks/Frontoviks in Suppression** and characterizes Guided as **selective removal**, not mass damage. The saved [#166 report](../battle-reports/161-170-n5-battle-report-tactical-analysis.md) gives mission/list context. A later [#122 Tunguska–Neoterra report](../battle-reports/121-130-n5-battle-report-tactical-analysis.md) offers the contrasting warning: huge Guided casualties did not replace pressing an antenna.

### Stop spending missile Orders when one of these becomes true

- The **mission's critical lane is already open**.
- You have killed/neutralized the **scorer/enabler**, and further kills do not deny the objective.
- The defender repeatedly clears Targeted or moves into a poor launcher range/illegal trajectory.
- **Direct shooting, FO, smoke or an E/M state attack** is now cheaper.
- Your remaining Orders are needed by an **eligible Specialist or zone holder**.
- Your attacker is about to force **Retreat!** prematurely for the mission you still need to finish (see [Endgame/Retreat strategy](endgame-retreat-and-loss-of-lieutenant.md)).

## 6. Defending against enemy Guided Missile strategies

### Before deployment and when going second

1. **Recognize the system**: a Guided-capable REM, Spotlighters/FOs, the initial Repeater net, and the **actual Pitcher launchers**. A visible normal ML or FTO REM **may not have Guided**.
2. **Space out important targets**, especially Fireteam members, Engineers and Specialists. Avoid giving one Circular-template shot an entire clustered support cell; check actual template and terrain reach.
3. **Do not place the only Hacker / Doctor / Lieutenant / mission runner inside easy enemy projected ZoC** merely because it cannot be seen from the enemy DZ. Distance from likely Pitcher landing walls matters.
4. **Layer defensive nodes** so killing one cheap Repeater or crossing one lane does not expose all protected models. Plan a **safe non-HI / non-TAG scoring path** where feasible.
5. **Preserve one attack route to the enemy enabler**: expendable gun, Camo/Infiltration, parachutist, KHD/Trinity, flank or FTO counter-fire. Your plan should not rely exclusively on winning direct Face to Face against the launcher.

### During the enemy Active Turn — prevent the *first* Guided shot

- **Contest or destroy the new Repeater/Pitcher** where legally possible. If the node cannot reach your valuable model, the hacker cannot simply skip network legality.
- **Reset against Spotlight** if that is the best defence; do not automatically choose Dodge against Comms Attacks. Factor in WIP, Firewall, BTS and that Spotlight requires failed Saves to apply Targeted.
- Consider **Dodge vs Reset** when already Targeted and a missile arrives: compare effective **PH minus no-LoF penalty** with **WIP minus Targeted penalty**, plus the huge benefit of **clearing Targeted** on a successful Reset. A high-PH model may prefer Dodge for immediate survival even though it can be targeted again.
- If an attack produces **Targeted**, proactively plan to **Reset / Engineer-clear** on a turn where doing so is worth the Order. Do not leave an elite key target exposed to repeat Guided just because it survived the first shot.
- **Do not ignore direct AROs while dealing with the cyber problem**. A network is dangerous because it can make one choice (Reset/clear the node) expose you to a different attack.

### During your Active Turn — dismantle the package in the cheapest order

| Enemy dependency | Efficient counterplay | Why this beats chasing the launcher |
|---|---|---|
| One exposed **Pitcher / Deployable Repeater** covers the lane | Shoot/clear it, then immediately move the HI/TAG or Specialist through the new safe route. | A cheap node can be the **actual** reason your army cannot operate. [#003](../battle-reports/001-010-n5-battle-report-tactical-analysis.md) provides a concrete example. |
| **Only Spotlight Hacker** supports several forward nodes | Attack that Hacker by KHD/physical flank or force it to protect itself; keep a backup route if it is too well screened. | Removing the single controller collapses much of the missile plan. [#021](../battle-reports/021-030-n5-battle-report-tactical-analysis.md) flags depending only on Jazz as a vulnerability. |
| Several Hackers, redundant nodes, but no spare Orders | **Ignore/route around**, spend Orders on objective control or a safe alternative flank. | Multiple Hackers are intimidating but do not make missile attacks free. |
| Protected **missile launcher** but exposed guns/specialists | Kill the **scoring/delivery** pieces or screen the target, instead of tunnelling on the bot. | A bot with no meaningful Targeted target/Orders cannot itself score most objectives. |
| High-value **Targeted TAG/HI** with recovery support | Use a sound **Reset/Engineer** and repeater-clearing sequence, while threatening the enemy's scoring line. | Do not try to outshoot every Guided blast with an expensive elite model. |
| Network covers one midfield corridor | **Split / redirect mission routes**, deploy reserve/AD pieces on another side, or use legal internal room geometry to stop a Guided trajectory. | Forces enemy to spend Orders rebuilding network and often makes their launcher irrelevant to the actual OP. |

**Examples of meaningful counterplay and limits:**

- [#056 Tunguska–Shindenbutai Battleground](../battle-reports/051-060-n5-battle-report-tactical-analysis.md) / [full original game](https://www.youtube.com/watch?v=UADKTi95X_s): the attacker actually deploys Pitchers, Spotlights, and fires Guided into JSA troops, with the defender choosing Dodge/Reset. The Shinden player's Hacker placement and limited recovery/alternate route matter. **Pre-N5.1:** transcript play does not overwrite current N5.3 rules.
- [#078 Corregidor–Starmada Evacuation](../battle-reports/071-080-n5-battle-report-tactical-analysis.md) / [video](https://www.youtube.com/watch?v=U2A2Y5BxMVs): Moran/Jazz/Vertigo pressure a link, but a **specialist route between the Repeater zones** and actual civilian extraction remained the better counterplan than simply duelling the gunline. **Caution:** the game includes nonstandard Tactical Support cards.
- [#229 Morats–Tunguska Crossing Lines](../battle-reports/221-230-n5-battle-report-tactical-analysis.md) / [full video](https://www.youtube.com/watch?v=843sIPoFsko): Tunguska has a Vertigo and hacking coverage, yet **Hollow Men/Heckler maintaining the scoring zones** are the more demonstrable reason for its result. The video includes an actual Dodge-versus-Reset Guided decision and shows how an apparent 8–0 does **not** prove that the missile bot alone was the winner.
- [#230 Nomads–Kosmoflot Uplink Center](../battle-reports/221-230-n5-battle-report-tactical-analysis.md): a sophisticated Nomad hacker shell has less direct traction against largely non-Hackable Ariadna (Spotlight remains legal, but alternatives may be better); both sides still must score consoles and the tech coffin. A non-Hackable piece is **not immune to Spotlight**.

**What to ask before trying to “counter Guided”:** Do I need to eliminate a Repeater, the Hacker, the launcher, or **none** of them to finish my own mission? A narrow safe corridor and one live Specialist may be the highest-percentage response.

## 7. Compact table-side checklist

**Attacking:** (1) Is the opponent worth the Orders? (2) Is the actual target legal for Spotlight/FO? (3) Is the Repeater live and not fatal to my Hacker? (4) Did the enemy **fail the Spotlight Saving Roll** and enter Targeted? (5) Does my **actual Guided profile** have legal range and trajectory, the prescribed mode, and remaining attacks this turn? (6) Is **Reset or Dodge** the better enemy defence, and what if it wins? (7) Will I still have Orders to score?

**Defending:** (1) Where is the *first* Repeater edge, and can I remove/bypass it? (2) Can the Hacker be scalpeled without exposing my entire army? (3) Is **Firewall / high BTS** protecting the Spotlight step, **ECM (Guided)** protecting the missile step, or both? (4) What are my *actual* Reset/Dodge numbers after MODs? (5) Can I clear Targeted by Reset/Engineer before another attack? (6) Which **scorer and corridor** must survive regardless of damage?

## 8. Source notes — original transcripts and evidence grades

**Rules:** [Guided](https://infinitythewiki.com/Guided), [Spotlight](https://infinitythewiki.com/Spotlight), [Reset](https://infinitythewiki.com/Reset), [Targeted](https://infinitythewiki.com/Targeted_State), [FO](https://infinitythewiki.com/Forward_Observer), [Repeater](https://infinitythewiki.com/Repeater), [Firewall](https://infinitythewiki.com/Firewall). Use these **over historical live-game arithmetic or podcast rules guesses**; check the latest published version before tournament use.

**Spotify / YouTube research directly checked against available transcripts:**

- **Loss of Lieutenant E155 — Burn City Brawl 2025 recap/winner interview**, [Spotify](https://open.spotify.com/episode/3bC5DmFnk3eFiNlZhBZBA3): ~**51:35–59:40** describes the Tunguska winner using Spotlight + Guided versus TAK suppression, active group compositions and “scalpel” decision-making. **First-hand player account**, not a sample of measured win rates; [saved #166](../battle-reports/161-170-n5-battle-report-tactical-analysis.md).
- **Loss of Lieutenant E161 — Pitcher Tierlist**, [Spotify](https://open.spotify.com/episode/1ZxuI8ZQ1zHJZ9aRPxYKft): Pitcher success does not ensure Spotlight success or useful Guided payoff; late discussion around **2:39:00–2:40:00** critiques the three-stage plan. **Panel opinion/strategic framework**, not factual hit probabilities.
- **Loss of Lieutenant E166 — The Art of the Fork**, [Spotify](https://open.spotify.com/episode/4AWYvbMuuQAeAYlaA26ghh): around **43:35–45:00**, Mine/Repeater/Hacker ARO dilemmas illustrate using network pressure *without* requiring a missile kill. **Rules principles must still be validated** against N5.3.
- **Loss of Lieutenant E176 — Deployment (Part 2)**, [Spotify](https://open.spotify.com/episode/109wmskmaxqFierHIG89kN) / [YouTube at 55:55](https://www.youtube.com/watch?v=UoYjrRvC5ic&t=3355s): distinguish defensive/on-table network, offensive Pitcher, protected cheap Hacker, and the reverse-hacking risk. **Deployment advice**, not a Guided damage demonstration.
- **#056 — Tunguska vs Shindenbutai**, [video](https://www.youtube.com/watch?v=UADKTi95X_s) / [saved analysis](../battle-reports/051-060-n5-battle-report-tactical-analysis.md): **observed** Pitcher placement, Spotlight/Targeted sequence and Guided launch with defender choices; **initial N5**, so check all rules anew.
- **#118 — Morats vs WinterFor**, [video](https://www.youtube.com/watch?v=bvNTyBHsGXM) / [saved analysis](../battle-reports/111-120-n5-battle-report-tactical-analysis.md): **first-hand commentary and observed play**; linked Dartoks and group-two Orders enable one Guided removal, but author says the missile is optional rather than a main gun.
- **#023 — Tunguska vs Hassassin**, [video](https://www.youtube.com/watch?v=HxYdE2Z8-0g) / [saved analysis](../battle-reports/021-030-n5-battle-report-tactical-analysis.md): **observed** firing at a Targeted model and explicit range/roll checks. Some transcript speech recognition is imprecise; no reliable fixed damage probability derived.
- **#229 — Morats vs Tunguska**, [video](https://www.youtube.com/watch?v=843sIPoFsko) / [saved analysis](../battle-reports/221-230-n5-battle-report-tactical-analysis.md): **observed** missile/Reset-versus-Dodge discussions plus non-missile scoring; live remarks on Short/Long Skills are not substitute rules.

**Archive synthesis:** Reviewed references to Guided, Spotlight and missile support across [#001–#241 report batches](../battle-reports/n5-battle-reports-and-tournament-reports.md) and [cross-report unit combinations](../battle-reports/cross-report-unit-effectiveness-and-combinations.md). Useful complements include [#021](../battle-reports/021-030-n5-battle-report-tactical-analysis.md) (missile **threat**), [#078](../battle-reports/071-080-n5-battle-report-tactical-analysis.md) (template pressure and civilian extraction), [#098](../battle-reports/091-100-n5-battle-report-tactical-analysis.md) (White Noise and network), [#122](../battle-reports/121-130-n5-battle-report-tactical-analysis.md) (Retreat does not equal mission victory), [#166](../battle-reports/161-170-n5-battle-report-tactical-analysis.md) (scalpel into suppression), and [#211](../battle-reports/211-220-n5-battle-report-tactical-analysis.md) (counter-pressure on Moran/Koalas). **Caution:** these are individual games, some in custom missions, with different N5 patches. They establish *possible play patterns*, not the likelihood of succeeding in an arbitrary matchup.
