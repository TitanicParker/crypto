---
layout: page
title: Finite Mathematical World
---

<div class="kicker">Formal world</div>

# A finite world of maths.

<p class="lede">Before asking whether the method is profitable, define the world in which the machine exists. The geometry is fixed, the relevant state space is finite once recursion depth is fixed, and market history supplies the realised path through that world.</p>

## 1. Structural universe

Let the fixed parent ladder be an ordered finite set:

```text
L = {L0, L1, ..., Ln}
with L0 < L1 < ... < Ln
```

Every neighbouring pair:

```text
[Li, Li+1]
```

is a parent container.

The levels do not move to fit later price action.

## 2. Structural position

For a value `P` inside exact container boundaries `A < B`:

```text
x(P; A,B) = ln(P/A) / ln(B/A)
```

So:

```text
x = 0   -> container bottom
x = 1   -> container top
```

and the canonical internal addresses are:

```text
0.236, 0.382, 0.500, 0.618, 0.786
```

Every observation can therefore have two coordinates:

```text
(actual value, structural address)
```

## 3. Recursive geometry

For exact boundaries `A < B`:

```text
child(f) = A * (B/A)^f
```

for:

```text
f in {0.236, 0.382, 0.500, 0.618, 0.786}
```

The geometry can recurse indefinitely in principle.

The trading experiment cannot.

To make the machine finite, choose a maximum recursion depth `d` in advance. The complete testable structural universe is then the set of all levels generated up to depth `d`.

## 4. The local five-point decision world

Take an eligible parent decision level `Li`, with adjacent parents `Li-` below and `Li+` above.

Define the local child-yellow boundaries:

```text
Ci- = Li- * (Li / Li-)^0.786
Ci+ = Li  * (Li+ / Li)^0.236
```

Then the irreducible local geometry is:

```text
Li- < Ci- < Li < Ci+ < Li+
```

This five-point object is the mathematical atom of the primitive trading method.

## 5. Two directional propositions

At `Li` define:

```text
H+ : Li -> Li+
H- : Li -> Li-
```

with:

```text
H+ invalidated at Ci-
H- invalidated at Ci+
```

The method is therefore not required to predict an entire trend.

It asks one local question:

> **Which directional proposition survives the local decision corridor?**

## 6. Price path becomes structural events

Let market value be a time-indexed path:

```text
P(t)
```

The machine does not need a story about why `P(t)` moves.

It reduces the continuous path to an ordered sequence of structural events, for example:

```text
Li -> Ci+ -> Li+
Li -> Ci- -> Li-
Li -> Ci+ -> Li -> Ci-
```

Continuous price therefore becomes a symbolic path through a finite set of relevant boundaries.

## 7. Finite machine states

A minimal state set is:

```text
S = {
  FLAT,
  BOTH_ACTIVE,
  UP_SURVIVES,
  DOWN_SURVIVES,
  UP_COMPLETE,
  DOWN_COMPLETE,
  UNRESOLVED
}
```

`UNRESOLVED` is a legitimate historical state when available data cannot determine event ordering.

The machine is allowed to say: **the path cannot be known from this data**.

## 8. Transition law

Let `E` be the finite set of admissible structural events.

The machine is a transition function:

```text
T : S x E -> S
```

Primitive transitions include:

```text
FLAT + valid arrival at Li        -> BOTH_ACTIVE

BOTH_ACTIVE + first valid hit Ci+ -> UP_SURVIVES
BOTH_ACTIVE + first valid hit Ci- -> DOWN_SURVIVES

UP_SURVIVES + hit Li+             -> UP_COMPLETE
DOWN_SURVIVES + hit Li-           -> DOWN_COMPLETE

UP_COMPLETE   -> FLAT
DOWN_COMPLETE -> FLAT
```

If event chronology cannot be established:

```text
state + ambiguous ordering -> UNRESOLVED
```

The exact definitions of arrival, hit, crossing, reset and re-entry must be frozen before scoring history.

## 9. Information state

At any moment the machine needs only a compact structural state, for example:

```text
Q(t) = (container, recursion_depth, structural_position, machine_state)
```

It does not require a narrative about the market.

It requires:

```text
where are we?
what state are we in?
what structural event happens next?
```

## 10. Time is a separate variable

The same structural path can happen quickly or slowly.

For structural event times:

```text
t0, t1, t2, ...
```

define:

```text
duration = t(k+1) - t(k)
```

and, if useful later:

```text
structural_rate = change_in_structural_position / duration
```

Rate can therefore be measured without changing the primitive geometry or directional rules.

The first trading test should not need a rate filter.

## 11. Three layers that must not be confused

### Geometry

Purely defined mathematics:

```text
levels
containers
children
structural position
local corridor
```

### Machine

A deterministic rule system over structural events:

```text
states
events
transitions
completion
flat
unresolved
```

### Empirical distribution

What actual market history does inside the machine:

```text
which child-yellow is reached first?
does the survivor reach the adjacent parent?
how long does traversal take?
what is the result after costs?
```

The first two layers are constructed.

The third is measured.

## 12. TOTAL and the 100 SMA live in the same world

TOTAL and its 100-period SMA can be assigned the same structural address:

```text
xTOTAL(t) = ln(TOTAL(t)/A) / ln(B/A)

xSMA(t)   = ln(SMA100(t)/A) / ln(B/A)
```

The market hypothesis then studies trajectories inside the same fixed coordinate system:

- displacement;
- convergence;
- divergence;
- crossings;
- retests;
- flattening;
- sustained near-horizontal spells;
- structural location of those spells.

This does not make TOTAL an execution rule.

The trading machine and the SMA hypothesis share geometry, not proof.

## 13. Compact definition

> **The Fixed Structural World is a finite-depth logarithmic hierarchy of ordered levels. A market path moves through that hierarchy and is observed as a sequence of structural events. At any eligible decision level, the trading machine occupies one state from a finite state set and changes state according to predefined boundary events. The geometry determines the possible states and boundaries; market history determines the realised sequence of transitions.**

In compact form:

```text
fixed geometry
+ moving market
+ finite states
+ transition rules
= the machine
```

## What this definition does not claim

It does not claim profitability.

It does not claim that the structural ladder predicts direction.

It does not claim that the TOTAL / 100-SMA hypothesis is proven.

It defines the world clearly enough that those empirical questions can be tested without changing the world after seeing the answers.

[Back to the structure ->](STRUCTURE.md) · [Enter the trading machine ->](TRADING.md) · [Understand the market ->](MARKET.md)
