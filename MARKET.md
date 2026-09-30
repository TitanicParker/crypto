---
layout: page
title: Understanding the Market
---

<div class="kicker">Side two · market condition</div>

# The candles are volatile. The average is smooth.

<p class="lede">The principal object here is <strong>TOTAL crypto market cap</strong>, its fixed structural ladder, and the slow path drawn by a roughly 100-day trailing average.</p>

<figure class="instrument">
<svg viewBox="0 0 1100 500" role="img" aria-label="Volatile TOTAL movement around fixed structure with a smooth magenta 100 SMA">
  <rect width="1100" height="500" fill="#090a0d"/>
  <line x1="60" y1="80" x2="1040" y2="80" stroke="#fff" stroke-width="4"/>
  <line x1="60" y1="170" x2="1040" y2="170" stroke="#ffd400" stroke-width="2"/>
  <line x1="60" y1="250" x2="1040" y2="250" stroke="#2f7cff" stroke-width="2"/>
  <line x1="60" y1="330" x2="1040" y2="330" stroke="#2f7cff" stroke-width="2"/>
  <line x1="60" y1="420" x2="1040" y2="420" stroke="#fff" stroke-width="4"/>
  <polyline points="80,390 130,355 180,410 230,290 280,330 330,240 380,295 430,210 485,255 540,190 600,245 660,175 720,205 780,150 840,210 900,165 960,185 1020,120"
    fill="none" stroke="#f5f7fb" stroke-width="3"/>
  <path d="M80 360 C180 350, 260 320, 360 300 S540 250, 650 230 S820 215, 900 210 S980 205, 1020 205"
    fill="none" stroke="#ff2aa3" stroke-width="9"/>
  <text x="800" y="245" fill="#ff2aa3" font-family="monospace" font-size="18">100 SMA</text>
</svg>
<figcaption>Price expands and contracts through the structure. The slower average records that activity as a smooth path.</figcaption>
</figure>

## Working hypothesis

> Nested expansion and contraction through a fixed logarithmic structure may generate a slow 100-day trajectory whose own path remains meaningfully organised by that structure.

This is a hypothesis, not a conclusion.

## Two things are happening

The visible market is constantly expanding and contracting.

A large expansion can be followed by a sustained contraction containing many smaller expansions and contractions. The same is true in reverse. The recursive structure gives those movements a fixed coordinate system at more than one scale.

At the same time, the same price history is continuously drawing the slower magenta curve.

The two views are related, but they are not the same measurement.

## Displacement and forcing

Let price and the slow average be expressed in the same structural coordinate system:

```text
p(t) = structural position of TOTAL
s(t) = structural position of the 100-day average
```

**Displacement**

```text
d(t) = p(t) - s(t)
```

describes where price is relative to the slow curve.

**100-day forcing**

```text
q100(t) = p(t) - p(t - 100 days)
```

describes the endpoint replacement pressure acting on that curve.

For a 100-day trailing mean:

```text
dM/dt = [P(t) - P(t - 100 days)] / 100 days
```

So the sign of the 100-day comparison determines whether the slow curve is being pulled upward or downward.

This is mechanical. It does not by itself prove anything about the Fibonacci structure.

## Expansion is not one thing

We do not use one word to hide several different measurements.

**Structural expansion / contraction** — movement away from or back toward a chosen structural center.

**Displacement expansion / contraction** — increasing or decreasing separation from the slow curve.

**Range expansion / contraction** — widening or narrowing of the recent structural range.

**Traversal** — movement through fixed recursive levels.

These can disagree at the same time. Price can be expanding through structure while contracting toward the SMA. A macro contraction can contain repeated micro-expansions and micro-contractions.

That nesting is part of the object under study.

## The slow curve

A 100-day average is expected to be smoother than price.

That smoothness is not evidence.

The question is whether the smooth path itself repeatedly occupies, turns around, crosses or travels between structural regions that were fixed independently of the later movement.

The market can remain violently active while the slow curve stays orderly because many shorter movements can cancel inside the rolling window.

## Cycle stage

The same local movement may mean different things in different parts of a larger cycle.

We therefore watch the relationship between:

```text
structural position
price/SMA displacement
100-day forcing
SMA slope
SMA curvature
multiscale expansion/contraction
```

The aim is not to assign a story after the event. It is to see whether those measurements are sufficient to distinguish recurring stages without moving the structure or changing the definitions.

## A useful historical case

The previous TOTAL cycle gives a white boundary at approximately:

```text
1.000 = $3.010T
```

using the previous-cycle low and high:

```text
0 = $0.728T
1 = $3.010T
```

The nearest recursive yellows around that white are approximately:

```text
lower yellow = $2.821T
white 1.000  = $3.010T
upper yellow = $3.297T
```

During the later 2024–2025 expansion, the daily 100 SMA appears to make an unusually smooth roll through this yellow-white-yellow region while price itself undergoes much larger expansion and contraction.

That is an observation to measure, not a conclusion.

## Primary representation

The **daily 100 SMA** remains the principal visual expression under study.

But the deeper mathematical question is now the approximately **100-day forcing horizon**.

Equivalent nominal horizons include:

```text
1D / SMA100
8h / SMA300
4D / SMA25
```

They are not numerically identical moving averages, but they share the same 100-day endpoint comparison when expressed per unit of calendar time.

A real 100-day phenomenon should preserve its broad geometry across those representations even if finer detail changes.

## What would make the idea interesting?

Not smoothness alone.

Stronger evidence would require some combination of:

- a structure fixed independently of the later event;
- a roll detected without using the structure to define it;
- similar macro geometry across 8h/300, 1D/100 and 4D/25;
- 100 days performing differently from nearby horizons;
- the observed structural corridor outperforming matched random corridors;
- repetition on later data without redefining the rules.

## TOTAL is weather

TOTAL can describe the broader condition in which assets are moving.

It does **not** automatically change an asset's fixed ladder, change an execution rule, or turn a market observation into a trade signal.

That separation keeps the two investigations independently testable.

## Observation before interpretation

<div class="split">
  <div class="note market">
    <span class="label market">OBSERVATION</span>
    <p>The daily 100 SMA crosses a previously defined structural region while TOTAL undergoes large expansion and contraction around it.</p>
  </div>
  <div class="note">
    <span class="label">INTERPRETATION</span>
    <p>The smooth trajectory may be organised by the fixed structure. That remains to be tested against matched alternatives.</p>
  </div>
</div>

The first statement can be measured. The second can be argued. They are not the same thing.

## What would count against the idea?

Keep examples where the SMA shows no stable relationship to fixed structure; where the apparent relationship disappears when exact parent boundaries are used; where convincing behaviour only appears after moving the structure; where nearby memory horizons perform just as well; where the macro roll is unstable across equivalent 100-day representations; where random matched corridors perform similarly; and where strong examples fail to repeat.

Negative examples are evidence too.

[Open the evidence →](OBSERVATIONS.md)
