# pyGETM nesting

Documentation of the two-way, multi-level nesting for [pyGETM](https://github.com/BoldingBruggeman/pygetm),
published with GitHub Pages: **https://bolding.github.io/nesting-docs/**

Each level of a nest is an ordinary pyGETM simulation with its own grid, time step and processes. The nesting
fills the halo zones where the levels overlap and matches the fluxes through the faces between them, so that
volume and tracer content are conserved, in 2D and in 3D between levels with different vertical grids.

## Pages

- [Overview](https://bolding.github.io/nesting-docs/) (`index.html`)
- [Methods](https://bolding.github.io/nesting-docs/methods.html) (`methods.html`): levels, halos, rim and ring, flux matching, load
  balancing; the 3D coupling; what the nesting changes in pyGETM
- Examples:
  - [IDEAL](https://bolding.github.io/nesting-docs/ideal.html) (`ideal.html`)
  - [DKm](https://bolding.github.io/nesting-docs/dkm.html) (`dkm.html`)
  - [NEAB](https://bolding.github.io/nesting-docs/neab.html) (`neab.html`)
- [Guides](https://bolding.github.io/nesting-docs/guides.html) (`guides.html`): how to run the tools and scripts, with examples
  (bathymetry, nesting-balance, the model runs, boundaries, analysis, animations)
- [Issues](https://bolding.github.io/nesting-docs/issues.html) (`issues.html`): the problems found along the way, how they were found and
  solved, and what is still open. The example pages link to the issues that concern them.
- [Status](https://bolding.github.io/nesting-docs/status.html) (`status.html`)

Figures are in `fig/` (methods) and `fig/<example>/`.

## Code

The nesting is developed on the fork [bolding/pygetm](https://github.com/bolding/pygetm), branch
`nesting-mpmd` (package `pygetm.nesting`). The example setups and the tools that build this site are not public yet.

This repository holds only the generated site: the pages are rebuilt from their sources, so edits made here
directly are overwritten. The former pages bolding/neab, bolding/dkm and bolding/ideal redirect here.

Karsten Bolding, Bolding & Bruggeman.
