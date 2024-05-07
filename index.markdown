---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Home
---

## Project overview 

Numerical resolution is widely considered to be a dominant factor in numerical model fidelity, driving earth system models (ESMs) toward the smallest horizontal resolution possible for a given application. However, increasing horizontal resolution comes with significant computational costs, placing substantial constraints on the resolution global ESMs can achieve when simulating long-term climate variability. Yet there is strong interest in understanding both how climate variability affects coastal regions – in order to provide actionable projections – and how unresolved processes in the open ocean may affect the global climate simulations, both of which require resolution at least an order of magnitude higher than current global ESMs can provide. This project focuses on improved representations of small-scale coastal and open-ocean processes such as river plumes, coastal fronts, and meso- and submesoscale eddy processes. We will do this by creating and evaluating a new component of the Energy Exascale Earth System Model (E3SM), based on the Regional Ocean Modeling System (ROMS), a community standard coastal ocean model that has been in use for over two decades. Through coupling with E3SM’s MPAS-O global ocean component we will investigate the representation of small-scale processes across model resolution, targeting improvements in the fidelity with which E3SM resolves nonlinear ocean dynamics.


## Scientific Objectives

Our overarching goal is to improve the ability of E3SM to model oceans with higher fidelity than currently possible. To achieve this goal, we plan to pursue the following two specific objectives 
 1. Extend the resolution capabilities of MPAS-O through coupling with a limited-domain, high-resolution, regional ocean model (ROMS), 
 2. Create a scientific and technical framework for efficient and robust two-way coupling of ROMS within MPAS-O that exploits the latest HPC architectures.
We will target project objectives outlined above through three tasks: 
 1.  Assess and improve representation of small-scale coastal and open-ocean processes — such as river plumes, coastal fronts, and meso- and submesoscale  - eddy processes — in the context of global ESMs
 2. Design and implement a scientific and technical framework for two-way coupling between ROMS and MPAS-O for optional, flexible, efficient, and robust dynamical up- and downscaling 
 3. Implement a new version of ROMS [REMORA](https://remora-ocean.readthedocs.io/en/latest/) that is performance portable and can run effectively on hardware from laptops to the cutting-edge architectures, and is able to exploit the different graphical processing units available on those machines
We expect this new coupled modeling framework will greatly enhance our understanding of both how coastal regions are affected by climate change and what local feedbacks are important in altering larger scale climate signals. The methodologies we develop will be directly translatable to other structured-grid regional models (such as MOM6, NEMO, GETM) and informative for unstructured-grid nesting for models (such as FVCOM, Thetis, and SCHISM). We also expect this work to improve representation of meso- and submesoscale fields, shown in various recent works to be critical for the faithful resolution of large-scale volume transport, important for e.g., Atlantic Meridional Overturning Circulation, as well as climate feedbacks including El Nino Southern Oscillation and sea-ice cover.

Specific technological advances include an MPAS-O upgraded with support for regional and coastal coupling with subgrid models (e.g., ROMS), enhanced limited-domain modeling capabilities through support for additional open boundary conditions, online numerical mixing estimates, support for additional subgrid momentum tendencies to represent the effect of subgrid turbulence effects, and a performance-portable version of ROMS for heterogeneous architectures with the ability to function as a standalone code available to the ocean modeling community with easy-to-use wrappers and drivers.
