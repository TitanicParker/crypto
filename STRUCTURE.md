---
layout: page
title: Structure
---

# The fixed logarithmic structure

The market establishes the parent ladder once. After that, the structure is **not redrawn to fit later candles**.

The standard white-to-white container is:

```text
White
  ├─ 0.236  Yellow
  ├─ 0.382  Blue
  ├─ 0.500  Blue
  ├─ 0.618  Blue
  └─ 0.786  Yellow
White
```

Or, read as a ladder:

**White → Yellow → Blue → Blue → Blue → Yellow → White**

## Parent containers

Two neighbouring fixed parent levels form a **container**.

If the exact boundaries are `A` and `B`, the market can be described in two ways at once:

- its actual price or market-cap value;
- its normalized position inside `A → B`.

That second description gives the observation a **structural address**.

## Child levels

Inside exact parent boundaries `A` and `B`:

```text
child(f) = A × (B/A)^f
```

using:

```text
0.236, 0.382, 0.500, 0.618, 0.786
```

The same calculation can be repeated recursively inside any smaller interval.

### Example

If the current parent container is:

```text
110.51526 → 133.37416
```

then every child used inside that interval must be calculated from **those exact endpoints**.

Do not slide a child line because a candle cluster looks persuasive.

## Structural position

For a value `P` inside `A → B`:

```text
position = ln(P/A) / ln(B/A)
```

So:

| Position | Meaning |
|---:|---|
| 0.000 | container bottom |
| 0.236 | lower yellow |
| 0.382 | first blue |
| 0.500 | middle blue |
| 0.618 | upper blue |
| 0.786 | upper yellow |
| 1.000 | container top |

This makes very different nominal markets comparable without pretending that their prices are the same thing.

## Yellow-to-yellow working area

Around a parent level `L`, let `L-` be the neighbouring parent below and `L+` the neighbouring parent above.

The local corridor around `L` can be described by the child-yellow immediately below and above it:

```text
lower yellow = L- × (L/L-)^0.786
upper yellow = L  × (L+/L)^0.236
```

This creates a compact working area around the decision level without changing the parent structure.

## Structural address

A useful chart note should be able to say:

```text
asset
→ timeframe
→ parent container
→ current interval
→ actual market value
→ normalized container position
```

That is enough to locate an observation precisely in the system.

## Pan, zoom and overlays

The examination procedure is simple:

1. Identify asset and timeframe.
2. Read the visible time and value range.
3. Determine whether the chart axis is linear or logarithmic.
4. Locate the fixed parent levels in or immediately around the visible range.
5. Recalculate child levels from their exact parent boundaries.
6. Overlay them without fitting them to candles.
7. Locate the 100 SMA where relevant.
8. Record traversal, occupation, flattening, crossings, convergence, divergence and parallel spells.

> **Pan and zoom change the view, not the structure.**

## What a serious chart snapshot should show

- asset and timeframe;
- visible date range;
- parent container;
- visible structural levels;
- recalculated child levels where needed;
- current value;
- current structural interval;
- normalized position;
- 100 SMA value and slope where relevant;
- the event the image is intended to illustrate.

Next: **[Trading the structure →](TRADING.md)** or **[Understanding the market →](MARKET.md)**
