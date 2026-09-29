---
layout: page
title: Evidence
---

<div class="kicker">The evidence</div>

# Show the chart first.

<p class="lede">This is the living notebook. Real screenshots, fixed overlays, measurements, failures, counterexamples and unresolved cases belong here.</p>

A serious entry should read in this order:

**chart → caption → observation → interpretation → measured result → status**

Do not make the reader cross a wall of prose before seeing the evidence.

## Evidence block

<div class="evidence-block">
  <span class="label evidence">CHART</span>

  <p><code>charts/YYYY-MM-DD-asset-timeframe-short-description.png</code></p>

  <span class="label">CAPTION</span>

  <p><strong>ASSET · TIMEFRAME · DATE RANGE</strong><br>
  Parent container: <code>A → B</code> · Current interval: <code>…</code> · Value: <code>…</code> · Position: <code>…</code> · SMA100: <code>…</code></p>

  <span class="label">OBSERVATION</span>

  <p>State only what is visible or measured.</p>

  <span class="label">INTERPRETATION</span>

  <p>State what the observation might mean. This can remain blank.</p>

  <span class="label">MEASURED RESULT</span>

  <p>Only where a predefined trading or market test applies.</p>

  <span class="label">STATUS</span>

  <p class="status unresolved">UNRESOLVED</p>
</div>

## Chart standard

Where possible, an annotated chart should visibly identify asset, timeframe, date range, parent container, current interval, current value, normalized structural position, relevant child levels, SMA100 value, SMA slope state, and the event being illustrated.

Use the same colour language as the structure itself:

**white boundary · blue level · yellow 0.236/0.786 · magenta SMA100**

## Observation fields

Use only the fields that help the case:

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

The notebook does not need every field every time.

## Status language

<p class="status supportive">SUPPORTIVE</p>
<p class="status contradictory">CONTRADICTORY</p>
<p class="status unresolved">UNRESOLVED</p>
<p class="status">DESCRIPTIVE ONLY</p>

A status describes the observation's relationship to the current question. It is not a global verdict on the project.

## Keep the distinctions hard

**Observation** — what happened.

**Interpretation** — what it may mean.

**Hypothesis** — the broader proposition under test.

**Trading rule** — what the method said to do.

**Measured result** — how the predefined test scored.

A beautiful chart is not automatically proof. A profitable structural trade does not prove the SMA hypothesis.

## Add a new case

1. Save the original or annotated image in `charts/`.
2. Put the image first in the entry.
3. Add the short caption and structural address.
4. Record observation before interpretation.
5. Add the measured result only if a rule was defined in advance.
6. Leave unresolved cases unresolved.

New entries go at the top.
