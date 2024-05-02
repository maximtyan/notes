---
layout: default
title: XFOIL Airfoil Analysis Guide
has_children: false
parent: Guides
grand_parent: Notes
---

# XFOIL Airfoil Analysis

[official page](http://web.mit.edu/drela/Public/web/xfoil/)

- Viscous (or inviscid) analysis of an existing airfoil, allowing
  - forced or free transition
  - transitional separation bubbles
  - limited trailing edge separation
  - lift and drag predictions just beyond CLmax
  - Karman-Tsien compressibility correction
  - fixed or varying Reynolds and/or Mach numbers
- Airfoil design and redesign by interactive modification of surface speed distributions, in two methods:
  - Full-Inverse method, based on a complex-mapping formulation
  - Mixed-Inverse method, an extension of XFOIL's basic panel method
- Airfoil redesign by interactive modification of geometric parameters such as
  - max thickness and camber, highpoint position
  - LE radius, TE thickness
  - camber line via geometry specification
  - camber line via loading change specification
  - flap deflection
  - explicit contour geometry (via screen cursor)
- Blending airfoils
- Writing and reading of airfoil coordinates and polar save files
- Plotting of geometry, pressure distributions, and multiple polars

## Interface

- XFOIL is an interactive program for the design and analysis of
  subsonic isolated airfoils.
- Analysis is performed using text user’s interface (keyboard input).

[xfoil main page](xfoil-1.png)

## Load airfoil

### Load airfoil from text file

```text
LOAD filename.txt
```

`filename.txt` – name of the coordinates file

### Use NACA 4-series airfoil

```text
NACA XXXX
```

`XXXX` – 4 digit code for NACA airfoil (example 2312)

{: .important }
> In XFOIL, the X and Y coordinate delimiter is mutiple space symbols, not tabs
