# Collection-completion planning baseline — 2026-10-31

**User-directed scenario for future unique-unit buy-list comparisons.** This is a **planning coverage overlay**, not a physical inventory audit or proof of a completed transaction. The six recorded `inventory/*.md` files remain authoritative for individual sculpts and confirmed quantities. Apply this overlay when the user requests *remaining units to acquire*; do not silently rewrite the underlying inventory as though every missing unit was physically purchased.

## Collections treated as complete for unique-unit shopping

The user directs that all **distinct useful unit types** in the following six current N5.3 rosters are considered satisfied, through some combination of purchased models and accepted proxies:

- Caledonian Highlander Army (Caledonia)
- Military Orders
- Kestrel Colonial Force
- Tartary Army Corps (TAK)
- Steel Phalanx
- Shindenbutai

For these six collections, **remaining unique-unit acquisition gap = 0** under the user's stated proxy rules. This does **not** assert all AVA limits can be fielded simultaneously, every distinct weapon sculpt exists, or every ancillary model is confirmed. It does not change Army legality.

## New items considered acquired in this scenario

Treat at least **one unit-type representation** of each below as already obtained when calculating further PanO purchases:

| Unit | Counts as covered in relevant N5.3 rosters | Scope |
|---|---|---|
| Swiss Guard | Swiss Guard | One unit type, number of miniatures unspecified |
| Kamau | Kamau Amphibious Intervention Teams | One unit type, number of miniatures unspecified |
| Bolt Paramedic | Neoterra Bolts | One Bolt trooper, Paramedic profile |
| Cutter | Cutter TAG | One unit type, number of miniatures unspecified |
| Helots / Helot Militia | Helot Militia | At least one unit type; model quantity unspecified |

These are user-provided **"consider bought" assumptions**, not independently verified physical counts. The saved main-branch inventory snapshots may still report zero dedicated models; this overlay supersedes those *for planning counts only*. When the user subsequently confirms physical ownership and quantities, reconcile the relevant inventory files.

## Explicit proxy coverage

In addition to the six completed collections, count the following **unit types as satisfied via proxy** in every roster where they are genuinely legal:

- Acontecimento Regulars — existing PanO light infantry proxies, per the SAA buy list.
- ORC Troops — existing appropriate heavy infantry proxies in SAA/Varuna and other legal PanO rosters.
- Dart, Optimate Huntress — existing appropriate S2 skirmisher proxy; check whether an S3 Sharvara is needed for a selected profile.
- Fusiliers — existing Fennec Fusiliers or other appropriate S2 LI models, without pretending the donor is an official standard Fusilier miniature.
- Sāchā Xenotech Hunters — proxied where roster-legal.
- Kazurabā Ruby Monday — proxied where roster-legal.

Sāchā and Ruby Monday are **not** ordinary Acontecimento roster entries; their stated proxy status applies to other eligible rosters. Fusiliers are not a separate Acontecimento roster entry under the pinned N5.3 reference.

## Immediate net gaps for the two PanO proxy-first armies

Baseline from `sectorials/panoceania/shock-army-of-acontecimento.md`, `sectorials/panoceania/varuna-immediate-reaction-division.md`, their buy lists and the original 2026-10-30/31 inventory. One model of each *unique* roster unit; exclude ordinary four REM roles, servant peripherals and whole-unit hard avoids; retain special support/pilot/TAG choices unless covered.

### Acontecimento — 7 still uncovered unit types

1. Bagh-Mari Unit
2. Kirpal Singh
3. Lt. Stephen Rao
4. Akalis
5. Guarda de Assalto
6. Flight Officer Agnes Ferreira
7. Dragões

Covered by the new explicit proxy assumptions: Regulars, ORC Troops, Dart. The Acontecimento buy list independently says **proxy-only / CAD 0 dedicated purchase plan**. All seven are therefore *uncovered unit identities* in this particular count, **not** an instruction to buy seven boxes; other suitable proxies may be assigned later.

### Varuna — 5 still uncovered unit types

1. Croc Men
2. Echo-Bravo Rapid Reaction Unit
3. Patsy Garnett
4. Zulu-Cobra
5. Captain Uma Sørensen

Now covered by user assumptions: Kamau, Cutter, Helot Militia (considered acquired); ORC Troops and Fusiliers (proxy); Richard Quinn (Kestrel completion overlay). Varuna's earlier buy list explicitly says **proxy-only / CAD 0 dedicated purchase plan**. Its five gaps do not override that no-purchase decision.

## Method and guardrails

- **Acquisition gap**, not absolute physical ownership. A unit-type covered by an accepted proxy counts as met in this planning layer.
- Exclude ordinary four fire-support REM chassis and servant peripheral bots. Generic baggage/EVO or specialized named REMs may still count unless explicitly proxied or covered by a completed collection.
- Ignore optional Spec-Ops/Team-Ops, reinforcements and model quantities above one per unit type.
- Do not mistake disliked loadouts for wholesale avoid-rated units.
- If an owned or assumed model is used for several different unit identities, only assume proxy reuse across *different army lists* unless there are enough distinct physical models to field them together.
- Apply the latest main-branch Army roster and explicit user statements before older hypothetical buy-list wording.
