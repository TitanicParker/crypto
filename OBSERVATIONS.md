---
layout: page
title: Observations
---

# Research notebook

This is the dynamic part of the project.

Add new entries at the top. Keep supportive, contradictory and unresolved examples. Do not rewrite old structural levels after seeing what happened next.

## Entry format

```markdown
## YYYY-MM-DD — ASSET — TIMEFRAME

![Short description](charts/YYYY-MM-DD-asset-timeframe-description.png)

**Side:** Trading / Market / Both  
**Parent container:** A → B  
**Current interval:** …  
**Market value:** …  
**Container position:** …  
**SMA100:** …  
**SMA slope:** rising / falling / near-horizontal / n.a.  
**Parallelism:** …  
**Convergence:** converging / diverging / neutral / n.a.  

### Observation
State only what is visible or measured.

### Interpretation
State what the observation might mean. This can remain blank.

### Trading rule / measured result
Only when relevant. Keep the predefined rule separate from the result.

### Status
Supportive / contradictory / unresolved / descriptive only.
```

---

## Example — market study

### 2026-09-29 — SOL — Daily

> *Illustrative record format only; replace the values below with a measured chart observation before treating it as evidence.*

**Side:** Market  
**Parent container:** `110.51526 → 133.37416`  
**Current interval:** to be measured  
**Market value:** to be measured  
**Container position:** to be calculated from the exact value  
**SMA100:** to be measured  
**SMA slope:** to be measured  
**Parallelism:** to be assessed over a defined spell  
**Convergence:** to be measured

#### Observation

No research conclusion is recorded until a source chart and measured values are attached.

#### Interpretation

Unresolved.

#### Status

**Template / not evidence.**

---

## Example — trading study

### YYYY-MM-DD — ASSET — TIMEFRAME — structural decision

**Side:** Trading  
**Decision level:** …  
**Adjacent target up:** …  
**Adjacent target down:** …  
**Long stop rule:** …  
**Short stop rule:** …  
**Costs model:** …

#### Trading rule

Write the exact rule that was being tested before scoring the path.

#### Observation

Record the sequence of structural crossings, for example:

```text
0.382 ↑ 0.500 ↑ 0.618 ↓ 0.500
```

#### Measured result

Record target/stop ordering, gross result, cost assumptions and net result separately.

#### Interpretation

Optional. Do not use interpretation to alter the measured result.

---

## Chart file naming

Keep it plain:

```text
charts/YYYY-MM-DD-asset-timeframe-short-description.png
```

Examples:

```text
charts/2026-09-29-total-1d-sma-flattening.png
charts/2026-09-29-sol-4h-parent-crossing.png
charts/2021-05-19-btc-1d-counterexample.png
```

A chart caption should identify:

- asset;
- timeframe;
- date;
- parent container;
- current interval;
- market value;
- SMA100 where relevant;
- what the image is meant to illustrate.

## Descriptive fields we may record

Use only what helps the observation:

```text
asset
timeframe
start_time
end_time
parent_container_low
parent_container_high
nearest_level
nearest_level_type
price
container_position
sma100
sma_slope_state
price_parallelism
sma_parallelism
parallel_duration_bars
convergence_state
crossing_event
retest_event
step_count
reversal_count
container_exit_side
source_image
notes
```

The notebook is not required to fill every field every time.
