# Defensive Architecture and the Reactive Turn

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

# 21. ARO decision framework

When an enemy activates, do not reflexively choose the most aggressive declaration.

Use this sequence.

## Step 1 — What is the attacker actually trying to achieve?

Possibilities:

- cross the table;
- remove this defender;
- reach an objective;
- enter the DZ;
- place a Pitcher or deployable;
- Discover a marker;
- force the defender to reveal;
- reposition for the next Order.

## Step 2 — What declaration hurts that plan most?

The answer may be:

- Shoot;
- Dodge;
- Reset;
- template attack;
- hacking ARO;
- Discover;
- remain in marker/hidden state where legal;
- accept the sacrifice because another layer matters more.

## Step 3 — What happens next Order if this succeeds?

This is the critical question.

A mediocre attack may be worse than a Dodge that breaks LoF and costs another Order.

A low-damage Flash Pulse may be better than preserving a cheap model if Stunned would end the attack run.

A marker reveal may be worse than remaining concealed and controlling the route.

Think one Order beyond the current roll.

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

The last two questions link defence directly to counterattack planning.

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
- Dodge when movement/survival costs the opponent more than a weak shot;
- give premium AROs an escape route and recovery path;
- use Suppressive Fire to control pockets and intersections;
- combine LoF, hacking, templates, deployables, and information threats;
- assume the outer layer can fail and protect the support core anyway;
- preserve a counterattack piece;
- build the defence so losing one important model weakens it rather than collapsing it.

The goal is not to construct an impenetrable wall. Infinity's Active Turn is too powerful for that to be a reliable plan.

The goal is to create a table where every additional step into your position costs something, and where the opponent eventually reaches the point at which continuing the attack is no longer worth the Orders required.
