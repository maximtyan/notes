---
layout: default
title: Software for Aircraft Analysis
has_children: false
parent: Guides
grand_parent: Notes
---

# Software for Aircraft Analysis and Design

In this section, I have listed software and datasets useful for aircraft
analysis and design. The list primarily comprises free and open-source
programs.

## Configuration

### OpenVSP

<https://openvsp.org/>

OpenVSP, also known as Open Vehicle Sketch Pad, is an open-source parametric aircraft geometry tool originally developed by NASA. It can be used to create 3D models of aircraft and to support engineering analysis of those models.  OpenVSP allows the user to quickly generate computer models from ideas, which can then be analyzed. As such, it is especially powerful in generating and evaluating unconventional design concepts.

### CPACS

<https://cpacs.de>

The Common Parametric Aircraft Configuration Schema (CPACS) is a data definition for the air transportation system. CPACS enables engineers to exchange information between their tools. It is therefore a driver for multi-disciplinary and multi-fidelity design in distributed environments. CPACS describes the characteristics of aircraft, rotorcraft, engines, climate impact, fleets, and mission in a structured, hierarchical manner. Not only product but also process information is stored in CPACS. The process information helps in setting up workflows for analysis modules. Since CPACS follows a central model approach, the number of interfaces is reduced to a minimum.

CPACS uses the following software for visualization and data interpretation.

- [TiXi](https://github.com/DLR-SC/tixi)
- [TiGL](https://dlr-sc.github.io/tigl/)
- [RCE](https://rcenvironment.de/)

## Aerodynamic Analysis

### SU2

<https://su2code.github.io/>

The SU2 suite is an open-source collection of C++ based software tools for performing Partial Differential Equation (PDE) analysis and solving PDE-constrained optimization problems. The toolset is designed with Computational Fluid Dynamics (CFD) and aerodynamic shape optimization in mind but is extensible to treat arbitrary sets of governing equations such as potential flow, elasticity, electrodynamics, chemically reacting flows, and many others. SU2 is under active development by individuals all around the world on GitHub and is released under an open-source license.

### Friction

<https://archive.aoe.vt.edu/mason/Mason_f/MRsoft.html#SkinFriction>

This program can be used to estimate the basic friction drag of an airplane. It is from Mason's Applied Computational Aerodynamics Class, and the acrobat manual is App. D.5 of the class notes. It should run using any FORTRAN compiler. Along with the manual and code, a sample input and the resulting sample output are provided. The program is available in Fortran and Matlab.

### XFOIL

<http://web.mit.edu/drela/Public/web/xfoil/>

XFOIL is an interactive program for the design and analysis of subsonic isolated airfoils. It consists of a collection of menu-driven routines which perform various useful functions such as:

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
- Blending of airfoils
- Writing and reading of airfoil coordinates and polar save files
- Plotting of geometry, pressure distributions, and multiple polars

### JavaFoil

<http://www.mh-aerotools.de/airfoils/javafoil.htm>

JAVAFOIL is a relatively simple program, which uses several traditional methods for the analysis of airfoils in subsonic flow. The main purpose of JAVAFOIL is to determine the lift, drag and moment characteristics of airfoils. The program will first calculate the distribution of the velocity on the surface of the airfoil. For this purpose, it uses a potential flow analysis module which is based on a higher order panel method (linear varying vorticity distribution). This local velocity and the local pressure are related by the Bernoulli equation. To find the lift and the pitching moment coefficient the distribution of the pressure can be integrated along the surface. Next JAVAFOIL will calculate the behavior of the flow layer close to the airfoil surface (the boundary layer). The boundary layer analysis module (a so-called integral method) steps along the upper and the lower surfaces of the airfoil, starting at the stagnation point. It solves a set of differential equations to find the various boundary layer parameters. The boundary layer data is then used to calculate the drag of the airfoil from its properties at the trailing edge.

### XFLR5

<http://www.xflr5.tech/xflr5.htm>

XFLR5 includes the XFOIL program for foil analysis, and several 3d analysis methods for planes:

- a non-linear lifting line method for standalone wings
- two vortex-lattice and a 3d panel method for the analysis of aerodynamic performance of wings and plane operating at low Reynolds numbers.
- The latest version introduces stability analysis of planes.

### AVL

<http://web.mit.edu/drela/Public/web/avl/>

AVL is a program for the aerodynamic and flight-dynamic analysis of rigid aircraft of arbitrary configuration. It employs an extended vortex lattice model for the lifting surfaces, together with a slender-body model for fuselages and nacelles. General nonlinear flight states can be specified. The flight dynamic analysis combines a full linearization of the aerodynamic model about any flight state, together with specified mass properties.

### Tornado VLM

<http://tornado.redhammer.se/>

Tornado is a Vortex Lattice Method for linear aerodynamic wing design applications in conceptual aircraft design or in aeronautical education. By modelling all lifting surfaces as thin plates, Tornado can solve for most aerodynamic derivatives for a wide range of aircraft geometries. With a very high computational speed, Tornado gives the user immediate feedback on design changes, making quantitative knowledge available earlier in the design process.
The code is implemented in MATLAB and is being used at many universities and corporations around the world. It is still in a development phase with new functionality added. The code can either be run with a text-based interface or in batch mode.

### Digital Datcom

<https://www.pdas.com/datcom.html>

This computer program calculates static stability, high lift and control, and dynamic derivative characteristics using the methods contained in the USAF Stability and Control Datcom (Data Compendium). Configuration geometry, attitude, and Mach range capabilities are consistent with those accommodated by the Datcom. The program contains a trim option that computes control deflections and aerodynamic increments for vehicle trim at subsonic Mach numbers. The user's manual (on the disc) presents the program capabilities, input and output characteristics, and example problems. User oriented features of the program include minimized input requirements, input error analysis, and various options for application flexibility.  

## Propulsion

### QProp

<http://web.mit.edu/drela/Public/web/qprop/>

QPROP is an analysis program for predicting the performance of propeller-motor or windmill-generator combinations. QMIL is a companion propeller/windmill design program. QPROP's output is entirely in tabular text format, and is typically used in conjunction with the user's own plotting programs. It is intended for large-scale parametric sweeps, driven manually or via batch execution.

### JavaProp

<http://www.mh-aerotools.de/airfoils/javaprop.htm>

JavaProp is a relatively simple program, which is based on the blade element theory. The propeller blade is divided into small sections, which are handled independently from each other. Each segment has a chord and a blade angle and associated airfoil characteristics. The theory makes no provision for three dimensional effects, like sweep angle or cross flow. But it can find the additional axial and circumferential velocity added to the incoming flow by each blade segment. This additional velocity results in an acceleration of the flow and thus thrust. Usually this simplified model works very well, when the power and thrust loading of the propeller (power per disk area) are relatively small, as it is the case for most aircraft propellers.

### Drive Calculator

<http://www.drivecalc.de/>

Drive Calculator is a free tool for brushless motor power system analysis and prop/motor selection. It has a large and growing database of motors, propellers, ESCs, and batteries. You can test combinations to get an estimate of maximum current, efficiency, prop speed, etc. It is available for Windows, MAC, and Linux.

### XROTOR

<http://web.mit.edu/drela/Public/web/xrotor/>

XROTOR is an interactive program for the design and analysis of ducted and free-tip propellers and windmills. It consists of a collection of menu-driven routines which perform various useful functions such as:

- Design of minimum induced loss rotor (propeller or windmill)
- Prompted input of an arbitrary rotor geometry
- Interactive modification of a rotor geometry
- Twist optimization of an arbitrary rotor for minimum induced loss
- Analysis of a rotor with a wealth of choices of operating parameters
- Incoming slipstream effects (from an upstream propeller, viscous wake...)
- Multi-point parameter display
- Structural analysis and corrections for twist under load
- Acoustic analysis with dB noise footprint predictions
- Interpolation of geometry to radii of interest
- Plotting of geometry, aerodynamic parameters, and performance maps

## Aircraft Design and MDO

### SUAVE

<https://suave.stanford.edu/>

SUAVE is a conceptual level aircraft design environment built with the ability to analyze and optimize both conventional and unconventional designs. This capability is achieved in part by allowing analysis information for aircraft to be drawn from multiple sources. Many other software tools for aircraft conceptual design rely on fixed empirical correlations and other handbook approximation. SUAVE instead provides a framework that can be used to design aircraft featuring advanced technologies by augmenting relevant correlations with physics-based methods.

### OpenMDAO

<https://openmdao.org/>

OpenMDAO is an open-source high-performance computing platform for systems analysis and multidisciplinary optimization, written in Python. It enables you to decompose your models, making them easier to build and maintain, while still solving them in a tightly coupled manner with efficient parallel numerical methods.
The OpenMDAO project is primarily focused on supporting gradient-based optimization with analytic derivatives to allow you to explore large design spaces with hundreds or thousands of design variables, but the framework also has several parallel computing features that can work with gradient-free optimization, mixed-integer nonlinear programming, and traditional design space exploration.

### OpenAeroStruct

<https://github.com/samtx/OpenAeroStruct>

OpenAeroStruct is a lightweight tool that performs aerostructural optimization using OpenMDAO. It couples a vortex-lattice method (VLM) and a 6 degrees of freedom (per node) 3-dimensional spatial beam model to simulate aerodynamic and structural analyses using lifting surfaces. These simulations are wrapped with an optimizer using NASA’s OpenMDAO framework. The analysis and optimization results can be visualized using included tools.
