<!--
SPDX-FileCopyrightText: 2026 Paul Bunch
SPDX-License-Identifier: CERN-OHL-P-2.0
-->

# Finger Motion Zones and Layout Design Principles

> [Читать на русском](ergonomics.ru.md)

These notes are based on the analysis of the [finger motion map](../cad/ergonomics/finger-zones.dxf). The study was conducted for the left hand. Each finger’s reach zone was recorded while the other four fingers remained stationary (simulating a normal typing posture).

![Left hand resting positions](../docs/img/hand-positions--297x209mm.jpg)
*Fig. 1. Left-hand resting positions*

![Finger motion zones](../docs/img/finger-zones--297x209mm.jpg)
*Fig. 2. Finger trajectories and reach zones with a stationary palm*

## Key Observations and Principles

### 1. Vertical Zoning (Column Stagger)

* **Bottom row:** When the four non-thumb fingers move downward, their horizontal reach narrows.
  * *Conclusion:* It is advisable to place only one key per finger on the bottom row.

* **Home and upper rows:** Horizontal reach expands in these rows.
  * *Conclusion:* For the index finger and especially the pinky (which has the largest zone), two keys per row are practical (additional inner/outer columns).

### 2. Thumb Cluster

* The thumb has the largest motion zone — comparable in area to the combined zones of the other four fingers.
* The portion of the zone that lies under the palm remains reachable, but is most comfortable when the hand is slightly elevated.
  * *Conclusion:* The zone size justifies exploring two rows of keys in the thumb cluster.
  * *Caveat:* Two keys **in the same column** under the thumb are often awkward in practice: the thumb bends unnaturally, and accidental presses are more likely when the palm rests. If a second row is kept, prefer different physical heights (one row higher/lower relative to the desk), recessed or low-profile switches, or a non-strictly vertical arrangement — see [design-notes.md](design-notes.md).

### 3. Column Geometry and Fan Layout (Splay)

* **Column spacing:** Placing adjacent columns tightly against each other does not feel natural.
* **Intra-finger vs inter-finger distance:** The distance between columns served by the same finger (index or pinky) should be smaller than the distance between columns served by different fingers.
* **Natural splay:** The motion zones form a natural fan shape.
  * *Conclusion:* Columns should not only be staggered vertically but also slightly angled relative to each other so that the key travel axes align with the natural joint trajectories. This also applies to the index-finger columns, which in most layouts are made parallel to the middle-finger column — a common simplification that does not fully match the hand’s anatomy.
  * *Clarification:* Splay is the baseline, not an alternative to “extra” keys. Additional positions in the index/pinky zones can coexist with splay; positions that fall poorly inside a zone (e.g. the bottom key of the index inner column) are better **omitted** than kept only to preserve a rectangular 3×5 block.

### 4. Discreteness and Comfort

* **Adaptive centers:** A continuous painted zone does not mean equal comfort at every point. Inside each zone there are discrete points of most natural finger placement.
  * *Principle:* Key centers should be located at these “maximum comfort” points, even if this results in uneven gaps between keys.

* **Static vs dynamic reach:** At the edge of a zone, a key may still be reachable when the hand is held still. During actual typing the hand often lifts reflexively to avoid twisting the finger, then “hovers” instead of returning to a stable rest — which adds strain. Key placement should target comfort in motion, not only static reach.

* **Pinky:** Among the four non-thumb fingers, the pinky has the largest motion zone — a fact often underestimated in conventional layouts.

### 5. Related material

* Layout comparisons against the zone map, community feedback, and open design questions: [design-notes.md](design-notes.md).
