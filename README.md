# Benjamin J. Derieg

I'm currently a second-year graduate student in physics at the University of Utah, and will graduate with my M.S. in 2026. My research here has focused on simulating black hole critical phenomena using numerical general relativity. I also have research experience in observational astronomy from my time at BYU. This helped me develop a wide variety of data-analysis skills that were backed up by my coursework at both universities (i.e., various computer science, computational physics, and statistics/modeling classes).

Below I give some samples of skills that I've developed through my research or coursework. All the code for these can be found in the repositories in my Github.

## Table of Contents

1. [Data Collection](#data-collection)
2. [MCMC](#mcmc)
3. [Image Processing (Telescope Data)](image-processing-telescope-data)

## Data Collection

The bderieg/autoap2 repository contains the code to build spectral energy distributions (SEDs) for early-type galaxies from a combination of aperture photometry on raw space-telescope data (from Hubble, Herschel, IRAS, WISE, etc.) and pre-existing measurements from the NASA/IPAC Extragalactic Database (NED). Below is an example of this for one galaxy.

![](https://github.com/bderieg/bderieg/blob/main/sed_w_alma.png)

The black points and error bars were gathered using aperture photometry on raw images. Examples of the images used for the data (and apertures) are shown in the insets. The red point was gathered automatically from NED. The red dash-dot line is a multi-parameter fit (specifically, a modified blackbody) to the 6 black points in the middle (see next section).

## MCMC

(...work in progress...)

![](https://github.com/bderieg/bderieg/blob/main/ngc1684_emcee.png)

## Image Processing (Telescope Data)
