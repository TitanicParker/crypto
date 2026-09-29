---
layout: page
title: Fixed Structure Research
---

<div class="kicker">Fixed Structure Research</div>

# The machine has a shape.

<p class="lede">The market establishes a logarithmic ladder once. We keep it fixed, watch price move through it, and test two separate ideas: whether the ladder can be traded mechanically, and whether the wider market reveals a smoother structural rhythm through the 100-period SMA.</p>

<div class="path-grid">
  <a class="path trade" href="TRADING.md">
    <span class="num">01</span>
    <span class="name">TRADE THE STRUCTURE</span>
    <span class="desc">The mechanical method. One decision level at a time.</span>
  </a>
  <a class="path market" href="MARKET.md">
    <span class="num">02</span>
    <span class="name">UNDERSTAND THE MARKET</span>
    <span class="desc">TOTAL, expansion, displacement and the 100 SMA.</span>
  </a>
  <a class="path evidence" href="OBSERVATIONS.md">
    <span class="num">03</span>
    <span class="name">SEE THE EVIDENCE</span>
    <span class="desc">Charts, measurements, failures and unresolved cases.</span>
  </a>
</div>

<figure class="instrument">
<svg viewBox="0 0 1100 560" role="img" aria-label="Fixed structural levels with volatile market movement and a smooth magenta 100 SMA">
  <rect width="1100" height="560" fill="#090a0d"/>
  <g font-family="monospace" font-size="18">
    <line x1="60" y1="70" x2="1040" y2="70" stroke="#fff" stroke-width="4"/>
    <text x="70" y="55" fill="#fff">WHITE · parent boundary</text>
    <line x1="60" y1="160" x2="1040" y2="160" stroke="#ffd400" stroke-width="2"/>
    <text x="70" y="145" fill="#ffd400">0.786 · YELLOW</text>
    <line x1="60" y1="240" x2="1040" y2="240" stroke="#2f7cff" stroke-width="2"/>
    <text x="70" y="225" fill="#2f7cff">0.618 · BLUE</text>
    <line x1="60" y1="320" x2="1040" y2="320" stroke="#2f7cff" stroke-width="2"/>
    <text x="70" y="305" fill="#2f7cff">0.500 · BLUE</text>
    <line x1="60" y1="400" x2="1040" y2="400" stroke="#2f7cff" stroke-width="2"/>
    <text x="70" y="385" fill="#2f7cff">0.382 · BLUE</text>
    <line x1="60" y1="480" x2="1040" y2="480" stroke="#ffd400" stroke-width="2"/>
    <text x="70" y="465" fill="#ffd400">0.236 · YELLOW</text>
  </g>
  <polyline points="90,450 145,410 200,455 250,350 310,390 365,285 430,330 485,260 540,305 600,210 655,250 710,185 770,215 835,150 905,190 980,120"
    fill="none" stroke="#f5f7fb" stroke-width="3" opacity=".85"/>
  <path d="M90 420 C220 400, 300 365, 420 330 S650 255, 760 240 S900 225, 1010 190"
    fill="none" stroke="#ff2aa3" stroke-width="8"/>
  <text x="790" y="275" fill="#ff2aa3" font-family="monospace" font-size="18">100 SMA</text>
  <text x="835" y="108" fill="#f5f7fb" font-family="monospace" font-size="18">market</text>
</svg>
<figcaption>The same visual grammar everywhere: white boundaries, blue structure, yellow decision bands, magenta 100 SMA.</figcaption>
</figure>

## One fixed foundation

The structural ladder is:

<div class="rule-line white"><span>1.000</span><i></i><span>WHITE</span></div>
<div class="rule-line yellow"><span>0.786</span><i></i><span>YELLOW</span></div>
<div class="rule-line"><span>0.618</span><i></i><span>BLUE</span></div>
<div class="rule-line"><span>0.500</span><i></i><span>BLUE</span></div>
<div class="rule-line"><span>0.382</span><i></i><span>BLUE</span></div>
<div class="rule-line yellow"><span>0.236</span><i></i><span>YELLOW</span></div>
<div class="rule-line white"><span>0.000</span><i></i><span>WHITE</span></div>

For exact parent values `A` and `B`:

```text
child(f) = A × (B/A)^f
```

The same geometry can recurse inside any interval.

> **Pan and zoom change the view, not the structure.**

[Learn the structure →](STRUCTURE.md)

Before either investigation, the structure can be reduced to a finite mathematical world: ordered levels, recursive children to a fixed depth, a local five-point decision corridor, finite machine states and explicit transition rules.

[Define the finite world →](FINITE_WORLD.md)

The primitive trading branch is now frozen as **Machine v0.1** and pre-registered as **Experiment 1**. Changes to its event grammar require a new machine version rather than rewriting the old test.

[Read Machine v0.1 →](MACHINE_SPEC.md) · [Open Experiment 1 →](EXPERIMENT_1.md)

## Two investigations. One evidence standard.

<div class="split">
  <div class="note trade">
    <span class="label trade">TRADING RULE</span>
    <p><strong>Every level is a decision.</strong><br>Next rung up or next rung down. Stops come from child structure, not arbitrary percentages.</p>
  </div>
  <div class="note market">
    <span class="label market">HYPOTHESIS</span>
    <p><strong>The candles are volatile. The average is smooth.</strong><br>We are studying whether that smooth path repeatedly organizes itself around the fixed structure.</p>
  </div>
</div>

Neither side gets to borrow proof from the other. A good trade does not prove the SMA hypothesis. A compelling TOTAL chart does not automatically change an execution rule.

## The evidence

Real chart images belong in `charts/` and should be shown before long commentary.

A serious evidence block is:

**chart → caption → observation → interpretation → status**

We keep successful examples, failures, counterexamples and unresolved cases.

[Open the research notebook →](OBSERVATIONS.md)
