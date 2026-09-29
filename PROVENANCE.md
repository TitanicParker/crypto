---
layout: page
title: Structural Provenance
---

<div class="kicker">Research integrity</div>

# When did the map become fixed?

<p class="lede">A fixed ladder can be studied retrospectively, but an ex-ante trading claim requires proof that the ladder and machine rules were already frozen before the simulated decision.</p>

## Rule

For every canonical asset ladder, preserve:

```text
asset
ladder_version
freeze_date
source_or_origin
first_public_commit
notes
```

Do not infer missing dates.

Until provenance is established, classify historical work as:

```text
fixed_ladder_traversal_study
```

rather than:

```text
ex_ante_backtest
```

## Current register

```text
BTC/USDT  freeze_date: TO ESTABLISH
ETH/USDT  freeze_date: TO ESTABLISH
SOL/USDT  freeze_date: TO ESTABLISH
TAO/USDT  freeze_date: TO ESTABLISH
TEL/USDT  freeze_date: TO ESTABLISH
ADA/USDT  freeze_date: TO ESTABLISH
AAVE/USDT freeze_date: TO ESTABLISH
ALGO/USDT freeze_date: TO ESTABLISH
TOTAL     freeze_date: TO ESTABLISH
```

The absence of a provenance date is not evidence against the structure. It only limits what kind of historical claim can honestly be made.

[Canonical ladders ->](ASSETS.md) · [Experiment 1 ->](EXPERIMENT_1.md)
