# Defensive Architecture and the Reactive Turn

**Mission-anchored defender packages and matchups:** [N5.3 Objective Holding / Zone Domination / Carried Objectives](objective-holding-zone-domination-and-carriers-apex-value.md) prioritizes the **enemy's last legal contact/pickup square**, protected carrier behind Total Cover, and serial Mines/Template/Repeater screens. Differentiates high-cost TAG zone VP from an actual eligible Supply Box Specialist and scenario Baggage VP modifiers.

**Concrete N5.3 DZ-defense unit shortlist:** [DZ Defenders — apex/value, anti-alpha and impersonation](dz-defenders-alpha-strike-and-impersonation-apex-value.md). It distinguishes 360º rear-edge/Combat Jump screens from Biometric anti-IMP guards, mines versus Boost weapons, and Regular dual-role support from expendable Irregular speed bumps. Keep serial defenses and dispersed cheerleaders.

Infinity defence is not primarily about winning gunfights during the opponent's Active Turn. The stronger goal is to make the opponent spend too many Orders, expose important pieces, consume limited resources, and finish the turn in positions that can be punished.

A good defence therefore asks:

> **How many different problems must the opponent solve before they can reach the part of my army or the mission state that actually matters?**

This is a whole-table concept. Deployment Zone defence is only the innermost layer. Midfield markers, mines, hacking coverage, weak AROs, Suppressive Fire, hidden threats, objective guards, and protected counterattack pieces are all part of the same defensive architecture.

## Rules baseline

Current project rules baseline: **N5.3 + N5 FAQ v0.1**.

This note is primarily strategic rather than a rules summary. For exact rule semantics, use the repository `rules/` references. Related strategy notes include:

- [Deployment, Initiative, and Reserve strategy](deployment-initiative-and-reserve-strategy.md)
- [DZ strikes and DZ defense](dz-strikes-and-dz-defense.md)
- [Marker-state and deception strategy](marker-state-and-deception-strategy.md)
- [Hacking and network projection](hacking-and-network-projection.md)
- [Movement, positioning, and vision control](movement-positioning-and-vision-control.md)
- [Terrain, silhouettes and table geometry](terrain-silhouettes-and-table-geometry.md)
- [List robustness and threat coverage](list-robustness-and-threat-coverage.md)

---

## 1. Measure defence in Orders, not kills

A reactive model does not need to kill anything to succeed.

A cheap troop that forces the attacker to:

1. move into position;
2. spend an Order attacking it;
3. spend another Order finishing or bypassing it;
4. reposition afterward;

may have generated excellent value even if it inflicted no wound.

A useful mental model is:

> **Defensive value = Orders consumed + route distortion + resources forced + mission delay + attacker exposure - future utility sacrificed.**

This produces three broad defensive jobs.

| Defensive job | Purpose |
| --- | --- |
| **Kill ARO** | Has realistic odds of stopping or severely damaging the attacker |
| **Tax ARO** | Probably loses eventually, but forces Orders, rolls, positioning, or resources |
| **Trap ARO** | Hidden, marker-state, deployable, or network threat that changes how the attacker may move |

Strong defensive architecture usually contains all three.

### ARO efficiency is asymmetric

The Active Turn normally controls:

- target selection;
- range selection;
- movement geometry;
- Burst advantage;
- setup pieces such as Smoke, White Noise, Pitchers, Sensor, or support attacks;
- whether to continue or disengage.

Do not judge every reactive exchange by whether the defender can win a straight Face-to-Face roll.

A deliberately weak ARO can succeed simply by changing `Move + Move` into `Move + Attack`.

That one distinction can consume several Orders over the course of an attack run.

---

# 2. Build defence in depth

Do not think of defence as a line across the front of the Deployment Zone.

Think in **defensive belts**.

| Layer | Typical tools | Main purpose |
| --- | --- | --- |
| **Information layer** | Camouflage, Hidden Deployment, Holo/Decoy effects | Prevent the opponent from knowing the complete problem |
| **Approach layer** | midfield Camo, mines, Repeaters, cheap AROs | Tax movement toward your half |
| **Long-range gate** | sniper, Missile Launcher, HRL, Feuerbach, Total Reaction | Prevent unrestricted crossing of major open lanes |
| **Mid-range layer** | rifles, Marksman Rifles, Suppressive Fire, hacking | Punish the attacker after the long-range layer is solved |
| **Breach layer** | DTWs, mines, Perimeter weapons, CC threats | Make entry into valuable spaces dangerous |
| **Core layer** | cheap guards, spacing, body-blocking, protected support | Stop one breach from becoming a DZ collapse |
| **Recovery/counterattack layer** | Doctor, Engineer, protected attacker | Recover losses or kill the overextended attacker next turn |

The layers should preferably require **different counters**.

If every layer is a conventional gun, Smoke or White Noise may disable most of the defence at once.

If every layer is hacking, a non-Hackable attacker can invalidate the plan.

If every layer is deployables, Sensor, Deactivator, expendable troops, or careful Dodges may dismantle the position efficiently.

A stronger sequence looks like:

> **LoF threat → marker problem → mine → Repeater → short-range template → protected core.**

The opponent must repeatedly switch tools and reevaluate the attack.

**Concrete counter-switching example:** an MSV attacker beats the visible gun, a Sensor or expendable trooper probes the Camo/mine layer, a KHD handles the Hacker, and a disposable mine-clearer opens the final route. Even if every answer is already in the opponent's list, repositioning between them consumes Orders.

**Command Token as first-turn defence:** when going second, the eligible Strategic Use can remove two Regular Orders from the opponent's first-turn Order Pool (only one if Counterintelligence applies), provided the Order-count threshold is met. That reduction may save more of the army than exposing an additional ARO piece. This is a first-turn Tactical Phase action, **not an ARO**; see [Command Tokens](command-tokens.md) for the exact restrictions.

---

# 3. Serial defence is often stronger than parallel defence

Several defenders covering the same lane can look impressive while remaining easy to solve.

## Parallel defence

Three models all cover roughly the same long firelane.

The opponent finds one good attack position, one Smoke solution, or one superior range band and attacks them sequentially.

The same answer defeats the whole defensive package.

## Serial defence

The opponent instead encounters different problems at different points:

1. long-range ARO;
2. corner or elevation change;
3. mine or marker;
4. Repeater zone;
5. short-range defender;
6. objective guard.

The attacker cannot solve the entire defence from one location.

### Design gates rather than walls

A defensive **gate** is a location the attacker must cross where multiple threats become relevant together.

Examples:

- a corner covered by a mine plus a second LoF;
- an objective inside a Repeater with a hidden or protected Hacker;
- a rooftop exit covered from one direction by a rifle and another by a template piece;
- a narrow approach that exposes a Hackable attacker to both a gun and hacking;
- a midfield intersection covered by Suppressive Fire plus a deployable.

The key question is not:

> "How many models see this lane?"

It is:

> **"Where must the attacker commit, and what becomes relevant when they cross that point?"**

---

# 4. Crossfires without exposing the whole army

A crossfire is useful when the attacker cannot fight every defender from the same safe position.

The bad version is several models standing along one roofline where the Active-Turn attacker can pie-slice each one.

The better version uses **different angles and different depths**.

```text
           A
           ↓
------ corner --------
          X  objective
                ← B
```

The attacker can engage A from one approach, but advancing toward X eventually exposes a different angle to B.

Add a mine, Repeater, marker, or short-range template around X and the route becomes a layered defensive gate.

### Crossfire principle

> **Two defenders are mutually supporting only when attacking one does not automatically solve the other.**

This often means placing them on:

- opposite sides of a building;
- different elevations;
- staggered depth;
- opposite sides of an objective room;
- different approach corridors.

---

# 5. Protect ARO pieces from pie-slicing

The classic defensive failure is:

> "Four models cover the approach."

But the attacker can expose itself to exactly one defender at a time.

That produces four isolated Active-Turn gunfights rather than a real defensive network.

## Pie-slicing audit

For every major exposed ARO, ask:

- From what positions can the opponent see only this model?
- Can the attacker choose its ideal range before becoming visible to anything else?
- Can Smoke/White Noise isolate this defender from the rest of the architecture?
- Does killing this model open the entire route?
- Is there another threat covering the attack position rather than merely the same lane?

### Cover the attack square

One of the strongest defensive concepts is to protect the **location from which your ARO will be attacked**.

If a sniper is likely to be challenged from one rooftop corner, do not merely add another sniper looking along the same lane.

Instead, consider covering that attack square with:

- a mine;
- a Repeater;
- a hidden ARO;
- a different-angle rifle;
- a template threat;
- a marker that makes staging there uncertain.

The attacker should have to solve something merely to obtain the ideal duel.

---

# 6. Expose fewer models than instinct suggests

Not every model with a long-range weapon needs to begin the game standing up.

Every exposed model should have a specific defensive job.

A strong Turn-1 defensive setup might expose only:

- one credible long-range gatekeeper;
- one cheap disposable ARO on another route;
- one midfield or marker threat controlling a third route;

while the rest of the army remains protected.

The opponent then has fewer easy Active-Turn targets while still facing multiple routes that cannot simply be ignored.

### Ask why the model is visible

Good reasons include:

- protecting an objective the opponent must interact with;
- stopping an important `Move + Move` route;
- forcing a weapon or support resource to be spent;
- covering a staging position for another defensive layer;
- providing a credible threat that changes deployment or movement.

Poor reason:

> "It has a sniper rifle, so it should ARO."

A premium long-range profile may be more valuable hidden or Prone until a later turn.

---

# 7. Deliberately weak AROs and sacrificial speed bumps

Cheap reactive pieces are frequently valuable because they prevent free movement.

Examples include:

- Flash Pulse pieces;
- cheap Panzerfaust or disposable-weapon troops;
- rifle troops watching a narrow route;
- warbands or other DTW troops behind a corner;
- expendable midfield skirmishers;
- cheap REMs covering a necessary crossing.

Their purpose is often:

> **"You may kill me, but you cannot ignore me and keep moving."**

### Why this matters

A fast attacker using repeated `Move + Move` Orders can cross the table with frightening efficiency.

If every defensive layer requires an attack, Dodge, Discover, hacking exchange, or detour, that same run may consume most of the Combat Group.

A speed bump is especially successful when it makes the attacker:

- stop at a bad location;
- reveal a marker state;
- spend a disposable weapon;
- take a wound or risk one;
- enter a later layer without enough Orders to exploit it;
- abandon the deeper attack entirely.

### Sacrifice intentionally

Do not try to save every outer defender.

Some models should be deployed with the explicit expectation that they die while consuming resources.

This is the **crumple zone**.

The crumple zone protects the valuable army behind it by absorbing the first part of the attacker's turn.

---

# 8. Hidden AROs should punish commitment

Hidden Deployment and other concealed threats become strongest when they reveal **after the opponent has committed to a plan**.

Do not reveal automatically because the first available shot appears.

A stronger reveal may occur after the attacker has:

- crossed its previous safe position;
- left cover;
- entered a worse range band;
- spent several Orders reaching the area;
- committed its main attack piece;
- exposed a support piece or secondary target;
- begun an objective interaction;
- passed the point where retreat is cheap.

The value is not merely another attack roll.

It is the destruction of the opponent's assumption that a route or staging location was safe.

### Phantom defence

A faction or list capable of Hidden Deployment can defend apparently empty space simply through uncertainty.

The opponent may:

- avoid efficient movement lines;
- spend Orders probing;
- choose safer but longer routes;
- refuse to expose an important attacker to an apparently open lane.

Do not throw away that information advantage for a low-value ARO unless the exchange is worth it.

---

# 9. Marker-state defence can occupy space without attacking

A Camouflage or other marker near a route creates a decision problem even when it never reveals.

The opponent may have to ask:

- Is this a troop or deployable?
- Do I Discover it?
- Do I risk passing it?
- Can it have a template or disposable weapon?
- Is Sensor worth spending an Order?
- Is another hidden threat positioned behind it?

This produces an **information tax**.

The marker does not have to attack to generate defensive value.

Sometimes the best reactive decision is to remain a marker and preserve the problem for the next Order.

See [Marker-state and deception strategy](marker-state-and-deception-strategy.md) for the fuller information-game framework.

---

# 10. When to Dodge instead of shoot

Reactive players often overvalue the opportunity to fire a weapon.

The real decision is:

> **Which declaration best changes the opponent's next Order?**

### Lean toward Dodge when

- the model is valuable and the gunfight is strongly unfavorable;
- a successful Dodge can reach Total Cover;
- Dodge movement can change the next engagement angle;
- the model can reach Engage or otherwise block movement;
- multiple attacks affect the model;
- surviving one more Order matters more than inflicting a low-probability hit;
- moving the model will strengthen another defensive layer.

### Lean toward attacking when

- the model is intentionally disposable;
- the attacker is trying to run past rather than fight;
- the reactive weapon has a high-impact effect such as E/M, Stun, Explosive ammunition, template damage, or another disabling state;
- the trade is favorable even if the defender dies;
- the attack forces the opponent to stop using `Move + Move`;
- killing or disabling the attacker immediately protects a high-value breach point.

### Dodge as movement

Do not think of Dodge only as avoiding damage.

A successful Dodge can reposition the defence.

Useful outcomes include:

- disappearing behind a wall;
- closing a corner;
- moving into template range;
- changing which route is covered;
- reaching protection from another model;
- forcing the attacker to spend an additional Order reacquiring LoF.

---

# 11. Design ARO positions with an exit

When placing an exposed reactive piece, identify its **escape square** before finalizing deployment.

Ask:

> **If this model survives the first exchange, where does it go?**

Good ARO positions may have:

- a wall immediately behind the model;
- a parapet or roof edge that breaks LoF;
- a nearby corner;
- somewhere to become Prone;
- a safe Unconscious position reachable by a Doctor or Engineer;
- a retreat route that preserves a second useful firing angle.

Bad ARO positions often have enormous LoF but no exit.

That model effectively fights until it dies.

### Guts should change the architecture

Plan for the possibility that a surviving defender can use Guts positioning to:

- break LoF;
- retreat into a stronger layer;
- stop offering the opponent repeated favorable shots;
- become recoverable;
- force the attacker to advance before continuing.

A premium ARO piece is often best treated as:

> **peek → tax → survive if possible → disappear → reappear later.**

Not:

> **peek → duel until dead.**

---

# 12. Suppressive Fire networks

Suppressive Fire is strongest when it controls **pockets and intersections**, not when it attempts to imitate a sniper.

Good SF terrain includes:

- objective rooms;
- courtyards;
- midfield intersections;
- approaches to consoles;
- DZ breach points;
- short streets where enemies must enter the SF model's preferred engagement distance.

### Build networks rather than isolated SF pieces

Weak setup:

```text
SF1 ================= lane
SF2 ================= lane
SF3 ================= lane
```

One long-range solution may dismantle all three.

Stronger setup:

```text
       SF1 →
            intersection
mine X          ← SF2

        repeater
```

Approaching SF1 from its weak side brings the attacker toward SF2, a mine, or hacking coverage.

### Suppressive Fire as end-turn architecture

Before ending the Active Turn, ask whether an independent model can spend remaining Orders or Coordinated resources to create a defensive pocket around:

- an objective you just captured;
- a retreat route;
- a scoring zone;
- your attacker's resting position;
- a likely enemy counterattack corridor.

Do not place SF models merely because unused Orders remain. The model should protect something the opponent actually wants.

---

# 13. Defend objectives rather than irrelevant lanes

A beautiful firelane is strategically irrelevant if the opponent can score without crossing it.

Start with the mission.

For every important objective, ask:

- From where can it be interacted with?
- Where can an enemy Specialist safely stand before interacting?
- Where will the Specialist move after interacting?
- What pieces can contest the objective later?
- Can the opponent Smoke or White Noise the objective itself?
- Does the defensive network still matter after the first ARO dies?

### Objective-centred defence

Instead of only watching the road leading to a console, consider defending the **interaction space** with:

- mines or other deployables;
- a Repeater;
- a short-range defender;
- a marker-state troop;
- a Hidden Deployment piece;
- Suppressive Fire;
- a model positioned to counterattack or re-contest next turn.

The opponent may still reach the objective, but scoring should require several independent actions.

A button that costs five Orders is very different from a button that costs one.

---

# 14. Combine different threat channels

The best defensive gates often combine threats that demand different responses.

## Gun + mine

The attacker may have to choose between fighting the gun and managing the deployable.

## Gun + hacking

A Hackable attacker cannot evaluate the gunfight in isolation.

## Repeater + protected or hidden Hacker

The network projects danger without exposing the actual Hacker to conventional attack.

## Cheap DTW + expensive gun behind it

The template piece forms a speed bump protecting the premium defender.

## Marker + deployable ambiguity

The attacker may need to purchase information with Orders before moving through the space.

## Objective + area denial

The defence is not trying to prevent the opponent from entering the general area. It makes the exact scoring location dangerous.

### Orthogonal defence

This is the defensive equivalent of orthogonal redundancy from the list-robustness note.

Two identical weapons are redundant.

Two different mechanisms that defend the same strategic area are usually more resilient.

Examples:

- long-range gun + minefield;
- Repeater/Hacker + DTW guard;
- Camo marker + Suppressive Fire;
- visible ARO + Hidden Deployment threat.

---

# 15. Defend against Smoke, Eclipse, and White Noise by protecting movement space

LoF-based defence can be switched off or bypassed.

Therefore the army needs at least some defensive tools that threaten **space rather than sight lines**.

Useful examples include:

- mines;
- Perimeter weapons;
- Repeaters and hacking;
- Direct Template Weapons covering emergence points;
- close-combat threats;
- deployables positioned behind or around objectives;
- multiple defensive layers separated far enough that one template zone does not bypass everything.

A useful shorthand is:

> **Vision control defeats firing lanes. Area denial defends movement corridors.**

If one Smoke template or White Noise zone turns off the entire defensive plan, the architecture is too one-dimensional.

---

# 16. Protect the support structure after the breach

Do not assume the outer defence will stop every attacker.

Eventually something may reach the DZ or protected midfield.

The second question is:

> **What happens after the breach?**

Avoid placing all valuable functions where one successful attacker can move through them in sequence.

Separate and protect:

- Lieutenant;
- Doctor;
- Engineer;
- Hackers;
- EVO/support pieces;
- Order generators;
- mission Specialists;
- Fireteam lynchpins.

### Do not make the ARO piece the thing it protects

If the army's only Engineer is also exposed as a routine ARO, two roles fail together when it dies.

The same warning applies to:

- only Hacker + ARO duty;
- Lieutenant + ARO duty;
- only scoring Specialist + ARO duty;
- critical Fireteam member + exposed lane guard.

Sometimes the risk is justified, but the default structure should be:

> **disposable/interchangeable defence in front → valuable functions protected behind.**

---

# 17. Defensive architecture should degrade gracefully

The strongest test of a defensive plan is:

> **What does my table look like after my best ARO dies?**

Bad architecture:

```text
main sniper dies
      ↓
entire flank opens
      ↓
attacker enters DZ
      ↓
support structure collapses
```

Better architecture:

```text
main ARO dies
      ↓
attacker advances
      ↓
marker / mine layer
      ↓
Repeater or short-range layer
      ↓
DTW / SF / objective guard
      ↓
protected core still exists
```

The defence becomes weaker, but it does not disappear.

That is **graceful degradation**.

### Redundancy does not mean duplicates

A second sniper is not necessarily the best backup for the first sniper.

Often stronger:

> **sniper + mine + Repeater + cheap template guard.**

Each layer survives a different counter.

---

# 18. Preserve a counterpunch

Do not spend so much on visible reactive defence that the army lacks an Active-Turn response.

A strong structure may contain:

- relatively cheap disposable interference;
- protected Orders;
- one or more hidden/protected attack pieces;
- recovery support;
- a route to punish an overextended enemy.

The defence has two phases:

> **delay → counterattack.**

If the opponent spends most of a Combat Group crossing your layers and finishes with the main attacker stranded in midfield, a protected gunfighter, Hacker, CC piece, or mobile attacker should be able to exploit that position on your next turn.

### Defence creates attack geometry

When choosing where the opponent is likely to finish its run, ask:

- Can my attacker reach that location efficiently next turn?
- Will the enemy be outside its best range band?
- Can I attack it from behind or from a different elevation?
- Will it have lost marker state, wounds, disposable resources, or support?
- Can I recover a fallen ARO before counterattacking?

Good defence often makes the opponent's Active Turn create your next Active-Turn target.

---

# 19. Think in routes rather than firelanes

During deployment, trace likely attack routes separately for different enemy archetypes:

- ordinary infantry;
- HI/TAG;
- Smoke/Eclipse user;
- Hacker or Pitcher platform;
- Camo infiltrator;
- Combat Jumper;
- Parachutist;
- motorcycle or Vehicle;
- Super-Jump/Climbing Plus piece;
- close-combat missile.

Then identify where those routes **converge**.

Those convergence points deserve defensive investment.

A broad central lane the opponent never needs to use can be irrelevant.

A narrow alley linking midfield to your Lieutenant/support shell may deserve several layers.

### Route distortion is defensive value

A defensive element succeeds even if it never attacks when it forces the opponent to take:

- a longer route;
- a worse range band;
- a route through another threat;
- a route that costs Climb/Jump movement;
- a route that ends farther from the objective;
- a route that prevents the attacker from retreating safely.

Do not evaluate untriggered mines, hidden threats, or weak AROs as "doing nothing" when they changed movement.

---

### Rear-arc warnings and Look Out!

A long-range ARO is not a substitute for rear-arc coverage. Place a cheap observer where it can see Combat Jump, Parachutist, climbing, jumping, or fast flank routes into valuable backline positions. Do not assume guards facing forward will react to every arrival.

**Look Out!** lets a trooper with LoF to the active enemy spend its own ARO warning allies. Eligible allies that have not already reacted can attempt the rule's **Dodge (PH-3)** to turn their LoF without displacement. This does not grant a free shot or guarantee success; use it to make a backline assassination require another Order. See [Look Out!](../../rules/5a_Common%20Skills/Look_Out.md) for exact requirements.

---

# 20. Defending retreat routes and resting positions

Your own Active Turn should end with the next Reactive Turn already in mind.

When an attacker finishes its run, consider protecting its retreat position with:

- mines or Drop Bears;
- Suppressive Fire from another model;
- a nearby Repeater;
- a cheap template guard;
- a Camo marker;
- a second model covering the approach;
- Total Cover plus a route for Doctor/Engineer recovery.

The objective is not necessarily to make the attack piece untouchable.

It is to make the opponent spend enough Orders removing it that the previous attack still creates net advantage.

### Do not strand the attack piece in front of the architecture

A premium Active-Turn gunfighter that ends the turn exposed without support may become the opponent's easiest first target.

Whenever possible, end the run so the attacker becomes **another inner defensive layer**, not an isolated offering.

---

# 21. ARO declaration and reactive decision theory

Reactive play is a decision problem under uncertainty. The Active Player normally declares the first Skill, sees your ARO, and then chooses the second Skill. This gives the Active Player a built-in ability to **fork** reactive declarations: move into a position where shooting, Dodging, Resetting, Discovering, or doing nothing each answers a different possible continuation.

The central reactive question should therefore not be:

> **"What declaration gives me the best odds in this roll?"**

It should be:

> **"What declaration causes the Active Player the greatest future cost?"**

A useful reactive-value model is:

> **Reactive value = Orders added + resources consumed + route distortion + information preserved/forced + mission delay + counterattack exposure - future utility sacrificed.**

This is deliberately broader than probability of winning the current Face-to-Face Roll.

For exact timing and legality, see the repository rules for ARO, Dodge, Reset, Discover, Camouflaged State, Hidden Deployment, Stealth, Sixth Sense, Combat Instinct, Direct Template Weapons, and Coordinated Orders.

### Fireteam ARO forks

Fireteam members have individual ARO opportunities, but reacting members must declare the **same ARO Skill** to preserve Fireteam integrity; conflicting declarations can remove members or cancel the team. An attacker who exposes one member to gunfire, another to a template, and a third to hacking can force an unfavorable common choice.

**Deployment fix:** stagger members and arcs so only the appropriate guard reacts at each approach, rather than presenting the whole link to the same fork. Check the [Fireteam ARO rules](../../rules/6_Command%20and%20Fireteams/Fireteam_ARO.md) before assuming that separate members may freely Shoot/Dodge/Reset in one Order.

## 21.1 Think one Order ahead

After the Active Player declares the first Skill, identify what they are trying to make possible with the second Skill and the following Order.

A model moving around a corner may intend to:

- shoot;
- template;
- hack;
- Move again;
- enter Silhouette contact;
- place a deployable or Pitcher;
- interact with an objective on the following Order;
- reveal a marker-state attack;
- force your ARO and choose whichever second Skill punishes it.

The best ARO often does not maximize immediate survival or damage. It makes the **next Order awkward, expensive, or impossible**.

Examples:

- a Dodge into Total Cover may be worth more than a weak B1 shot because it forces another movement Order;
- a Flash Pulse may be worth more than damage because Stunned ends the attack run;
- a Reset may be worth more than returning fire because preventing IMM-B or Targeted denies an entire follow-up sequence;
- remaining Camouflaged may be stronger than revealing for a speculative shot because the unresolved marker continues taxing movement.

When evaluating an ARO, ask:

1. What does the attacker want this Order to accomplish?
2. What does the attacker want the **next** Order to accomplish?
3. Which declaration damages that sequence most?

## 21.2 Shoot vs Dodge vs Reset vs Discover vs Delay vs no ARO

| Declaration | Main purpose | Best when |
| --- | --- | --- |
| **BS/CC/Comms Attack** | Immediate removal, state, or credible threat | One success strongly changes the attack plan |
| **Dodge** | Survival plus positional change | Repositioning forces another Order or closes a route |
| **Reset** | Deny Comms setup or remove relevant states | Hacking success would make the next Orders much cheaper |
| **Discover** | Convert marker uncertainty into future attackability | Revealing the Marker materially worsens its next Order |
| **Delay** | Refuse to commit before a Marker reveals its intention | The Marker wants to attack or reveal this Order |
| **No ARO / remain concealed** | Preserve information and future threat | Revealing would buy too little compared with continued uncertainty |

Do not treat Delay as a generic option. It exists only where the rules explicitly permit it, most importantly against Camouflaged Markers. If the Marker does not reveal with the second Skill, the delaying Trooper loses that ARO.

Similarly, deliberately declaring nothing is not passive play. A Camo or Hidden Deployment piece may create more cost by remaining unknown than by taking one low-value shot.

## 21.3 Shoot when consequence matters more than survival

Attack when one successful hit creates a large future problem even if the odds are mediocre.

Strong reactive attacks often include:

- EXP/DA/T2 or other high-consequence ammunition against a key attacker;
- E/M, PARA, Adhesive, Stun, Flash, or hacking that disables rather than merely wounds;
- shooting a Specialist immediately before scoring;
- attacking a support piece that the main attacker depends on;
- forcing a fast attacker to stop using `Move + Move`;
- attacking an enemy whose loss collapses the rest of the attack sequence.

The relevant comparison is not only hit probability. It is:

> **probability of success × consequence of success.**

A Panzerfaust, Missile Launcher, E/M weapon, Flash Pulse, or disabling hacking program can be a better ARO than a statistically safer low-impact option because the attacker cannot comfortably accept the consequence of losing.

## 21.4 Dodge is often an investment in the next ARO

Dodge should be evaluated as **movement plus survival**, not merely as a defensive roll.

A successful reactive Dodge can:

- reach Total Cover;
- move behind a corner;
- move deeper into the defensive structure;
- change the next range band;
- reach template range;
- enter Engaged State;
- body-block or narrow a movement route;
- move toward Doctor/Engineer recovery access;
- force the attacker to reacquire LoF.

Compare the whole sequence.

If shooting gives a small chance to wound but Dodge gives a high chance to disappear behind Total Cover, the Dodge may be worth **an entire additional enemy Order**.

Likewise, a cheap troop that Dodges into Silhouette contact can transform an elite shooter's efficient gun run into a CC-removal problem.

This is why the correct reactive question is often:

> **"Where will this model be if the Dodge succeeds?"**

not merely:

> "What is my PH?"

## 21.5 Reset is about denying the follow-up

Reset is strongest when the incoming Comms Attack is a **setup effect** whose real value appears on later Orders.

Examples include attempts to:

- Immobilize a TAG or HI before shooting/CC;
- apply Targeted before Guided attacks or other follow-up pressure;
- force a high-value model to spend future Orders clearing states;
- establish a hacking advantage that opens a protected route.

Ask what the successful hack enables.

If accepting the current Comms Attack makes the next three enemy Orders dramatically stronger, Reset may be the highest-value declaration even when another ARO looks more immediately aggressive.

Conversely, do not Reset merely because a Hacker is present. If a disposable defender can instead remove the Repeater carrier, Pitcher platform, Hacker, or other enabling piece, attacking the infrastructure may create more future cost.

## 21.6 A Normal Roll can be better than a bad Face-to-Face

Reactive players often overvalue Face-to-Face Rolls because they combine attack and defence.

Sometimes contesting the attacker is exactly what the Active Player wants: their Burst, modifiers, and chosen range can reduce the reactive piece to a tiny chance of affecting the game.

A deliberate **Normal Roll trade** can be better when the defender is expendable and the attacker's survival matters much more.

The classic case is a Direct Template Weapon.

If a cheap template defender accepts that it will probably die and places the template instead of taking an awful B1 gunfight, the attacker must deal with the automatic template hit and make the appropriate Saving Roll unless it Dodges successfully. A return BS Attack against the template user is not Face-to-Face with the template.

Prefer the trade when:

- the defender is cheap or already strategically spent;
- the attacker is expensive or mission-critical;
- one wound/state may end the attack run;
- the attacker already spent several Orders reaching the defender;
- the template catches multiple Active Troopers;
- survival of the defender has little future value.

This principle extends beyond templates. Whenever the Face-to-Face odds are dreadful, ask whether another declaration creates an **independent risk** the attacker cannot cancel with superior dice.

## 21.7 Discover versus Delay against Markers

Against a Camouflaged Marker, the defensive problem is not simply "Discover or not."

### Discover

Discover is strongest when revealing the Marker now materially worsens its next Order.

Good reasons include:

- the Marker is approaching an objective;
- revelation removes future Surprise Attack leverage;
- another defender can exploit the revealed model on the next Order;
- the Marker must cross another ARO after this one;
- Discover modifiers are favorable;
- several different defenders can attempt Discover simultaneously.

Do not waste strong Discover pieces on low-value, long-range attempts merely because a Marker appeared. A failed Discover prevents that Trooper from trying against the same Marker again that Player Turn.

### Delay

Delay is strongest when the Marker wants to reveal and attack during the current Order.

It creates a useful fork:

> **Reveal and give me my full ARO, or remain concealed and accomplish less.**

But do not Delay automatically. If the Marker is perfectly happy to `Move + Move`, delaying may simply donate free movement.

Ask:

> **"Does this Marker need to reveal now, or am I letting it advance for free?"**

If allowing another Move would put the Marker in a decisive position, Discover or Dodge may be more valuable.

## 21.8 Preserve Camo and Hidden information when the reveal is too cheap

Information is a defensive resource.

Revealing a Camo or Hidden Deployment piece gives the opponent more than a target. It may reveal:

- exact identity;
- weapons and equipment;
- the fact that a marker is not a Mine;
- the location of a Hacker or support piece;
- the absence of another hidden threat in that area;
- the safe routes that remain after the reveal.

Therefore every concealed ARO has a **reveal cost**.

A Camo troop should often decline a low-value shot if staying a Marker continues to impose a Discover tax, protects Surprise Attack, or makes an objective approach uncertain.

Hidden Deployment makes the calculation even harsher because the opponent may not even know a threat exists. Do not reveal simply because the first legal shot appears. Strong reveal points are usually after the attacker has:

- crossed its previous safe position;
- spent several Orders reaching the area;
- left support behind;
- reached a mission-critical interaction point;
- entered an unfavorable range band;
- committed its primary attacker beyond cheap retreat.

A Hidden Deployment model that never reveals can still have generated value if the opponent distorted movement or spent Orders respecting the possibility.

## 21.9 Coordinated Orders: react to the model that matters after the Order

A Coordinated Order can activate several Troopers, but each Reactive Trooper chooses only one of those Active Troopers as the target of its ARO.

The obvious target is often the Spearhead because it normally retains the strongest Burst. That is correct when the Spearhead is also the key future threat.

But do not target the Spearhead automatically.

A non-Spearhead may be more important if it is:

- the Specialist that will score next;
- the Engineer supporting a TAG;
- the only E/M, template, or disabling weapon in the group;
- the easiest model to remove and therefore the best way to break the follow-up plan;
- a high-value support piece that is temporarily exposed only because of the coordination.

The useful question is:

> **"Which activated model creates the most enemy value after this Order resolves?"**

### Shoot one or Dodge the whole problem

If several coordinated attackers all affect the same defender, shooting one member may produce a Face-to-Face exchange against that model while allowing other attacks to resolve as Normal Rolls.

Dodge can therefore be substantially more attractive than shooting one participant, particularly when survival and repositioning matter more than trading into a specific member.

### Templates punish clustered coordination

A reactive template can also invert the usual efficiency of coordination. Several models moving through the same narrow geometry may all become exposed to one cheap template ARO.

Against armies likely to use coordinated advances, defend narrow gates with some template coverage rather than relying exclusively on conventional gunfighters.

## 21.10 Stealth, ZoC, Sixth Sense, and Combat Instinct

Do not count every ZoC or Hacking Area as a guaranteed reactive layer.

### Stealth

Stealth can suppress ZoC/Hacking Area ARO generation for movement-based Skills when the Active Trooper remains outside LoF. This allows a Stealth attacker to move through parts of a defensive network without provoking the usual Dodge, Reset, or hacking AROs.

This makes the following more important:

- actual LoF geometry;
- deployables that do not care about Stealth;
- positioning that forces the attacker to perform a non-movement Skill before reaching the valuable target;
- Sixth Sense;
- Combat Instinct.

### Sixth Sense

Sixth Sense is primarily a reactive anti-bypass tool. It lets the user respond to Attacks directed at them from outside LoF, defeats Stealth, and improves Dodge/Reset reliability by ignoring most negative MODs that would normally apply.

It does **not** create generic 360-degree awareness against every movement. An enemy simply moving outside LoF is not the same as an enemy attacking the Sixth Sense user.

Strategically, Sixth Sense removes many of the attacker's usual ways to create a safe approach followed by an uncontested attack.

### Combat Instinct

Combat Instinct solves a different problem. It defeats Stealth and ignores Surprise Attack MODs, but does not provide Sixth Sense's attack-triggered out-of-LoF perception.

A useful shorthand is:

> **Sixth Sense = harder to bypass or fork through awareness.**
>
> **Combat Instinct = harder to ambush through Stealth + Surprise.**

Both are valuable defensive anchors against infiltrators, impersonators, and short-range assassins.

## 21.11 Protect information and force information asymmetry

The Reactive Player manages three broad resources:

1. models and wounds;
2. position;
3. information.

The third is often spent too cheaply.

Revealing a hidden weapon, Hacker, Camo identity, Hidden Deployment piece, or template guard changes how every later enemy Order is planned.

Before revealing, ask:

> **"Will revealing this threat create more future cost than leaving the possibility of the threat intact?"**

If not, preserve it.

The inverse is also useful: Discover, Sensor, forcing a Marker to reveal, or baiting a hidden ARO can be valuable because it purchases information even when no model dies.

Reactive decision theory is therefore partly an **information economy**. A strong defence tries to make the Active Player commit Orders before they know the complete problem.

## 21.12 Template trading and future-cost math

A cheap reactive piece can produce large value by forcing a high-value attacker to choose between:

- Dodge and lose offensive tempo;
- attack and accept an unopposed template or other Normal Roll;
- stop and remove the defender first;
- take another route.

All of those outcomes can be defensive wins.

This is especially powerful near:

- objectives;
- narrow corners;
- DZ breach points;
- Fireteam/coordinated movement paths;
- retreat routes;
- support clusters.

A template defender is not primarily asking, "Can I kill this model?"

It is asking:

> **"Can I make this model spend an extra Order, lose movement, accept a Save, or stop the attack run?"**

That is the correct way to evaluate sacrificial template defence.

## 21.13 Reactive decision procedure

For actual play, use this sequence after the Active Player's first Skill:

1. **What is the attacker trying to accomplish this Order?**
2. **What second Skill are they hoping I allow?**
3. **What will their next Order be if I do nothing?**
4. **Can I force another movement/setup Order instead?**
5. **Is survival important, or is this defender disposable?**
6. **Would Dodge movement improve the next engagement more than shooting now?**
7. **Would Reset deny a setup that makes later Orders much stronger?**
8. **Against a Marker, does Discover matter now, or should I Delay?**
9. **Am I spending Camo/Hidden information for too little value?**
10. **Can a Normal Roll/template trade create more real risk than a terrible Face-to-Face?**
11. **Against a multi-model activation, which model matters most after this Order?**
12. **What declaration leaves the attacker in the worst position for my next defensive layer or counterattack?**

Then apply the governing question:

> **What declaration causes the Active Player the greatest future cost?**

That is the reactive-turn equivalent of target priority.

---

# 22. Turn-by-turn defensive priorities

Defence should change across the game.

## Turn 1

Priority:

- preserve Orders;
- prevent catastrophic breach;
- protect command/support structure;
- preserve future Specialists;
- force the first attacker to spend heavily.

Be conservative with valuable pieces.

## Turn 2

Priority:

- defend the developing score;
- protect surviving mission pieces;
- use damaged or expendable troops more aggressively;
- shape Turn 3 access routes;
- contest objectives and zones.

Some troops that were worth preserving on Turn 1 may now be legitimate speed bumps.

## Turn 3

Priority:

- defend the actual scoring state;
- sacrifice almost anything whose future Order generation no longer matters;
- body-block movement;
- force one extra Order before an objective interaction;
- occupy or contest zones;
- expose pieces if their survival no longer matters after scoring.

A Turn-3 defence should often be much more willing to trade models than Turn 1.

---

# 23. Common defensive failure modes

## The single-sniper fortress

The entire defensive plan depends on one premium ARO.

**Fix:** add midfield tax pieces, short-range defence, area denial, and a counterattack layer.

## The rooftop firing squad

Several models have excellent theoretical LoF but can be pie-sliced individually.

**Fix:** stagger depth, cover attack squares, and use different angles.

## The all-gun defence

Smoke, Eclipse, White Noise, or superior active shooting disables everything.

**Fix:** add mines, Repeaters, templates, markers, and movement-space control.

## The all-hacking defence

A non-Hackable attacker ignores the network.

**Fix:** pair hacking with physical area denial and conventional AROs.

## The expensive crumple zone

Valuable Specialists and attack pieces are exposed merely to slow the opponent.

**Fix:** use cheaper expendable troops for the first layer.

## The irrelevant firelane

The defender dominates a lane the opponent never needs.

**Fix:** defend routes to mission objectives and army structure.

## No exit square

A premium ARO survives but remains visible and simply gets attacked again.

**Fix:** deploy with Dodge/Guts escape geometry and recovery access.

## No counterpunch

The opponent spends eight Orders attacking, survives in midfield, and then remains uncontested.

**Fix:** preserve an Active-Turn piece that can exploit overextension.

## Defence disappears after one casualty

Killing one sniper or Hacker opens the table.

**Fix:** build orthogonal layers that degrade independently.

---

# 24. Practical whole-table defensive audit

Before finishing deployment, ask:

1. **What is the opponent's easiest route into my half?**
2. **Can the main attacker repeatedly Move + Move without interacting with anything?**
3. **Can one attack position pie-slice all visible AROs individually?**
4. **What protects the attack position from which my main ARO will be challenged?**
5. **If my best long-range ARO dies immediately, what is the next layer?**
6. **Which defenders are deliberately disposable?**
7. **Which models must survive for Orders, scoring, command, or recovery?**
8. **Does one Smoke/Eclipse/White Noise solution switch off most of the defence?**
9. **Does a non-Hackable attacker invalidate the network?**
10. **Are mines, markers, and deployables actually distorting useful routes?**
11. **Can exposed ARO pieces Dodge or use Guts into a meaningful safer position?**
12. **Can an Unconscious key ARO be reached by the Doctor or Engineer?**
13. **Are objectives themselves defended, or only the roads leading toward them?**
14. **What happens after an enemy breaches the outer layer?**
15. **Can a fast, airborne, vertical, or CC attacker bypass the assumed geometry?**
16. **Is there at least one threat the opponent cannot completely account for from Open Information?**
17. **Where is the opponent's main attacker likely to finish after spending six to eight Orders?**
18. **What attacks that model on my following Active Turn?**
19. **Which ARO declaration would create the greatest future Order cost rather than merely the best current roll?**
20. **Against Camo/Hidden pieces, am I preserving information until the reveal actually matters?**
21. **Can a parachutist, Combat Jumper, jumper/climber, or fast flanker arrive in my rear arc unopposed? Is there an observer who can use Look Out!?**
22. **Could one Order fork multiple Fireteam members into incompatible Shoot/Dodge/Reset choices?**
23. **If going second, am I using the eligible Strategic Command Token option to reduce the attacker's first-turn Orders?**

The last questions link defence directly to reactive decision quality and counterattack planning.

---

# 25. Compact doctrine

A strong Reactive Turn can be summarized as:

> **Uncertainty → tax → gate → breach defence → protected core → counterpunch.**

The practical principles are:

- defend the mission and army structure, not every visible lane;
- force interaction before the attacker reaches valuable pieces;
- prefer serial layers to several identical parallel AROs;
- cover attack positions and commitment points rather than merely adding more guns;
- use cheap troops deliberately as Order taxes;
- preserve hidden and marker-state threats until the reveal changes the attack plan;
- choose AROs by future cost, not merely current Face-to-Face odds;
- Dodge when movement/survival costs the opponent more than a weak shot;
- accept Normal-Roll/template trades when an expendable defender can impose disproportionate risk;
- use Reset to deny setup sequences rather than merely react to hacking in isolation;
- Discover or Delay against Markers according to what the Marker needs to accomplish next;
- against Coordinated Orders, react to the model whose survival matters most after the Order rather than automatically targeting the Spearhead;
- account for Stealth, Sixth Sense, and Combat Instinct when evaluating ZoC and ambush geometry;
- give premium AROs an escape route and recovery path;
- use Suppressive Fire to control pockets and intersections;
- combine LoF, hacking, templates, deployables, and information threats;
- assume the outer layer can fail and protect the support core anyway;
- preserve a counterattack piece;
- build the defence so losing one important model weakens it rather than collapsing it.

The goal is not to construct an impenetrable wall. Infinity's Active Turn is too powerful for that to be a reliable plan.

The goal is to create a table where every additional step into your position costs something, and where the opponent eventually reaches the point at which continuing the attack is no longer worth the Orders required.

## Cross-game N5.3 ARO tier and deployment study

The [ARO apex/value tier list and matchup guide](aro-units-apex-and-value.md) compares premium hidden missile ambushes, durable MSV/neurocinetics shooters, low-SWC Total Reaction REMs, Panzerfaust/Flash/DTW disposable AROs, mines and anti-DZ screens. It explicitly ranks **maximum reactive impact separately from cost effectiveness**, reconciles current N5.3 profiles with competing video/podcast views, and explains serial defence and when to decline an ARO. Exact profiles and Fireteams remain in the authoritative `sectorials/` files.

## Additional media leads from the imported condensed guide

The imported note specifically recommends **Loss of Lieutenant, ep. 165: Automatic Reaction Order (ARO)**; **ep. 166: The Art of the Fork**; **Infinity the Dante: MSV and Marksmanship AROs — Infinity N5**; and **Shipwreck / Tunnel Fission: Deployment in Infinity**. These titles are retained as viewing/reading leads, **not newly transcript-verified findings** from this merge. For source-linked comparisons and disagreements, use the [ARO apex/value guide](aro-units-apex-and-value.md).
