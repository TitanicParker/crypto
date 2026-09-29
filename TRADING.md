---
layout: page
title: Trading Method
---

<div class="kicker">Side one · mechanical method</div>

# Every level is a decision.

<p class="lede"><strong>Next rung up or next rung down.</strong> The primitive trade is one adjacent structural move. Larger paths are built from successive decisions, not guessed destinations.</p>

<figure class="instrument">
<svg viewBox="0 0 1000 430" role="img" aria-label="Trading decision at a structural level with adjacent targets and local child-yellow stops">
  <rect width="1000" height="430" fill="#090a0d"/>
  <line x1="90" y1="70" x2="910" y2="70" stroke="#2f7cff" stroke-width="2"/>
  <line x1="90" y1="215" x2="910" y2="215" stroke="#fff" stroke-width="4"/>
  <line x1="90" y1="360" x2="910" y2="360" stroke="#2f7cff" stroke-width="2"/>
  <line x1="90" y1="165" x2="910" y2="165" stroke="#ffd400" stroke-width="2"/>
  <line x1="90" y1="265" x2="910" y2="265" stroke="#ffd400" stroke-width="2"/>
  <text x="105" y="55" fill="#2f7cff" font-family="monospace" font-size="18">adjacent target up</text>
  <text x="105" y="200" fill="#fff" font-family="monospace" font-size="18">current decision level</text>
  <text x="105" y="345" fill="#2f7cff" font-family="monospace" font-size="18">adjacent target down</text>
  <text x="650" y="155" fill="#ffd400" font-family="monospace" font-size="16">upper child-yellow</text>
  <text x="650" y="288" fill="#ffd400" font-family="monospace" font-size="16">lower child-yellow</text>
  <path d="M500 210 L500 100" stroke="#2f7cff" stroke-width="5"/>
  <polygon points="500,85 490,105 510,105" fill="#2f7cff"/>
  <path d="M545 220 L545 330" stroke="#f5f7fb" stroke-width="3" opacity=".7"/>
  <polygon points="545,345 535,325 555,325" fill="#f5f7fb"/>
</svg>
<figcaption>Parent decision in white. Adjacent targets in blue. Local child-yellow corridor in yellow.</figcaption>
</figure>

## The primitive trade

A one-level test asks one clean question:

> From a valid structural decision, which predefined boundary is reached first: the adjacent target or the structural stop?

That result can be measured historically without needing a story about what the market “should” do.

## Child structure is local structure

The parent ladder gives the larger decision. Recursive children give a tighter working corridor.

A child level can define local invalidation, a stop, a trailing stop, a smaller interval, or the point at which one directional hypothesis no longer survives.

The exact rule must be written before the path is scored.

## Flat is a real state

The method should not force exposure.

Flat can be correct when a decision is unresolved, both sides have been invalidated, the rule calls for no entry, or realistic execution costs make the theoretical trade unusable.

**Time spent flat is a measured result.**

## Both directions at one decision

Conceptually, one structural point can generate two competing hypotheses:

```text
long  → next rung up
short → next rung down
```

For historical reverse engineering, both can be scored independently.

Live execution is different. Depending on venue and account rules, implementation may require separate accounts, subaccounts, hedge mode, or a single-net-position rule.

That execution choice must never be confused with the geometry itself.

## Gross is not net

Keep three layers separate:

**Structural result** — which predefined target or stop was reached first?

**Gross trading result** — what did the price move produce before costs?

**Executable net result** — what remains after fees, spread, slippage, funding and account constraints?

A theoretical backtest is not a live trading record.

## Continuation is a separate test

One successful level-to-level move does not prove that the next level will follow.

A path can be compressed into adjacent crossings:

```text
0.382 ↑ 0.500 ↑ 0.618 ↓ 0.500 ↓ 0.382
```

That lets us ask whether continuation, reversal and structural region have measurable differences.

## What we eventually measure

- one-level target hit rate;
- child-stop hit rate;
- unresolved decisions;
- gross result;
- net result after realistic costs;
- time spent flat;
- differences by level type or structural region;
- whether a structural trailing rule improves or worsens continuation results.

The method begins as a rule set. Its effectiveness is an empirical question.

[See the canonical ladders →](ASSETS.md) · [Open the evidence →](OBSERVATIONS.md)
