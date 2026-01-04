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

In SEDs like the one in the previous section, we it's expected that the middle hump follows a distribution known as a modified blackbody. Using the data in the SED above, I used MCMC to fit a modified blackbody with 3 free parameters (mass of the object, temperature, and $\beta$, a parameter relating to the opacity of the object). The gray shaded area shows the 1-$\sigma$ posterior spread, and the plot below shows a corner plot of the posterior distribution.

![](https://github.com/bderieg/bderieg/blob/main/ngc1684_emcee.png)

## Image Processing (Telescope Data)

Below is an example of data taken with the telescope atop the old physics building at the University of Utah in January 2025 as part of a project to measure the brightness of a recent supernova. The left image is the raw, unreduced data from the telescope, and the right image shows a calibrated (science-ready) image. Specifically, multiple frames were combined to improve the signal-to-noise ratio, then a calibration frames were applied to remove any gradients, vignetting, and dark noise (i.e., noise from the pixels themselves). All the code for this can be found in the bderieg/sn_data_reduction repository.

![](https://github.com/bderieg/bderieg/blob/main/before_after.png)
