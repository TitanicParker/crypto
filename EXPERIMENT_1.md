---
layout: page
title: Experiment 1
---

<div class="kicker">Primitive machine test</div>

# Experiment 1: adjacent structural resolution.

<p class="lede">This is the smallest credible test of Machine v0.1. No TOTAL filter, no SMA filter, no rate filter, no continuation and no optimization.</p>

## Question

> **When the fixed machine is applied repeatedly to historical price, what structural outcomes occur and what is the complete two-hypothesis expectancy after friction?**

## Pre-registration

Experiment 1 uses:

```text
Machine version: 0.1
Assets: BTC/USDT, ETH/USDT, SOL/USDT
Underlying event data: 1-minute OHLCV where available
Recursion depth: 1
Continuation: off
Trailing: off
TOTAL filter: off
SMA filter: off
Rate filter: off
Level optimization: prohibited
```

## Structural inputs

Use only the canonical parent ladders already published in `ASSETS.md`.

For every eligible internal parent level `Li`:

```text
Li-
Ci-
Li
Ci+
Li+
```

are calculated before the event is scored.

## Event generation

For every armed decision level:

1. first valid touch of `Li` starts one event;
2. instantiate the two virtual hypotheses;
3. observe which child-yellow boundary is reached first;
4. invalidate one hypothesis;
5. score whether the survivor reaches its adjacent parent target or opposite failure boundary first;
6. if chronology is unknowable from the data, record an unresolved outcome;
7. return to flat;
8. rearm only according to Machine v0.1.

No chart may be excluded because the path looks unattractive.

## Required outputs

### Integrity

```text
number_of_decision_events
resolved_events
unresolved_commitments
unresolved_survivors
unresolved_fraction
```

### Direction discovery

```text
upper_commitment_first
lower_commitment_first
up_survivors
down_survivors
```

### Survivor outcome

```text
UP_TARGET
UP_FAILURE
DOWN_TARGET
DOWN_FAILURE
survivor_target_rate
```

### Economics

```text
gross_long_return
gross_short_return
gross_combined_return
net_0bps
net_5bps
net_10bps
net_20bps
funding_result_or_not_modelled
average_event_return
median_event_return
outcome_distribution
MAE
MFE
```

### Time

```text
event_duration
time_flat
time_both_active
time_directionally_exposed
flat_fraction
discovery_fraction
directional_exposure_fraction
```

### Stratification

Report without changing the rules:

```text
by_asset
by_decision_level_type
by_transition_type
by_parent_container
by_direction
```

## Primary falsification condition

The primitive trading method is practically weakened if the complete two-hypothesis process has non-positive net expectancy across reasonable friction assumptions, or if apparent performance depends heavily on unresolved chronology.

That result would not by itself falsify the fixed structural ladder.

## Secondary questions

After the baseline is complete, but not before:

1. Does recursion depth 2 improve information after additional friction?
2. Does a structural trailing rule improve continuation?
3. Does rate condition outcomes?
4. Do boundary classes behave differently?
5. Does contemporaneous TOTAL state alter the already-defined outcome distribution?

Those are later experiments, not modifications to Experiment 1.

## Provenance condition

For each asset, record when its canonical ladder was established.

Historical periods before that freeze date can still be used for a **fixed-ladder traversal study**, but they must not be presented as an ex-ante trading backtest unless the ladder was genuinely available at the simulated decision time.

[Machine v0.1 ->](MACHINE_SPEC.md) · [Canonical ladders ->](ASSETS.md) · [Event schema ->](EVENT_SCHEMA.md)
