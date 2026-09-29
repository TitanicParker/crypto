---
layout: page
title: Event Schema
---

<div class="kicker">Common evidence language</div>

# One schema for the whole project.

<p class="lede">Trading events and market-hypothesis observations share the same structural address. The schema keeps raw observation separate from interpretation and makes unresolved chronology explicit.</p>

## Core identity

```text
record_id
record_type
machine_version
asset
venue
instrument
timeframe
start_time
end_time
source_data
source_image
```

Suggested `record_type` values:

```text
trade_decision
market_spell
chart_observation
```

## Structural address

```text
parent_container_low
parent_container_high
decision_level
nearest_level
nearest_level_type
current_interval_low
current_interval_high
price
container_position
recursion_depth
```

## Trading-machine fields

Use for `trade_decision` records:

```text
lower_adjacent_parent
upper_adjacent_parent
lower_commitment_boundary
upper_commitment_boundary
entry_time
entry_price
initial_state
first_boundary_reached
first_boundary_time
surviving_hypothesis
survivor_target
survivor_failure_boundary
resolution
resolution_time
resolution_price
machine_state_final
event_duration_bars
rearm_time
gross_long_return
gross_short_return
gross_combined_return
net_return_0bps
net_return_5bps
net_return_10bps
net_return_20bps
funding_result
mae
mfe
chronology_status
```

Suggested categorical values:

```text
initial_state:
- BOTH_ACTIVE

first_boundary_reached:
- lower_commitment
- upper_commitment
- unresolved

surviving_hypothesis:
- up
- down
- unresolved

resolution:
- UP_TARGET
- UP_FAILURE
- DOWN_TARGET
- DOWN_FAILURE
- UNRESOLVED_COMMITMENT
- UNRESOLVED_SURVIVOR

chronology_status:
- resolved
- unresolved_same_bar
- unresolved_gap
- insufficient_data
```

## TOTAL / SMA market fields

Use for `market_spell` and relevant chart observations:

```text
sma100
sma_structural_position
sma_slope
sma_slope_state
price_parallelism
sma_parallelism
parallel_duration_bars
price_sma_distance
convergence_state
crossing_event
retest_event
step_count
reversal_count
container_exit_side
```

Suggested categorical values:

```text
sma_slope_state:
- rising
- falling
- near_horizontal

convergence_state:
- converging
- diverging
- neutral

container_exit_side:
- top
- bottom
- unresolved
```

## Observation and interpretation

Every record may also contain:

```text
observation
interpretation
predefined_test
measured_result
status
notes
```

Suggested status values:

```text
SUPPORTIVE
CONTRADICTORY
UNRESOLVED
DESCRIPTIVE_ONLY
```

The status is always local to the question being tested. It is never a verdict on the whole project.

## Rule

> **A field should describe what was measured, what the machine did, or what question was predefined. It should never encode the desired conclusion before the event is scored.**

[Machine v0.1 ->](MACHINE_SPEC.md) · [Evidence notebook ->](OBSERVATIONS.md)
