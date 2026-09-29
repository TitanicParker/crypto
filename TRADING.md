---
layout: page
title: Trading Method
---

# Side One — trading the structure

This side asks a deliberately testable question:

> **Can the fixed structural ladder be traded mechanically enough to survive historical measurement and realistic costs?**

It does not begin by assuming the answer is yes.

## The primitive idea: adjacent level to adjacent level

A structural level is a decision point.

At the simplest level, the next meaningful destination is not an arbitrary percentage target. It is the **adjacent structural rung**.

```text
rung below ← current decision level → rung above
```

The smallest complete structural trade is therefore a **one-level trade**.

If movement continues, a larger trend can be represented as a sequence of adjacent rung crossings rather than as one forecast made at the beginning.

## Flat is a position

The method should not force constant exposure.

Being flat can be the correct state when:

- a structural decision has not resolved;
- both directional ideas have been invalidated;
- the market is inside a working area without a defined rule-based entry;
- costs or execution conditions make the theoretical trade unattractive;
- the research rule being tested explicitly calls for no position.

Time spent flat is therefore something to **measure**, not something to hide.

## Parent level and local working area

A parent level can be surrounded by its local yellow-to-yellow corridor. This gives the trade a smaller decision area while leaving the parent ladder untouched.

Conceptually:

```text
lower child-yellow
        │
        │   working area
        │
parent decision level
        │
        │   working area
        │
upper child-yellow
```

The child yellows are mathematical consequences of the exact neighbouring parent bounds, not hand-fitted stop lines.

## Natural child-level stops

A simple research rule can use the relevant child level as an invalidation point for one side of a structural decision.

For example, if a level is being tested in both directions, movement far enough into one side's child structure may remove the opposite hypothesis before the adjacent parent target is reached.

Exactly which child constitutes a valid stop is a **trading rule** and must be written down before historical results are counted.

## Structural trailing stops

A continuation can be treated as a path through successive levels.

Once a new structural rung is crossed and accepted, a trailing stop can migrate according to a predefined structural rule instead of an arbitrary price distance.

The important research discipline is the same: define the migration rule before scoring the result.

## One-level trade versus continuation

These are different tests.

### One-level test

Ask only:

> From a valid decision, was the adjacent target reached before the specified structural stop?

### Continuation test

Ask:

> After one adjacent level was reached, did the same directional move continue through further structural rungs under a predefined trailing rule?

A continuation winner must not be allowed to retrospectively rescue a failed one-level rule.

## Recording structural paths

A market path can be compressed into adjacent structural crossings.

For example:

```text
0.382 ↑ 0.500 ↑ 0.618 ↓ 0.500 ↓ 0.382
```

That representation allows later questions such as:

- How often does a crossing continue one more rung?
- How often does it reverse immediately?
- Do yellow, blue and white levels behave differently?
- Does path behaviour differ by parent container?

## The awkward practical question: both directions at one decision point

The conceptual rule can treat the decision point as two competing directional hypotheses:

```text
long hypothesis  → next rung up
short hypothesis → next rung down
```

That does **not** mean every exchange account can literally hold both positions at once.

### Conceptual rule

For historical research, both hypothetical positions can be opened from the same structural decision and scored independently until their predefined target or stop is hit.

This answers a clean research question without pretending an exchange executed the trades.

### Possible live implementations

Depending on venue and account rules, a trader might use:

- separate accounts;
- subaccounts;
- hedge mode where the venue supports simultaneous long and short positions;
- one live position plus a separately tracked hypothetical opposite side;
- a single net-position rule that chooses one side, provided that selection rule is explicitly defined and tested separately.

These are **execution implementations**, not changes to the structural geometry.

### Exchange and account limitations

Actual execution can differ because of:

- whether hedge mode exists;
- margin mode and collateral rules;
- minimum order sizes;
- leverage constraints;
- liquidation mechanics;
- funding;
- venue-specific fees;
- spread and slippage;
- market availability and data quality.

A theoretical backtest that ignores these is not the same thing as an executable live strategy.

## Gross result is not net result

Historical reverse engineering should keep at least three layers separate:

1. **Structural result** — which target or stop was reached first?
2. **Gross trading result** — what would the price move have produced before costs?
3. **Executable net result** — what remains after realistic fees, spread, slippage, funding and account constraints?

Do not collapse those into a single number.

## Questions the research should eventually answer

- If every valid structural decision had been traded, what happened?
- How many one-level targets were reached?
- How often did the child-yellow stop remove one side?
- How many decisions ended with neither side cleanly resolved?
- What was the gross result?
- What remained after realistic costs?
- How much time was spent flat?
- Did yellow, blue and white decisions behave differently?
- Were particular structural regions materially different?
- Did multi-level continuation add value after the one-level test was already satisfied?

## What belongs in an observation

Keep four things distinct:

**Trading rule** — what the method said to do.  
**Observation** — what price actually did.  
**Measured result** — how the predefined test scored it.  
**Interpretation** — what we think the result may mean.

That separation is the foundation of the eventual historical study.

Next: **[See the canonical asset ladders →](ASSETS.md)**
