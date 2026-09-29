---
layout: page
title: Fixed Structure Research
---

# Trade the structure. Understand the market.

This is a living illustrated notebook about a fixed logarithmic market structure.

There are **two questions**.

<div class="hero-grid">
  <div class="card">
    <h3>Trade the structure</h3>
    <p>Decision level → adjacent rung → predefined stop → measured result.</p>
  </div>
  <div class="card">
    <h3>Understand the market</h3>
    <p>TOTAL → fixed structure → 100 SMA → expansion, contraction and parallel spells.</p>
  </div>
</div>

## 1. Can fixed market structure be traded mechanically?

The trading side treats every structural level as a decision point: **next rung up or next rung down**. The primitive trade is one adjacent level. Larger moves are built from successive structural crossings rather than guessed targets.

[**Learn the trading method →**](TRADING.md)

## 2. Does the wider market reveal another rhythm through the 100 SMA?

The market-research side studies **TOTAL crypto market cap** against its own fixed structure, with special attention to the **daily 100-period simple moving average**. We are looking for expansion, contraction, displacement, convergence, crossings, flattening and sustained periods in which price or the SMA becomes approximately parallel to the structural levels.

[**Explore the market hypothesis →**](MARKET.md)

<div class="weather" aria-label="Schematic showing market movement and a flatter 100 SMA across fixed horizontal levels">
  <div class="level one"></div>
  <div class="level two"></div>
  <div class="level three"></div>
  <div class="market"></div>
  <div class="sma"></div>
  <div class="label">Schematic only: volatile market movement smoothed into a flatter 100 SMA against fixed horizontal structure.</div>
</div>

---

## One common foundation

Both investigations use the same fixed geometry:

<div class="ladder" aria-label="Fixed structural ladder">
  <div class="rung white"><span>0.000</span><span>White</span></div>
  <div class="rung yellow"><span>0.236</span><span>Yellow</span></div>
  <div class="rung blue"><span>0.382</span><span>Blue</span></div>
  <div class="rung blue"><span>0.500</span><span>Blue</span></div>
  <div class="rung blue"><span>0.618</span><span>Blue</span></div>
  <div class="rung yellow"><span>0.786</span><span>Yellow</span></div>
  <div class="rung white"><span>1.000</span><span>White</span></div>
</div>

| Fraction | Level |
|---:|---|
| 0.236 | Yellow |
| 0.382 | Blue |
| 0.500 | Blue |
| 0.618 | Blue |
| 0.786 | Yellow |

For exact parent values `A` and `B`:

```text
child(f) = A × (B/A)^f
```

where `f` is `0.236, 0.382, 0.500, 0.618, 0.786`.

A market value can also be given a structural address:

```text
position = ln(price/A) / ln(B/A)
```

The original parent levels are invariant.

> **Pan and zoom change the view, not the structure.**

[**Learn the structure →**](STRUCTURE.md)

---

## How to read this project

A simple route through the material is:

**Structure → Containers → Recursion → Trading → TOTAL → 100 SMA → Observations → Evidence**

The conceptual pages should change slowly. The notebook should change often.

A striking chart is not automatically evidence of a profitable trading rule. A profitable structural trade does not prove the SMA hypothesis. TOTAL is market weather, not an automatic trade trigger.

[**See the evidence →**](OBSERVATIONS.md)

---

## Visual evidence

Chart images live in [`charts/`](charts/). A useful sequence is:

**Original chart → structural overlay → annotation → short observation**

Each image should say what it is showing rather than forcing the reader to reverse-engineer the point from the picture.

### Suggested chart caption

> **SOL · Daily · 29 Sep 2026**  
> Container: `110.51526 → 133.37416` · Price: `…` · SMA100: `…`  
> *Purpose: show a near-horizontal SMA spell inside a fixed parent container.*

---

## Research rule

The project begins with no assumption that either investigation works.

We keep supportive examples, failures, anomalies and unresolved cases. New evidence may change our understanding, but it must not silently move old structural levels to make the theory look better.
