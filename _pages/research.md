---
title: "Research"
permalink: /research/
author_profile: true
---

My research develops statistical and machine-learning methods for extracting information from cosmological data. I focus on connecting realistic simulations to Bayesian inference, working with the large-scale structure as a field rather than a collection of summary statistics, and building interpretable models that make scientific predictions faster and easier to test.

## Simulation-Based Inference

Cosmological observations are shaped by nonlinear structure formation, complex survey effects and uncertain astrophysical processes. Simulation-based inference makes it possible to constrain cosmological models using forward simulations of these processes, without requiring a tractable analytic likelihood. My work explores how to build this approach around informative summaries of galaxy clustering and how to obtain reliable, calibrated parameter constraints from realistic simulated data.
See [LTU-ILI](/publications/2024-02-09-ltu-ili/) for a publicly released code which
can help incroporate simulation based inference into your astrophysics/cosmology pipeline.

![pipeline](/files/2024-02-09-ltu-ili.png)

## Accelerating Cosmological Simulations with ML

Large cosmological simulations are essential for interpreting current and upcoming surveys, but their computational cost limits the volumes, resolutions and number of model evaluations that can be explored. I work on machine-learning methods that reduce this cost while retaining physical accuracy, rather than treating a fast emulator as an unchecked replacement for the underlying simulation.

For example, [COCA](/publications/2024-09-05-coca/) couples a learned frame of reference to an N-body simulator. The equations of motion are still solved, allowing force evaluations to correct errors in the learned prediction.

![coca_diagram](/files/coca_diagram.png)

## Symbolic Regression

Symbolic regression searches for equations that describe data, producing explicit mathematical expressions rather than opaque fitted models. This makes it useful both for scientific discovery and for creating fast, differentiable approximations that can be inspected and used in downstream analyses.

In [Exhaustive Symbolic Regression](/publications/2023-05-26-esr/), the space of candidate expressions is systematically ranked using a principled trade-off between fit and complexity, which can be extended by using language models as [priors](/publications/2023-07-24-priors-sr/). I also apply symbolic regression to cosmological emulation, including analytic models for the [linear matter power spectrum](/publications/2023-11-28-sr-linear-pofk/), [nonlinear structure formation](/publications/2024-02-28-syren-halofit/), [baryonic effects](/publications/2025-06-11-syren-baryon/) and for parameterising [dust attenuation](/publications/2026-06-08-ltu-dust/) in galaxies.

![planck_fit](/files/2023-11-28-sr-linear-pofk.png)

## Field-Level Inference

Many analyses reduce observations to a small set of summary statistics or focus on selected objects. Field-level inference instead uses the spatially resolved maps of matter or radiation, aiming to retain more of the information in the data while accounting for the physical processes that connect latent cosmic structure to observations.

My work includes Bayesian analyses of the nearby Universe using constrained simulations and full-sky maps. For example, a [field-level search for dark-matter annihilation and decay](/publications/2022-11-29-flat/) uses the large-scale distribution of matter to build gamma-ray templates and constrain dark-matter interactions, rather than restricting the analysis to a list of individual targets.

![dm_ann](/files/flat_skymap.png)

For a complete list of papers, see the [Publications page](/publications/).