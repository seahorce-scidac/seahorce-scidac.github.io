---
layout: page
title: Research
permalink: /research/
order: 1
---

<a href="https://ui.adsabs.harvard.edu/search/q=klion%2C%20h&sort=date%20desc%2C%20bibcode%20desc&p_=0" target="_blank">ADS</a> \| <a href="https://scholar.google.com/citations?hl=en&user=Td1D_bsAAAAJ&view_op=list_works&sortby=pubdate" target="_blank">Google Scholar</a> \| <a href="https://www.github.com/hklion" target="_blank">Github</a>

### Astrophysical Plasmas and Reconnection with WarpX

### Kilonova Light Curves with Sedona
My PhD thesis focused on understanding the light we see from neutron star mergers
(kilonovae). I used multidimensional hydrodynamic and radiation transport simulations to predict trends in kilonova light curves. My focus was on the effects of the relativistic jet that's embedded in the radioactive ejecta.

<img align="right" style="padding-left: 15px; padding-bottom: 15px" src="/files/sedona.png" width="200">
My primary tool is Sedona, a 3D Monte Carlo radiation transport code, which I also develop. My development work has mostly focused on performance and parallelization, with the goal of improving the code's speed and scalability on supercomputers like [NERSC's](https://www.nersc.gov/) [cori](https://docs.nersc.gov/systems/cori/). Projects I've undertaken include:
 - Implementing checkpointing and restarting (including saving and restoring the state of the random number generators)
 - Adding multithreading to the opacity and temperature calculations
 - Finding and resolving HDF5 errors and memory leaks
 - Benchmarking and scaling tests
 - Updating makefiles and build workflow, and modernizing the development workflow

### Non-Blocking MPI Collectives in FLASH
<img align="left" style="padding-right: 15px; padding-bottom: 15px" src="/files/sc17.png" width="300">
Communication and calculations can both be time-consuming for high-performance codes, but use different resources. If possible, it can be advantageous to overlap them. I implemented this strategy in FLASH, a 3D multiphysics code, overlapping the calculation-heavy nuclear reaction network with the communication-heavy self-gravity solver. I tested the scaling and performance of this approach, and found that its effectiveness depended greatly on the MPI implementation used. I presented a peer-reviewed [poster](https://www.dropbox.com/sh/ixa8axlcce1zwmk/AABQ8wqIJYwoKaKU0-sK6Q76a?dl=0) on this project at Supercomputing17.


### Red Giant Asteroseismology & Rotation

Asteroseismic observations of red giants provided the first direct measurements of stellar core rotation rates. While this confirmed that red giant surfaces rotate more solwly than their cores, the interior rotation profiles remain unconstrained. Namely, whether the differential rotation is concentrated near the core, or whether it is spread out through the convective envelope. We developed a simple diagnostic for estimating the location of the differential rotation based on ratios of rotational splittings and an independent surface rotation measurement. It is less precise than traditional methods for finding rotational profiles, but it is less sensitive to the stellar models used and is less time consuming.
