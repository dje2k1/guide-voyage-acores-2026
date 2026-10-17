# Ski en famille, février 2027 — design

**Thesis.** A family's ski-week decision laid out like a topo map and a ranked comparison sheet, not a travel ad. Mode: Operate (compare, filter, open a listing).

## Tokens
| Role | Value |
|---|---|
| Paper (page) | `#F7F9FA` |
| Surface (map, buttons) | `#FFFFFF` |
| Ink / secondary / tertiary | `#1C2A32` / `#4B5B64` / `#74838B` |
| Rules | `#DCE3E7`, light `#EDF1F3` |
| Selected week column | `#EAF2F7` |
| Map: glacier / ridge / contour / river | `#E1EEF5` / `#EEF4F7` / `#C3D3DC` / `#7FAFCB` |
| Hovered pin | `#C2361F` |
| Pool access | `#C8952C` (ring), `#8A6418` (text), `#FAF1DC` (note background) |
| Over budget | `#A3402E` |

## Type
Archivo only (Google Fonts, variable width). Titles wide (`wdth` 108–118, 680–760, tracking −0.02/−0.025em); body `wdth` 100; map lettering condensed (`wdth` 75–85), water, massifs and ski areas in italic. Prices use tabular figures.

## Components
- **Week switch**: February (6–13) / April (3–10) segmented control in the header, with a one-line note on crowds and lift closures; drives map pins, short-list prices and the highlighted column.
- **Map**: hand-projected SVG of the Mont-Blanc country (lat/lon → viewBox 800×612). Desktop: pins hex-packed around their commune, best rank in the middle, numbered by rank. Fill = availability for the selected week, gold ring = pool access. Phones: one bubble per commune with the count of lodgings free in budget; tapping filters the table to that commune.
- **Short-list**: top five (photo, reason, name, size, price) and three no-review finds in a compact list.
- **Ranking table**: rank, photo, name/where/size, wellness, reviews, both weeks, link. Click to expand facts, the score breakdown and a yellow "check before booking" note. First 20 rows, then a "show the rest" button. Collapses to stacked rows under 760px.
- **Method**: five-column definition list explaining the 100-point score.
- **Ruled out**: two-column definition list.

## Rules
Rules and whitespace instead of boxes; photos are the only colour-rich element. Motion only answers clicks (row expand, pin hover, week switch), all ≤ 250 ms with ease-out, disabled under reduced motion. No eyebrows, no pills except small controls.
