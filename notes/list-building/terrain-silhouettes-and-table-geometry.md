# Terrain, silhouettes and table geometry

**Radial deployment/table audit — [Loss of Lieutenant E176 Part 2 ~18–39m](https://www.youtube.com/watch?v=UoYjrRvC5ic&t=1080s), full transcript checked 27 Oct 2026:** Radial DZs are **narrower and deeper**, enabling serial AROs/Lt depth but reducing sideways breakout lanes and available S4/S7 staging. The nearest corners can be close while **far-flank objectives/HVTs are far away**; Infiltration, FD and Parachutist can earn more Orders saved, and long diagonal lines sometimes make **Sniper range bands** important against traditional missile positions. Examine **multiple terrain heights**, back-DZ escape, any **objective-room LoF convention** and central building shadows; the speakers prefer true-LoF plus meaningful interior scatter but explicitly say event/table agreement decides. [Part 1 ~3:04:52](https://www.youtube.com/watch?v=il2w0PSGr0U&t=11092s) gives an actual sparse-compound map-reading exercise (roof-vs-fence height, objectives, protected stairs, TAG shelter) that cannot be copied as universal geometry. [Main checklist](deployment-initiative-and-reserve-strategy.md#part-2-radial-corner-deployments-change-the-price-of-mobility-e176-1839m).

## Core principle

Infinity terrain is not merely **Cover**. It defines three overlapping maps:

1. **movement map** — where each silhouette can physically travel;
2. **LoF map** — where models can see and be seen;
3. **attack-volume map** — where templates, hacking, deployables, Super-Jump, Climbing Plus, etc. can project threats.

Different silhouettes are effectively playing on different tables.

**Rules baseline:** the repository's [N5.3 + N5 FAQ v0.1 references](../../rules/README.md) govern exact legality and movement/LoF checks. This is a strategic table-reading guide, not a replacement for the rules pages.

An S2 trooper, S4 Remote, and S7 TAG may all have the same nominal route to an objective while having radically different real routes, exposure, corner costs, and hiding options.

The strategic question before deployment is therefore not just:

> Where is the Cover?

It is:

> **What routes, firing angles, hiding volumes, and access restrictions does this table create for each important model?**

---

## 1. Treat Silhouette as a movement and exposure stat

Silhouette controls much more than whether the miniature fits aesthetically.

Approximate standard profiles:

| Silhouette | Base | Height | Typical geometry consequence |
|---|---:|---:|---|
| S2 | 25 mm | 40 mm | Excellent access, easiest to hide, can use Narrow Gates |
| S3 | 40 mm | 32 mm | Wider but low; moderate routing tax |
| S4 | 55 mm | 32 mm | Very wide but low; strong hiding height, poor dense-terrain access |
| S5 | 40 mm | 45 mm | Moderate footprint and exposure |
| S6 | 40 mm | 55 mm | Moderate footprint but tall exposure |
| S7 | 55 mm | 67 mm | Wide and tall; routing and concealment both matter |
| S8 | 70 mm | 70 mm | Extreme footprint and exposure |

Use the **silhouette volume**, not the sculpt.

A rifle barrel, antenna, sword, tail, etc. does not create LoF by itself.

### Width problem vs height problem

Separate two questions:

- **Can the base pass through the route?**
- **Can the silhouette remain hidden while doing so?**

S4 and S7 both have large footprints, but behave very differently vertically.

An S4 Remote may disappear completely behind a relatively short wall yet struggle to negotiate a dense alley.

An S6 Heavy Infantry model may fit through the same 40 mm route much more easily but become visible over terrain that completely conceals S2/S4.

### Practical doctrine

When deploying an expensive large model, physically trace:

- launch route;
- first attack position;
- objective route if relevant;
- retreat position;
- fallback route if the preferred lane is blocked.

Do not assume the table that looks open to S2 is open to a 55 mm or 70 mm base.

---

## 2. Large silhouettes gain vaulting advantages

Large silhouettes are not purely disadvantaged.

The maximum obstacle height that can be vaulted is based on the troop's Silhouette height.

That means large/tall troops can casually cross obstacles that may require additional movement decisions from smaller infantry.

This matters when assessing:

- low walls;
- planters;
- barricades;
- scatter terrain;
- multiple shallow elevation steps.

### Table-reading implication

Do not label every obstacle as simply "blocking terrain."

Ask:

> **Which silhouettes can vault this in their normal route?**

A table filled with waist-high scatter may tax S2 movement while barely slowing a TAG.

---

## 3. Narrow terrain is access control

Narrow Gates are strategically important because only suitable small silhouettes can pass through them.

Going Prone does not turn a larger model into an S2 model for access purposes. **Formal Narrow Gates admit S2 or lower, while Wide Gates admit any Silhouette**, regardless of ordinary physical appearance or the Prone State. Agree and mark Access Widths with the opponent before play; the Access Width rule takes precedence over general movement permissions. See [Scenery Structures — Access Width](../../rules/7_Terrain,%20Scenery,%20Triumph,%20Table,%20Scenarios,%20ITS/Scenery_Structures.md).

This creates **S2-only movement networks**.

### Strong uses

Use narrow access to:

- move Specialists through buildings large attackers cannot enter;
- create safe retreat paths;
- establish protected objective routes;
- hide vulnerable support pieces inside inaccessible interiors;
- force a TAG/Remote to circle a building instead of taking the direct route.

### Important distinction: inaccessible is not automatically safe

A large model may be unable to enter a doorway while still having LoF through the opening.

So good access-control terrain usually needs:

**narrow entrance + interior depth + lateral offset / internal corner**

rather than simply putting the model directly behind the doorway.

### Informal bottlenecks

Even when terrain is not formally designated a Narrow Gate, actual base clearance matters.

A 30 mm alley may be:

- comfortable for S2;
- impossible for a 40 mm base;
- completely irrelevant to a 55 mm TAG.

Before deployment, look for natural **base-size filters**.

---

## 4. Large bases pay a corner tax

Movement around corners must account for the whole base.

The larger the base, the farther its outside edge has to travel to clear tight geometry.

This creates a significant hidden movement cost for:

- S4 Remotes;
- Motorcycles;
- TAGs;
- large Peripherals;
- large warbands / creatures.

### Strategic consequence

A model with excellent MOV can still be slow on a dense table.

Do not estimate movement as a straight-line distance to the objective.

Trace the actual path through:

- 90-degree corners;
- alley mouths;
- cargo-container gaps;
- stair landings;
- building entrances;
- scatter terrain.

### Defensive application

A zig-zag approach can be more effective against large attackers than one solid wall.

Every forced turn can:

- cost movement;
- create another ARO window;
- force another pie-slice;
- expose a different side;
- make retreat more expensive.

---

## 5. LoF is silhouette geometry, not eye-level geometry

Infinity does not normally use the miniature's physical head position.

Check LoF between silhouette volumes.

Only a small visible portion may be needed to establish LoF: the visible area must meet the **3 × 3 mm minimum**. Tiny exposures can matter, but a smaller sliver is not automatically sufficient. Check the facing/180° front arc as well as the Silhouette volumes. See [Line of Fire](../../rules/1_Basic%20Rules/Line_of_Fire.md).

### Reciprocal LoF heuristic

If your active model can see enough of an enemy silhouette to attack it, assume that enemy can usually see you back if facing permits it.

Do not rely on intuitive arguments such as:

- "my model can see his head but he cannot see mine";
- "my gun is above the wall";
- "the sculpt is crouching."

Use the silhouettes.

### Elevation changes target availability, not reciprocity

A high model may see behind low terrain that blocks a ground-level attacker.

That creates new engagements, but usually also exposes that elevated model to reciprocal LoF.

Elevation is therefore an **angle generator**, not automatic safety.

---

## 6. Pie-slicing is a geometry problem

Two defenders covering the same street do not automatically create a two-model ARO.

If the active player can move to a point where only one defender becomes visible, resolve that fight, then reveal the second defender later, the defense can be dismantled sequentially.

### When building ARO networks ask

> **Can the attacker expose itself to only one defender at a time?**

If yes, the apparent overlap is weak.

### Stronger crossfires

Better geometry makes it difficult to acquire LoF to A without simultaneously exposing to B.

Useful methods include:

- defenders at meaningfully different horizontal angles;
- defenders at different elevations;
- one gun plus a hidden/deployable threat at the corner;
- a lane where moving farther to isolate one ARO crosses another threat zone;
- overlapping long-range and short-range consequences.

### Deployment test

From the opponent's likely attack corner, imagine sliding the active silhouette outward millimetre by millimetre.

Ask which defender appears first.

If every defender appears one at a time, the crossfire may not be a real crossfire.

---

## 7. Cover geometry: terrain between models is not enough

Partial Cover is not simply "something is in the way."

A model normally needs the relevant scenery to obscure part of its silhouette **and be in contact with it**.

### Practical doctrine

If a model is meant to fight from a wall or corner:

> **Touch the terrain.**

Do not stop a few millimetres away and assume the terrain still grants the Cover MOD.

### Corner play

When slicing a corner offensively, try to achieve all three:

1. expose only the desired target;
2. stay in contact with the cover piece;
3. avoid creating secondary LoF from another angle.

### Total Cover vs Partial Cover

Distinguish:

- **Partial Cover** — helps a firefight;
- **Total Cover** — removes LoF and often removes the attack entirely.

For expensive pieces in Reactive Turn, Total Cover is generally far more valuable than favorable Partial Cover.

---

## 8. Prone is a geometry tool, not merely a defensive status

Prone changes the model's effective silhouette dramatically.

This can convert terrain that merely obscures a standing model into complete visual protection.

### Strong routine

**Move normally -> finish Prone behind parapet / wall / rooftop lip.**

Under the N5.3 rule, a trooper may enter or cancel Prone at the **start or end** of an eligible Movement-labelled Skill or ARO (**except Jump and Berserk**), not mid-route. Going Prone at the end does **not** reduce the movement distance already travelled upright; moving while Prone halves the applicable distance. See [General Movement Rules](../../rules/2_Movement/General_Movement_Rules.md) and [Prone State FAQ](../../rules/8_Game%20States%20and%20Glossary/Prone_State.md).

### Rooftop use

A rooftop with a low parapet may be:

- dangerous to a standing S2 model;
- excellent Total Cover to a Prone model;
- still poor protection for a TAG or other model that cannot use Prone.

### Deployment doctrine

When placing an Order generator, Specialist, Hacker, Doctor, Engineer, Lieutenant, etc. on an upper level, check the **Prone silhouette**, not just the standing silhouette.

A model that is safe Prone can activate later, stand, act, and disappear again.

### Models that cannot Prone

Large non-Prone-capable troops need genuine hiding volume.

Do not assume a parapet that protects infantry protects:

- TAGs;
- vehicles;
- many mounted troops;
- other restricted profiles.

---

## 9. Rooftops are staging areas, not automatically sniper nests

A rooftop provides:

- elevation;
- firing angles;
- routes around ground obstacles;
- places to go Prone;
- access to unusual objectives or approach vectors.

But it may also create a movement trap.

### Before deploying on a roof ask

- How does the model get down?
- Is there a ladder or stair?
- Can it safely approach the edge?
- Is there a parapet that fully hides it Prone?
- Which enemy rooftops can see it?
- Can Super-Jump attack it from behind?
- Can Climbing Plus reach the blind side?
- How many Orders does retreat cost?

### Order-trap principle

A perfect firing position is not perfect if leaving it costs half a turn.

A 30-point model that dominates Turn 1 but requires three Orders to rejoin the mission may become strategically stranded.

---

## 10. Rooftop-edge peeking

During Move, the rules explicitly allow a trooper to **peek over a roof edge with up to half its Silhouette**, including to gain LoF to targets at a different level. Model the exact route and ARO exposure under the [General Movement Rules](../../rules/2_Movement/General_Movement_Rules.md); this is not permission to finish in an unsupported position or exceed the permitted peek.

This makes roof lips behave much like horizontal corners.

### Offensive use

Use the minimum exposure needed to acquire the target.

Think of the roof edge as a **vertical pie-slice**.

Expose progressively rather than simply moving the model to the center of the roof edge.

### Defensive implication

Do not assume a model several centimetres back from a roof edge is safe merely because a ground model cannot currently see it.

A moving enemy may be able to reach an edge angle that reveals it during the Order.

---

## 11. Ladders and stairs are vertical roads

Ladders and stairs often allow ordinary Movement-labelled Skills rather than forcing inefficient Jump/Climb sequences.

Treat them as movement lanes.

### Before deployment identify

- every ladder into your DZ;
- every ladder onto an objective roof;
- every stair connecting table levels;
- where a model appears when it reaches the top;
- whether the top exit is covered by mines, templates, hacking, or guns.

### Defensive doctrine

A ladder exit is similar to a doorway.

Cover it with:

- a template;
- mine;
- close-range gun;
- Repeater / Hacker;
- Perimeter weapon;
- hidden model;
- crossfire.

Do not leave a clear ladder ending beside your Lieutenant or primary attacker.

---

## 12. Ordinary Climb creates vulnerable transitions

Normal Climb can be Order-intensive and can leave a model in tactically poor states or positions while moving on vertical surfaces.

### Exploit vertical transition points

If an enemy must climb the obvious wall, place defenses so that reaching the top exposes them to:

- templates;
- Suppressive Fire;
- mines;
- close-range AROs;
- melee threats;
- hacking zones.

### Do not strand yourself

Before putting an ordinary infantry model on an inaccessible upper ledge, calculate the cost of returning to ground level.

Vertical distance can create an **Order debt** that only becomes visible later in the game.

---

## 13. Climbing Plus turns walls into roads

Climbing Plus changes table evaluation fundamentally.

Do not classify vertical walls as impassable to these models. Climbing Plus permits Move/Dodge on a vertical surface and other Short Skills while hanging, but **does not grant Partial Cover on vertical surfaces**; the user must still follow movement, end-position, and exact-trajectory restrictions. See [Climbing Plus](../../rules/5b_Special%20Skills/Climbing_Plus.md).

A Climbing Plus attacker may:

- use the blind face of a building;
- bypass a guarded doorway;
- reach the side of an elevated target;
- traverse a facade instead of a street;
- generate LoF from unusual heights;
- attack from a direction that ordinary infantry could never use efficiently.

### Best offensive use

Do not climb the front wall just because you can.

Prefer:

1. approach a blind wall;
2. travel vertically outside conventional LoF;
3. appear at exactly the height/angle needed;
4. attack one isolated target;
5. finish where retaliation is awkward.

### Defensive doctrine

Against Climbing Plus, ask:

> **Which wall is the safest approach to my supposedly hidden model?**

The answer is often the wall you were not planning to defend.

---

## 14. Super-Jump creates attack vectors through empty air

Super-Jump means the attacker is not constrained to the ground movement network.

Terrain that protects against ordinary shooters may not protect against a model that can rise above it, acquire LoF briefly, and land back behind safety.

### Common mistake

"Nobody on the street can see this model" is not sufficient protection.

Check whether an enemy can jump high enough to see over:

- containers;
- low buildings;
- rooftop lips;
- walls;
- vehicles;
- scatter terrain.

### Cover limitation

Jumping models generally cannot rely on Partial Cover while travelling through open air.

So Super-Jump attack runs are strongest when they expose to **one target**, not several. **A normal Jump cannot reverse course midair;** a return-to-start attack trajectory needs the appropriate ability (such as **Super-Jump: Jet Propulsion**) and a legal measured path. Declare the entire trajectory so all AROs can be checked. See [Super-Jump](../../rules/5b_Special%20Skills/Super-Jump.md) and [Jump](../../rules/2_Movement/Jump.md).

### Vertical pie-slicing

A good Super-Jump attack often resembles pie-slicing:

- rise only enough to see the desired target;
- avoid cresting enough to reveal additional AROs;
- attack;
- finish back in safety when the skill/profile allows the useful trajectory.

### Defensive answer: volumetric hiding

Protect high-value models behind scenery that is:

- tall enough;
- deep enough;
- layered enough;

that an attacker cannot simply rise into LoF from nearby.

Use several blockers, not only one low wall.

---

## 15. Template geometry is three-dimensional

Templates are not abstract target lists.

Their Area of Effect occupies physical space and interacts with scenery and silhouette positions.

### Better anti-template deployment

Do not merely "spread models out."

Use **hard geometry** between them:

- opposite sides of a wall;
- different floors;
- different corners;
- roof/parapet separation;
- interior/exterior separation.

A blast that cannot propagate through Total Cover is far less dangerous than one where models are merely an extra inch apart. Templates have **three-dimensional Area of Effect** (normally with height equal to the template's radius or half its width); a target must lie within that volume and be reachable from the **Blast Focus** without intervening Total Cover. See [Template Weapons and Equipment](../../rules/3_Combat/Template_Weapons_and_Equipment.md).

### Doorways and corners

Direct Templates become especially threatening around:

- doors;
- narrow alleys;
- ladder exits;
- stair landings;
- objective consoles;
- clustered Fireteams;
- deployment-zone chokepoints.

Avoid lining up multiple valuable silhouettes behind the same approach.

### Prone vs templates

Prone can sometimes reduce the model's vertical exposure enough that a template which would touch a standing silhouette no longer reaches it.

Check actual three-dimensional geometry when relevant.

### Cover is not the same as template protection

Partial Cover may do little against the attack mode you fear.

Against templates, seek **Total Cover from the relevant origin / Blast Focus**, not merely the ordinary BS-Attack Cover bonus.

---

## 16. Elevation changes range and exposure

Vertical displacement changes the actual distance between models.

This can push attacks into or out of important range bands.

### Before choosing an elevated firing point check

- horizontal distance;
- vertical difference;
- actual diagonal distance;
- whether the elevation changes the preferred weapon band.

A target that appears "24 inches away" across the table may be meaningfully farther once height is included.

### Weapon interaction

Elevation can therefore make:

- Rifle / Spitfire bands worse;
- Sniper / Missile / Feuerbach bands better;
- template approaches harder;
- shotgun positioning less convenient.

Do not choose a rooftop only because it has LoF. Check whether the weapon actually wants that distance.

---

## 17. Large-base hiding requires deliberate planning

Large models often die because the player finds a good firing position but not a good **post-attack parking position**.

### Before activating a TAG / S4 attack Remote ask

- Where can it end completely out of LoF?
- Can its entire silhouette hide there?
- Can its base physically rotate / turn through the route?
- Is there enough width to retreat if the attack stalls?
- Does the hiding spot protect against elevated LoF?
- Does it protect against Super-Jump / Climbing Plus?

### Attack-route doctrine

For expensive pieces, plan:

**launch -> engagement -> fallback**

before spending the first Order.

If the fallback location does not exist, the attack is much more committal than it appears.

---

## 18. Use terrain to exclude the opponent's best attacker

One of the strongest forms of table control is forcing the opponent's ideal attacker to use a bad route.

Examples:

- S2 Specialist enters a building a TAG cannot enter;
- objective can be approached through an alley too narrow for S4;
- Prone infantry uses a low tunnel / parapet network while tall attackers remain exposed;
- defender places a key model where the opponent's long-range piece cannot obtain useful LoF without moving several Orders;
- attack route forces a TAG to negotiate repeated corners while infantry takes a direct interior path.

### Strategic objective

Do not merely ask:

> How do I defend against the enemy's strongest piece?

Also ask:

> **How can the table prevent that piece from being the right tool at all?**

This is especially valuable against very expensive models whose cost assumes they can project force efficiently.

---

## 19. Deployment-zone evaluation

Choosing deployment side can be strategically decisive on an asymmetric table.

### Evaluate each DZ for your army specifically

Do not ask which side "looks better."

Ask which side gives **your silhouettes and attack plan** better geometry.

### Primary questions

#### Launch lanes

Can your main attack piece leave the DZ without:

- spending several lateral Moves;
- crossing an exposed lane;
- negotiating a large-base bottleneck;
- climbing unnecessarily?

#### Total-cover parking

Can your expensive models hide completely?

Check this for:

- S2 standing;
- S2 Prone;
- S4;
- S6/S7;
- whatever large profiles your list actually contains.

#### Rooftop access

Are there useful roofs?

Can your troops actually reach and leave them efficiently?

#### Objective routes

Can S2 Specialists approach objectives through protected paths?

#### Enemy attack vectors

Does the opposing DZ have an easy rooftop / Super-Jump / Climbing Plus angle into your backline?

#### Large-base mobility

Can TAGs/Remotes reach the center without route taxes?

#### Retreat routes

Can an attacker finish its run somewhere useful rather than dying in the open?

---

## 20. Pre-deployment table scan

A useful table-reading routine:

### Step 1 — Find the movement skeleton

Identify:

- main streets;
- alleys;
- interior routes;
- ladders;
- stairs;
- roof links;
- climbable faces;
- narrow gates;
- bottlenecks.

### Step 2 — Trace S2 routes

From each DZ to:

- main objectives;
- midfield;
- enemy DZ approaches;
- safe retreat locations.

### Step 3 — Trace your largest-base routes

Repeat with the actual footprint of:

- TAG;
- S4 Remote;
- bike;
- large Peripheral;
- other key large model.

### Step 4 — Map true Total Cover

Find hiding places for:

- standing S2;
- Prone S2;
- S4;
- tallest / largest model.

### Step 5 — Map elevated attack vectors

Check:

- roofs;
- ladders;
- Super-Jump arcs;
- Climbing Plus surfaces;
- elevated long-range positions.

### Step 6 — Map pie-slice points

Find corners from which an attacker can reveal your defenders sequentially.

### Step 7 — Map template traps

Mark:

- narrow doors;
- ladders;
- stair exits;
- small rooftops;
- clustered consoles;
- DZ bottlenecks.

### Step 8 — Compare deployment sides

Now decide whether one DZ gives such a strong geometric advantage that it changes the normal preference for choosing turn order.

---

## 21. Turn-by-turn geometry

Terrain use changes over the game.

### Turn 1

Prioritize:

- safe development routes;
- attack lanes;
- retreat locations;
- denying enemy long-range access;
- occupying strong midfield corners.

### Turn 2

Terrain often becomes more open because:

- ARO pieces are dead;
- mines have detonated;
- doors/routes are cleared;
- midfield pieces have moved.

Re-evaluate the table rather than using the Turn 1 mental map.

### Turn 3

Objective access dominates.

A route that was strategically irrelevant early may become the most important route on the table because it reaches:

- console;
- zone;
- antenna;
- exclusion area;
- surviving enemy Specialist.

Preserve an efficient scoring route rather than occupying every attractive firing position.

---

## 22. Common geometry mistakes

### "This model is behind Cover"

Maybe, but is it actually touching the scenery required for Partial Cover?

### "These two AROs cover each other"

Can they be pie-sliced independently?

### "The TAG can fit through there"

Check the whole 55/70 mm base around every corner.

### "This rooftop is safe"

Safe from ground level, or safe from Super-Jump / Climbing Plus / another rooftop?

### "I'll just climb down later"

Calculate the Orders now.

### "They're spread out, so templates are fine"

Are they separated by hard geometry or merely by a few inches?

### "My Remote is fast"

Fast in a straight lane is not the same as fast through four dense corners.

### "Nobody can get into that room"

Can they shoot through the entrance? Climb the back wall? Jump to a window/roof? Template the doorway?

---

## 23. Compact geometry heuristics

- **Terrain is model-dependent.** Different silhouettes play on different maps.
- **Trace the base, not the centerline.** Large bases pay for tight corners.
- **Width and height are separate problems.** Wide models struggle to route; tall models struggle to hide.
- **Use narrow routes to exclude expensive large attackers.**
- **Touch terrain if you expect Partial Cover.**
- **Prone turns many parapets into Total Cover.**
- **A rooftop needs an exit plan.**
- **Treat ladders and stairs as roads.**
- **Treat Climbing Plus walls as roads too.**
- **Super-Jump makes empty air an attack lane.**
- **Crossfires must survive pie-slicing.**
- **Separate valuable models with walls/elevation, not merely distance.**
- **Plan a large attacker's parking position before its firing position.**
- **Look for geometry that prevents the opponent's best model from being the right tool.**

---

## Deployment geometry checklist

| Question | Desired answer |
|---|---|
| Can my S2 Specialists reach objectives efficiently? | Yes |
| Can my largest base leave the DZ cleanly? | Yes |
| Is there true Total Cover for expensive pieces? | Yes |
| Can key infantry finish Prone behind parapets? | Yes |
| Are important rooftops accessible and escapable? | Yes |
| Have I identified ladders and stairs? | Yes |
| Can a Super-Jump model see over my hiding terrain? | Ideally no |
| Can Climbing Plus bypass my guarded approaches? | Not into something valuable for free |
| Can the opponent pie-slice my AROs one at a time? | Not easily |
| Are valuable models separated by hard geometry from templates? | Yes |
| Is my TAG / S4 retreat route actually wide enough? | Yes |
| Does a narrow route exclude an enemy large attacker? | Exploit it |
| Does elevation distort my intended weapon range bands? | Checked |
| Is choosing the stronger DZ worth more than choosing turn order? | Explicitly evaluated |

## Compact doctrine

**Read the table in three dimensions -> trace routes by silhouette -> identify true hiding volumes -> test pie-slicing -> map vertical attack vectors -> plan both entry and retreat.**

The key terrain question is not simply **"Where can I get Cover?"**

It is:

> **Which models can physically reach which positions, what can they see from there, and what must they expose themselves to along the way?**

## Related notes

- [Defensive architecture / Reactive Turn](defensive-architecture-and-reactive-turn.md)
- [Deployables and area control](../deployables-area-control.md)
- [Movement, positioning and vision control](movement-positioning-and-vision-control.md)
- [Deployment, Initiative and Reserve strategy](deployment-initiative-and-reserve-strategy.md)
- [Target priority and attack sequencing](target-priority-and-attack-sequencing.md)
- [Probability and Face-to-Face decisions](probability-and-face-to-face-decision-framework.md)

## Rules / research reminders

- Use current N5/N5.3 wording for Prone, Climb, Climbing Plus, Super-Jump, movement measurement, silhouettes, and scenery access.
- Be cautious with older N5 videos/forum posts describing Climbing Plus movement because early N5 wording and later FAQ/update wording differ.
- Useful canonical repository references: [Silhouettes](../../rules/1_Basic%20Rules/Silhouettes.md), [Moving and Measuring](../../rules/2_Movement/Moving_and_Measuring.md), [Cover / Ballistic Skills](../../rules/3_Combat/Ballistic_Skills.md), [Climb](../../rules/2_Movement/Climb.md), [Climbing Plus](../../rules/5b_Special%20Skills/Climbing_Plus.md), [Super-Jump](../../rules/5b_Special%20Skills/Super-Jump.md), [Direct Template Weapons](../../rules/3_Combat/Direct_Template_Weapons.md), and [Scenery Structures](../../rules/7_Terrain,%20Scenery,%20Triumph,%20Table,%20Scenarios,%20ITS/Scenery_Structures.md).
- Useful competitive geometry principle: apparent overlapping AROs only matter if their placement prevents or meaningfully punishes sequential pie-slicing.
