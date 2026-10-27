# Assignment 1: Night Shift

**Live site:** https://jaswin2302.github.io/a1-ghd3/

Night Shift is a generated harbor city drawn with SVG primitives and d3.js. Drag the clock through a 24 hour day and the whole scene recolors, from a pastel noon to a dark skyline full of lit windows.


Shapes used: `rect` (buildings, windows), `circle` (stars, moon, sun, lamps), `line` (antennas, lamp posts), `polygon` (mountains, spires), `path` (waves, trees), and `ellipse` (clouds).

## Technical Achievements

* **Linked views.** Hovering a bar in the census chart highlights every shape of that type in the city. Hovering a shape in the city shows a tooltip and lights up its bar.

* **Seeded generation.** Each city is built from a random seed using `d3.randomLcg`. The seed is saved in the URL so a city can be shared.
* **Time of day model.** Color scales drive the sky, buildings, water and everything else. Windows turn on one by one at dusk.
* **Draggable clock** built with `d3.arc` and `d3.drag`.
* **Extra shapes:** ellipses, `d3.symbol` triangles, `d3.arc`, smooth `d3.line` curves, a gradient and a glow filter.
* **Animation.** Buildings rise in on load, census bars count up, clouds drift, and Play runs through the whole day.

## Design Achievements

* **Day and night palette** that looks good at every hour, not just noon and midnight.
* **Ambient motion:** twinkling stars, blinking beacons, drifting clouds and flowing water. Turned off for users with reduced motion enabled.
* **Responsive layout** that scales to any screen width.
* **Tooltips with color swatches** for inspecting any shape.
* **Log scale census** so small counts stay visible next to hundreds of windows.

## Sources

* Written from scratch using the [d3.js docs](https://d3js.org/).
