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
5. [lapka](https://github.com/braindefender/lapka) (*)
6. [lapka-42](https://github.com/braindefender/lapka-42) (*)
7. [Charlieflex](https://github.com/ctranstrum/chuck)
8. [Lintilla](https://github.com/ctranstrum/lintilla)
9. [Visorbearer](https://github.com/carrefinho/visorbearer)

*Note:* * — the layout is missing from or limited in [layout-comparison.dxf](../cad/ergonomics/layout-comparison.dxf) due to licensing constraints.

Layouts were aligned to the resting position of the middle finger. The middle-finger column was oriented vertically for every layout so the remaining columns could be compared consistently.

### TOTEM

Splay is used only on the middle, ring, and pinky columns. The index columns run parallel to the middle column.

The index finger has two columns with a small Y offset. The bottom key of the outer index column sits poorly inside the index zone.

The pinky has two columns; the outer one has only a single key. There is no obstacle to adding one or even two more keys on the outer pinky column. It would help to move the pinky columns farther from the ring column and slightly down in Y to better match the pinky zone.

The middle and ring columns, and the thumb cluster, match their zones best. The thumb cluster is three keys in one row; their placement almost perfectly follows the upper arc of the thumb-zone boundary.

The case geometry is worth noting: a rectangle whose sides are orthogonal to the middle-finger column. Peripheral keys that stick outside the case are less appealing — though that choice is probably popular with many split-keyboard users.

### KLOR POLYDACTYL

Same author as TOTEM, created slightly earlier and effectively its predecessor. TOTEM inherited KLOR’s main ideas for key arrangement and case, but the layout geometry differs slightly.

Key spacing on KLOR is a bit larger — so the outer bottom index key intersects the index zone even worse.

The pinky columns sit a little farther from the ring column; the outer pinky column has two keys — both points are positive.

The thumb cluster is four keys in one row, slightly lower than on TOTEM. All four sit well inside the thumb zone, but they no longer trace the upper arc of the zone boundary as cleanly.

### yacc46

Key count and placement for the pinky, ring, and middle columns match KLOR POLYDACTYL one-to-one. Differences are in the index columns and the thumb cluster.

yacc46 has three index columns, parallel to the middle column and slightly higher in Y than on KLOR. The inner and middle columns have three keys each; the outer has two. Both outer keys fall outside the index zone. Also outside the zone: the top key of the inner index column, and the top and bottom keys of the middle index column.

The thumb cluster is four keys in two rows: three on the upper row (along an arc) and one on the lower row under the central upper key. The upper arc does not sit ideally inside the thumb zone; the outer upper key exceeds thumb reach.

### LYNX

Only the four-finger block is considered. Columns are parallel to each other; almost all keys are ortho-linear, except those on the outer index column.

Two strong points:

1. the smallest inter-key spacing among the layouts compared;
2. spacing between columns of the same finger is smaller than spacing between columns of different fingers — which matches the principle in [ergonomics.md](ergonomics.md) and comes from using microswitches.

Middle and ring columns have four keys each; all sit well inside their zones.

The index finger has two columns: four keys on the inner, three on the outer with a Y offset. All index-column keys sit well inside the index zone.

The pinky has two columns: three keys on the inner, two on the outer. Only the top key of the inner pinky column leaves the pinky zone and lands entirely in the ring zone.

### Lapka

All four-finger columns are splayed relative to each other, including the outer index column. Angles between the middle, ring, and pinky columns are nearly the same as on TOTEM.

Differences: the pinky has only one column of three keys; the pinky and ring columns sit slightly higher. As a result, the top pinky key largely leaves the pinky zone.

The index finger has two columns of three keys each. The bottom key of the outer index column largely leaves the index zone.

The thumb cluster is three keys in one row; all three lie inside the thumb zone.

### Lapka-42

Compared with Lapka, an outer pinky column of three keys was added — parallel and ortho-linear to the inner pinky column.

The outer index column was also made parallel and ortho-linear to the inner one (uniform splay across all columns looked nicer to the author on the original Lapka; on 42 keys, full splay would have worked worse in their view).

On the map: the bottom outer index key sits better inside the index zone. The thumb cluster moved up in Y, and its outer key now leaves the thumb zone.

### Charlieflex

Distinctive feature: two columns under the ring finger — three keys on the main column and one extra key on the upper row toward the pinky zone. That is interesting: the ring zone has a protrusion in exactly that area. On my map the extra key sits partly in the ring zone and partly in the pinky zone. With microswitches instead of a 19×19 grid, the idea could probably be executed more cleanly.

The pinky has only two keys; the column is shifted down in Y — that seems right, but the gap to the ring column could be larger.

The index finger has two parallel columns splayed relative to the middle: three keys on the inner, two on the outer. The outer column is shifted down in Y, so the bottom key leaves the index zone.

The thumb cluster is two keys in one row; the outer one slightly leaves the zone.

### Lintilla

Same author as Charlieflex. Key count and placement are very close to KLOR POLYDACTYL, with these differences:

- pinky columns are slightly closer in X to the ring column and a little lower in Y;
- the thumb row has three keys (no under-palm key as on KLOR);
- there is an extra key outside the finger reach zones, roughly above the pinky and ring zones.

### Visorbearer

Pinky and ring columns use a more aggressive splay than TOTEM. The pinky column has three keys and is shifted down to a level similar to Charlieflex. I support that shift, but the column is still close to the ring column — the bottom key leaves the pinky zone.

The index finger has two parallel columns: three keys on the inner, two on the outer. All of these keys fall inside the index zone.

The thumb has one row of two keys. The row sits fairly high in Y: the inner key is about halfway outside the zone; the outer key is entirely outside.

## Working layout hypothesis

Prefer not a plain 3×5 block, but a layout with positions that fit the zones poorly trimmed away, while keeping splay.

Target for the **four fingers** (thumb cluster excluded): **2×6 + 1×4** — six columns on the upper and home rows, and four columns on the bottom row. To be refined with mock-ups and further overlays.

## Thumb cluster: two rows

By zone area, two rows look justified. Feedback from several people in the [Ergonomic Keyboards](https://t.me/ergokeyboards) chat (Oct 2026):

- two keys **in the same column** are awkward to press with the thumb — the thumb bends unnaturally;
- resting the palm on the desk or case increases the risk of accidental presses on the “far” row;
- mitigating ideas: different row heights (one higher, one lower); short key travel; keys recessed into the case; wrist rests (debatable on a flat board).

Important: the negative experience mainly concerns a **Y-pair in one column**, not every kind of second row (an arc or X-offset may behave differently).

Putting `Alt`+`Ctrl` (and likewise `Shift`+`Super`) in one column under the thumb for simultaneous chords: one participant dropped that idea on ordinary splits because of misclicks and discomfort; combos and macros were easier. Needs validation on a mock-up.

## Open questions

- Best geometry for a second thumb row on a **flat** low-profile board (no keywell — bowl-shaped case recess).
- How many physical modifiers to move off layers and hold-tap onto dedicated keys without overloading the thumb and pinky.

## Feedback sources

Discussion in [Ergonomic Keyboards](https://t.me/ergokeyboards) (Oct 2026), including comments from Lapka authors and users of other flat splits.
