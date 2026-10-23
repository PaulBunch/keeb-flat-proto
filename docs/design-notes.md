<!--
SPDX-FileCopyrightText: 2026 Paul Bunch
SPDX-License-Identifier: CERN-OHL-P-2.0
-->

# Layout Design Notes

> [Читать на русском](design-notes.ru.md)

Working log: comparisons of existing keyboard layouts against the finger-zone map, community feedback, and open questions.

Overlay drawings of layouts on the finger-motion map are in [layout-comparison.dxf](../cad/ergonomics/layout-comparison.dxf).

Layout principles derived from the finger-motion map are in [ergonomics.md](ergonomics.md).

## Comparisons of existing layouts against the finger-motion map

Flat or nearly flat layouts were overlaid on the map:

1. [TOTEM](https://github.com/GEIGEIGEIST/TOTEM)
2. [KLOR POLYDACTYL](https://github.com/GEIGEIGEIST/KLOR) (*)
3. [yacc46](https://github.com/1m38/keyboards/tree/main/yacc46)
4. [LYNX](https://www.lynxware.org/) (*) — four-finger block only
5. [Lapka](https://github.com/braindefender/lapka) (*)
6. [Lapka-42](https://github.com/braindefender/lapka-42) (*)
7. [Charlieflex](https://github.com/ctranstrum/chuck)
8. [Lintilla](https://github.com/ctranstrum/lintilla)
9. [Visorbearer](https://github.com/carrefinho/visorbearer)
10. [Kyria](https://github.com/splitkb/kyria) (*)
11. [Redox](https://github.com/mattdibi/redox-keyboard)
12. [Dygma Defy](https://dygma.com/products/dygma-defy) (*)

*Note:* * — the layout is missing from or limited in [layout-comparison.dxf](../cad/ergonomics/layout-comparison.dxf) due to licensing constraints.

Layouts were aligned to the resting position of the middle finger. The middle-finger column was oriented vertically for every layout so the remaining columns could be compared consistently.

### TOTEM

Splay is used only on the middle, ring, and pinky columns. The index columns run parallel to the middle column.

The index finger has two columns with a small Y offset. The bottom key of the outer index column sits poorly inside the index zone.

The pinky has two columns; the outer one has only a single key. There is no obstacle to adding one or even two more keys on the outer pinky column. It would help to move the pinky columns farther from the ring column and slightly down in Y to better match the pinky zone.

The middle and ring columns, and the thumb cluster, match their zones best. The thumb cluster is three keys in one row; their placement almost perfectly follows the outer arc of the thumb-zone boundary.

The case geometry is worth noting: a rectangle whose sides are orthogonal to the middle-finger column. Peripheral keys that stick outside the case are less appealing — though that choice is probably popular with many split-keyboard users.

### KLOR POLYDACTYL

Same author as TOTEM, created slightly earlier and effectively its predecessor. TOTEM inherited KLOR’s main ideas for key arrangement and case, but the layout geometry differs slightly.

Key spacing on KLOR is a bit larger — so the outer bottom index key intersects the index zone even worse.

The pinky columns sit a little farther from the ring column; the outer pinky column has two keys — both points are positive.

The thumb cluster is four keys in one row, slightly lower in Y than on TOTEM. All four sit well inside the thumb zone, but they no longer trace the outer arc of the zone boundary as cleanly.

### yacc46

Key count and placement for the pinky, ring, and middle columns match KLOR POLYDACTYL one-to-one. Differences are in the index columns and the thumb cluster.

yacc46 has three index columns, parallel to the middle column and slightly higher in Y than on KLOR. The inner and middle columns have three keys each; the outer has two. Both outer keys fall outside the index zone. Also outside the zone: the top key of the inner index column, and the top and bottom keys of the middle index column.

The thumb cluster is four keys in two rows: three on the top row (along an arc) and one on the bottom row under the central top key. The top-row arc does not sit ideally inside the thumb zone; the outer top key exceeds thumb reach.

### LYNX

Only the four-finger block is considered. Columns are parallel to each other; almost all keys are ortho-linear, except those on the outer index column.

Two strong points:

1. the smallest inter-key spacing among the layouts compared (18.4 mm between columns of neighbouring fingers; 13.8 mm between columns of the same finger; 12 mm between rows in Y);
2. spacing between columns of the same finger is smaller than spacing between columns of different fingers — which matches the principle in [ergonomics.md](ergonomics.md) and comes from using microswitches.

Middle and ring columns have four keys each; all sit well inside their zones.

The index finger has two columns: four keys on the inner, three on the outer with a Y offset. All index-column keys sit well inside the index zone.

The pinky has two columns: three keys on the inner, two on the outer. Only the top key of the inner pinky column leaves the pinky zone and lands entirely in the ring zone.

### Lapka

All four-finger columns are splayed relative to each other, including the outer index column. Angles between the middle, ring, and pinky columns are nearly the same as on TOTEM.

Differences: the pinky has only one column of three keys; the pinky and ring columns sit slightly higher in Y. As a result, the top pinky key largely leaves the pinky zone.

The index finger has two columns of three keys each. The bottom key of the outer index column largely leaves the index zone.

The thumb cluster is three keys in one row; all three lie inside the thumb zone.

### Lapka-42

Compared with Lapka, an outer pinky column of three keys was added — parallel and ortho-linear to the inner pinky column.

The outer index column was also made parallel and ortho-linear to the inner one (uniform splay across all columns looked nicer to the author on the original Lapka; on 42 keys, full splay would have worked worse in their view).

On the map: the bottom outer index key sits better inside the index zone. The thumb cluster moved up in Y, and its outer key now leaves the thumb zone.

### Charlieflex

Distinctive feature: two columns under the ring finger — three keys on the main column and one extra key on the top row toward the pinky zone. That is interesting: the ring zone has a protrusion in exactly that area. On my map the extra key sits partly in the ring zone and partly in the pinky zone. With microswitches instead of a 19×19 grid, the idea could probably be executed more cleanly.

The pinky has only two keys; the column is shifted down in Y — that seems right, but the gap to the ring column could be larger.

The index finger has two parallel columns splayed relative to the middle: three keys on the inner, two on the outer. The outer column is shifted down in Y, so the bottom key leaves the index zone.

The thumb cluster is two keys in one row; the outer one slightly leaves the zone.

### Lintilla

Same author as Charlieflex. Key count and placement are very close to KLOR POLYDACTYL, with these differences:

- pinky columns are slightly closer in X to the ring column and a little lower in Y;
- the thumb row has three keys (no under-palm key as on KLOR);
- there is an extra key outside the finger reach zones, roughly above the pinky and ring zones in Y.

### Visorbearer

Pinky and ring columns use a more aggressive splay than TOTEM. The pinky column has three keys and is shifted down in Y to a level similar to Charlieflex. I support that shift, but the column is still close to the ring column — the bottom key leaves the pinky zone.

The index finger has two parallel columns: three keys on the inner, two on the outer. All of these keys fall inside the index zone.

The thumb has one row of two keys. The row sits fairly high in Y: the inner key is about halfway outside the zone; the outer key is entirely outside.

### Kyria

Kyria is said to have inspired KLOR, from which TOTEM was later derived.

Only the thumb cluster is of interest here. It has two rows: five keys on the bottom row, two on the top. The top keys sit directly above the outer bottom key and the key in the adjacent column. The bottom-row keys lie inside the thumb zone and follow an arc that matches the outer arc of thumb motion well. The deepest under-palm key on the bottom row sits on the boundary between the ring and middle zones. Both top keys fall entirely outside the thumb reach zone.

### Redox

Only the dual-row thumb cluster is of interest. The bottom row has three keys; the top has two. The outer and centre bottom keys are 1.5u; the inner is 1.25u. The outer and centre keys align with the thumb; the inner is rotated 90° relative to them. The two top 1u keys sit directly above the outer and centre bottom keys. The three bottom keys lie inside the thumb zone on the same arc as Kyria’s. Both top keys lie outside the thumb zone — even farther in Y than Kyria’s top keys.

### Custom (24+6)×2 Split, 2×3 Thumbs (Weirwynn)

In my view the Redox and Kyria thumb clusters sit too high in Y, forcing the thumb to reach for the top row. In the Reddit discussion, user Weirwynn shared a photo of their Custom (24+6)×2 Split with a 2×3 thumb cluster. It has two ortho-linear rows. The cluster is rotated ~12.5° relative to the main key grid. Centre-to-centre column pitch in the thumb cluster is 16 mm. Bottom-row keys are 1.5u; top-row keys are 1u. In the photo the top-row keycaps look roughly twice as tall as the bottom ones — consistent with a Z-height split between rows, though the comment text does not state that explicitly. The top-row keys sit at roughly the same Y position as the bottom-row keys on Kyria and Redox. I consider this placement the most successful of the dual-row examples so far.

### Dygma Defy

The main point of interest is the thumb cluster. The switches sit on a single plane tilted about 3° relative to the desk: the farther a row is from the wrist, the higher it sits above the desk (Z). Call this the base plane.

The cluster has eight keys: four on the top row, three on the bottom, and one long outer key spanning both rows. Keys follow an arc that matches the natural motion of an extended thumb.

All keys fall inside the thumb zone. In top view the keys vary in size: extent in Y is comparable to the main keys (~18 mm); width in X ranges from 13 to 27 mm. Most are trapezoidal; the 13 mm minimum is the narrow base of the trapezoid. The long outer key is about 40 mm in Y.

Keys are staggered in Z: the top row is higher; the bottom row and the long outer key are lower. In side view the top surface of the top-row keys is at 11° to the base plane. Vertical distance from the top surface of the bottom-row keys to the nearest edge of the top-row keys is 4.3 mm; to the far edge, 6.7 mm. That matches MX travel (3.2–4 mm) used on the top row. The cluster sits slightly below the average top surface of the other four fingers’ keys: about 2.7 mm from the top of the top-row keys to the mean surface of the main keys.

The Defy cluster is among the most carefully engineered. That conclusion comes from a Dygma Lab YouTube overview of the thumb cluster. The solutions used there are worth carrying into this project. A detailed analysis (geometry and prototype evolution) is in [thumb-cluster-defy.ru.md](thumb-cluster-defy.ru.md) (Russian).

Keycap geometry takeaways:

- convex profile on thumb keycaps;
- V-shaped gaps between keycaps (pyramidal form);
- chamfered edges between keys at different Z heights;
- tactile homing bump on the primary thumb key.

Ideas rejected during development:

- keycaps with a very small top surface area;
- narrow (small extent in Y in top view) top-row keycaps;
- a three-row cluster;
- a shallow arc in favour of a tighter radius of curvature.

Two hypotheses explain the different key counts (4 on the top row, 3 on the bottom) and the staggered (not stacked) placement:

1. **Geometric:** with a tighter bottom-row arc, switch body size limits packing density. The same constraint produces the staggered offset between rows.
2. **Anatomical:** the stagger and the reduced bottom-row count follow the natural thumb path and improve hit accuracy.

> To clarify this, a discussion was opened on 23 Oct 2026 in [r/DygmaLab](https://www.reddit.com/r/DygmaLab/comments/1xdf5n2/defy_thumb_cluster_why_are_top_and_bottom_row).

Magnetic attachment of the palm rests (magnets in the case and in the rest) is a nice detail.

## Working layout hypothesis

Prefer not a plain 3×5 block, but a layout with positions that fit the zones poorly trimmed away, while keeping splay.

Target for the **four fingers** (thumb cluster excluded): **2×6 + 1×4** — six columns on the top and home rows, and four columns on the bottom row. To be refined with mock-ups and further overlays.

## Thumb cluster: two rows — community summary

Survey in October 2026 in the [Ergonomic Keyboards](https://t.me/ergokeyboards) chat and on [r/ErgoMechKeyboards](https://www.reddit.com/r/ErgoMechKeyboards/comments/1x8gdxb/has_anyone_documented_perfinger_reach_zones/): experience with dual-row thumbs on flat or nearly flat boards.

### Common complaints

* Reaching the second row means “stepping over” the near row — the thumb works with the **pad** and tends toward an awkward **claw curl**.
* Misclicks when the palm rests on the case or desk (not universal; Dygma Defy with a palm rest did not report this).
* With a relatively short thumb, the bottom row sits too close to the palm.
* Some people rarely use the top row for typing and relegate it to infrequent functions (backlight, etc.).
* Repeated motion at the extremes of thumb range is linked to overuse risk — [Getreuer, thumb ergo anecdotes](https://getreuer.info/posts/keyboards/thumb-ergo/index.html#anecdotes). Russian notes on possible injuries: [thumb-overuse.ru.md](thumb-overuse.ru.md).

### Working mitigations

* Different **row heights in Z** (elevation) and a slight hand angle — dual-row without curl; sometimes a comfortable simultaneous combo of both rows.
* Low-profile (or lower caps) on the row nearer the palm; taller or standard caps on the far row.
* Top key in a column mainly as part of a **combo** with the bottom key, not as a frequent single press; otherwise a rare macro.
* 1.5u on the bottom thumb row — easier to press with the **heel** of the thumb, less tip curl (report from the custom 2×3 cluster).
* Tighter thumb pitch (e.g. 16×19 mm) and ~12.5° cluster angle — positive long-term experience; vertical chords almost unused.
* Dygma Defy — multi-year dual-row use with no cluster complaints *when a palm rest is used*.

### Dual-row references

| Layout | Thumb | Note |
|--------|-------|------|
| yacc46 | 2 rows (3+1) | Top-row arc weaker |
| Custom (24+6)×2, 2×3 | 2×3 | 16×19 mm, ~12.5°; photo in the Reddit thread |
| Dygma Defy | dual-row + Z-height split | Commercial; long-term + palm rest |
| Kyria / Redox | 2 rows | Top row above the zone in Y — what to avoid |

### Preliminary conclusion

Community rejection of dual-row largely inherits the geometry of early references (top row too far in Y / awkward to reach). A few custom builds (2×3, different pitch/angle, top row as combo) work long-term but are almost invisible and do not shape “common opinion.”

### Decision for MVP

On the flat prototype, **include two thumb rows** to validate the arrangement on my own hand — do not average the majority’s rejection.

Starting constraints:

* allow different row or keycap heights in Z;
* during build and the first weeks of typing, watch for thumb fatigue (see Getreuer’s cautions).

Field results may keep two rows, simplify to one, or change geometry (arc, X offset, Z height).

## Outer pinky column

Reddit user Weirwynn uses wide (1.5u) keys on the outer pinky column of the Custom (24+6)×2 Split for these reasons:

- tactile homing (the edge of the row feels different);
- lower precision demand when stretching to the top keys and when holding Shift with the same hand (no opposite-hand Shift);
- continuity with the wide outer keys of standard keyboards, as long as it does not fight the zones.

Worth recording: use a different keycap profile (wider / otherwise distinct) on the outer pinky column. No prior mispresses in the pinky zone, but it is worth checking on a mock-up — especially if Shift modifiers stay on the pinky.

## Open questions

- How many physical modifiers to move off layers and hold-tap onto dedicated keys without overloading the thumb and pinky.
- What Z height / pitch / thumb-cluster angle is the minimum needed so the top row does not sit on the edge of reach.

## Feedback sources

- Discussion in [Ergonomic Keyboards](https://t.me/ergokeyboards) (Oct 2026), including comments from Lapka authors and users of other flat splits.
- Dual-row thumb survey on [r/ErgoMechKeyboards](https://www.reddit.com/r/ErgoMechKeyboards/comments/1x8gdxb/has_anyone_documented_perfinger_reach_zones/) (Oct 2026).
