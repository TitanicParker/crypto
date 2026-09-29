---
layout: page
title: Structure
---

<div class="kicker">Common foundation</div>

# The structure does not move.

<p class="lede">The market establishes the parent ladder once. After that, we can zoom, recurse and measure — but we do not redraw the ladder to fit later price action.</p>

## The parent container

<div class="rule-line white"><span>1.000</span><i></i><span>WHITE</span></div>
<div class="rule-line yellow"><span>0.786</span><i></i><span>YELLOW</span></div>
<div class="rule-line"><span>0.618</span><i></i><span>BLUE</span></div>
<div class="rule-line"><span>0.500</span><i></i><span>BLUE</span></div>
<div class="rule-line"><span>0.382</span><i></i><span>BLUE</span></div>
<div class="rule-line yellow"><span>0.236</span><i></i><span>YELLOW</span></div>
<div class="rule-line white"><span>0.000</span><i></i><span>WHITE</span></div>

Two exact neighbouring parent values form a **container**.

Inside exact boundaries `A` and `B`:

```text
child(f) = A × (B/A)^f
```

with:

```text
0.236, 0.382, 0.500, 0.618, 0.786
```

The same rule can be repeated recursively inside any smaller interval.

## Structural position

A market value can be recorded both as a real number and as an address inside its container:

```text
position = ln(price/A) / ln(B/A)
```

<figure class="instrument">
<svg viewBox="0 0 1000 260" role="img" aria-label="A price and SMA located inside a structural container">
  <rect width="1000" height="260" fill="#090a0d"/>
  <line x1="70" y1="45" x2="930" y2="45" stroke="#fff" stroke-width="4"/>
  <line x1="70" y1="105" x2="930" y2="105" stroke="#2f7cff" stroke-width="2"/>
  <line x1="70" y1="165" x2="930" y2="165" stroke="#2f7cff" stroke-width="2"/>
  <line x1="70" y1="225" x2="930" y2="225" stroke="#fff" stroke-width="4"/>
  <circle cx="610" cy="145" r="8" fill="#fff"/>
  <circle cx="690" cy="125" r="9" fill="#ff2aa3"/>
  <text x="625" y="150" fill="#fff" font-family="monospace" font-size="17">price · position 0.57</text>
  <text x="705" y="120" fill="#ff2aa3" font-family="monospace" font-size="17">SMA100</text>
</svg>
<figcaption>A structural address says where the market is, not just what it costs.</figcaption>
</figure>

## Local working corridor

Around a parent level `L`, let `L-` be the parent below and `L+` the parent above.

```text
lower child-yellow = L- × (L/L-)^0.786
upper child-yellow = L × (L+/L)^0.236
```

Those child-yellow levels define a compact local corridor around the parent decision.

They are calculated. They are not hand-fitted.

## How to inspect any chart

1. Identify asset and timeframe.
2. Read the visible time and value range.
3. Locate the fixed parent levels in or around that range.
4. Recalculate children from exact parent boundaries.
5. Overlay them without fitting to candles.
6. Locate price and the 100 SMA where relevant.
7. Record traversal, occupation, flattening, crossings, convergence, divergence and parallel spells.

> **Pan and zoom change the view, not the structure.**

## Minimum structural address

```text
asset
→ timeframe
→ parent container
→ current interval
→ actual value
→ normalized position
```

That address is shared by both sides of the project.

[Define the finite mathematical world →](FINITE_WORLD.md) · [Trade the structure →](TRADING.md) · [Understand the market →](MARKET.md)
