# Assignment #2 — Advanced CSS (Flexbox & Grid)

Three independent tasks, plain HTML/CSS only (no Bootstrap, no JavaScript, no media queries).

## Structure

```
task1-grid-composition/   Geometric composition, CSS Grid only
task2-component-library/  Five reusable UI components, Flexbox only
task3-multi-layout/       One markup, three switchable layouts (Grid + Flexbox)
```

Open any `index.html` directly in a browser — no build step, no dependencies.

## Task 1 — Geometric composition (CSS Grid)
A single `.composition` element is a 6×6 CSS Grid (`grid-template-columns/rows: repeat(6, 1fr)`).
Each colored block is placed with `grid-column` / `grid-row` spans. The black lines are the grid
container's own background showing through the `gap` between cells — no borders or margins on the
blocks. The whole grid is sized with `width: min(90vw, 90vh, 720px)` and `aspect-ratio: 1/1`, so it
stays square and never grows taller than the viewport.

## Task 2 — Component library (Flexbox)
Five components — navbar, card row, pagination bar, comment block, pricing table — sharing one
stylesheet, one color palette (CSS custom properties) and one spacing scale. All layout is Flexbox:
`flex-wrap`, `flex: 1 1 <basis>`, `margin-left: auto`, `align-items`, etc. No fixed widths/heights are
used for layout; only the avatar keeps its own intrinsic size, as allowed by the brief.

## Task 3 — Three layouts, one markup (Grid + Flexbox)
One `.gallery` of 12 `.item` articles. The container's display mode (grid of cards / compact list /
magazine with a lead item) is controlled by a single state on the container — implemented with a
CSS-only radio/`:checked` toggle so the three modes can be demoed live without JavaScript. Each mode
is CSS Grid at the container level; Flexbox is used inside every `.item` to arrange its image, text and
date (column direction in grid/magazine mode, row direction in list mode).

## Author
`<Maidabek Bertan>`, group `<IT-2505>`
