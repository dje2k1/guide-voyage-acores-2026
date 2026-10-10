# Noël au ski 2026 — design

**Thesis.** A family's ski-week decision laid out like a topo map and a comparison sheet, not a travel ad. Mode: Operate (compare, filter, open a listing).

## Tokens
| Role | Value |
|---|---|
| Paper (page) | `#F7F9FA` |
| Surface (map, buttons) | `#FFFFFF` |
| Ink / secondary / tertiary | `#1C2A32` / `#4B5B64` / `#74838B` |
| Rules | `#DCE3E7`, light `#EDF1F3` |
| Selected week column | `#EAF2F7` |
| Map: glacier / contour / river | `#E1EEF5` / `#C3D3DC` / `#7FAFCB` |
| Hovered pin | `#C2361F` |
| Private pool | `#C8952C` (ring), `#FAF1DC` (note background) |
| Over budget / full | `#A3402E` / tertiary ink |

## Type
Archivo only (Google Fonts, variable width). Titles wide (`wdth` 112–118, 700–760, tracking −0.02/−0.025em); body `wdth` 100; map lettering condensed (`wdth` 75–85), water and massifs in italic. Prices use tabular figures.

## Components
- **Week switch**: segmented control in the header; drives map pins, short-list prices, table sort and the highlighted column.
- **Map**: hand-projected SVG (lat/lon → viewBox), pins clustered around their commune, numbered with the lodging's stable number. Fill = availability for the selected week; gold ring = private pool. Phones get a zoomed viewBox and larger pins (`--u`).
- **Short-list**: four ruled rows with photo, reason, name, price for the week.
- **Comparison rows**: ruled grid, both weeks side by side, click to expand facts and notes. Collapses to stacked rows under 760px.
- **Ruled out**: two-column definition list.

## Rules
Rules and whitespace instead of boxes; photos are the only colour-rich element. Motion only answers clicks (row expand, pin hover, week switch), all ≤ 250 ms with ease-out, disabled under reduced motion. No eyebrows, no pills except small controls.
