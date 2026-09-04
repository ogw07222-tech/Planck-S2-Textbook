# Figma Scientific Figure Reproduction Priority

Canonical source: `main`.

## Scope and ordering rule

- Proceed in textbook dependency order, beginning with Volume 1.
- Within a chapter, reproduce the primary numbered figure first, then chapter-specific auxiliary `F1X`/`F2X` figures.
- Existing GitHub assets are reference material only. Each replacement is rebuilt from scratch in Figma as editable vectors/layers.
- Scientific meaning and `sources/proof-status.md` labels must not be changed by figure production.
- A figure advances only after: Figma build → visual/scientific QA → GitHub canonical asset/reference sync → registry update.
- Producer status stops at `ASSET PRESENT · DRAFT COMPLETE · AUDIT PENDING`; independent `AUDIT PASS` is never self-assigned.

## Actual asset inventory checked on main

### Volume 1
Present: `F001.png`, `F002.png`, `F003.png`, `F004.png`, `F005.svg`–`F018.svg`, `F1X01.png`, `F1X02.svg`–`F1X06.svg`.

### Volume 2
Present: `F019.svg`–`F030.svg` and the currently stored auxiliary Volume 2 assets listed in the directory. Volume 3+ entries in `figures/registry.md` remain `NEEDED` unless an actual asset is later verified on main.

## Reproduction priority — Volume 1 first

| Priority | Chapter | Figure | Current asset | Reason |
|---:|---:|---|---|---|
| 1 | 1 | F001 | PNG | First chapter; registry only `DRAFT CREATED`; needs fully editable vector reconstruction. |
| 2 | 2 | F002 | PNG | Early foundational dimension diagram; raster master. |
| 3 | 2 | F1X01 | PNG | Companion intrinsic/embedding diagram; raster master. |
| 4 | 3 | F003 | PNG | S¹/S² vs disk/ball distinction; foundational geometry; raster master. |
| 5 | 3 | F004 | PNG | Coordinate geometry figure; raster master; preserve audit-revised meaning. |
| 6 | 4 | F005 | SVG | Rebuild from scratch in Figma despite existing SVG. |
| 7 | 4 | F1X02 | SVG | Companion map-type comparison. |
| 8 | 5 | F006 | SVG | Scalar/vector/unit-vector field distinction. |
| 9 | 5 | F1X03 | SVG | Companion field comparison. |
| 10 | 6 | F007 | SVG | Domain S² vs target S². |
| 11 | 6 | F008 | SVG | Meaning of n(x). |
| 12 | 7 | F009 | SVG | Degree 0. |
| 13 | 7/8 | F010 | SVG | Degree +1; must preserve charge/bit/electron non-equivalence. |
| 14 | 7 | F011 | SVG | Degree −1. |
| 15 | 7 | F012 | SVG | Degree 2. |
| 16 | 7 | F1X04 | SVG | Orientation sign companion. |
| 17 | 8 | F1X05 | SVG | Q=1 meaning boundary panel. |
| 18 | 9 | F013 | SVG | Configuration distinction. |
| 19 | 10 | F014 | SVG | Configuration-space schematic; must not imply literal 2D geometry. |
| 20 | 10 | F1X06 | SVG | Mapping-space component schematic; actual physical configuration space remains OPEN. |
| 21 | 11 | F015 | SVG | Path. |
| 22 | 12 | F016 | SVG | Loop. |
| 23 | 13 | F017 | SVG | Contractible vs noncontractible loop. |
| 24 | 15 | F018 | SVG | Z₂ table; must not identify Z₂ directly with ±1 quantum phase. |

After Volume 1, continue Volume 2 in chapter order beginning with `F2X01`/`F019` according to chapter placement, then `F020`…`F030`, preserving the canonical proof-status boundaries.
