---
title: "syren-baryon: Analytic emulators for the impact of baryons on the matter power spectrum"
collection: publications
date: 2025-09-26
venue: 'A&A'
citation: 'L. Kammerer, D.J. Bartlett, G. Kronberger, H. Desmond and P.G. Ferreira (2025). &quot;syren-baryon: Analytic emulators for the impact of baryons on the matter power spectrum.&quot; <i>A&A, 701, A284 </i>.'
---

[Download paper here](https://arxiv.org/abs/2506.08783)

## Abstract
*Context:* Baryonic physics has a considerable impact on the distribution of matter in our Universe on scales probed by current and future cosmological surveys, acting as a key systematic in such analyses. 

*Aims:* We seek simple symbolic parametrisations for the impact of baryonic physics on the matter power spectrum for a range of physically motivated models, as a function of wavenumber, redshift, cosmology, and parameters controlling the baryonic feedback. 

*Methods:* We use symbolic regression to construct analytic approximations for the ratio of the matter power spectrum in the presence of baryons to that without such effects. We obtain separate functions of each of four distinct sub-grid prescriptions of baryonic physics from the CAMELS suite of hydrodynamical simulations (Astrid, IllustrisTNG, SIMBA and Swift-EAGLE) as well as for a baryonification algorithm. We also provide functions which describe the uncertainty on these predictions, due to both the stochastic nature of baryonic physics and the errors on our fits. 

*Results:* The error on our approximations to the hydrodynamical simulations is comparable to the sample variance estimated through varying initial conditions, and our baryonification expression has a root mean squared error of better than one percent, although this increases on small scales. These errors are comparable to those of previous numerical emulators for these models. Our expressions are enforced to have the physically correct behaviour on large scales and at high redshift. Due to their analytic form, we are able to directly interpret the impact of varying cosmology and feedback parameters, and we can identify parameters which have little to no effect.  

*Conclusions:* Each function is based on a different implementation of baryonic physics, and can therefore be used to discriminate between these models when applied to real data. We provide publicly available code for all symbolic approximations found. 

## Code
Implementations of the analytic emulators can be [accessed here](https://github.com/DeaglanBartlett/symbolic_pofk).

![example_pk_suppression](/files/2025-06-11-syren-baryon.png)
*Predicted baryonic suppression of the matter power spectrum, $S$, as a function of wavenumber, $k$, at redshift zero for four randomly sampled hydrodynamical simulations at $z=0$. Our predictions are shown as solid lines, and the shaded regions give the estimated error on these. The dashed lines give the true values measured from the simulations, which are seen to be consistent with our predictions.*
