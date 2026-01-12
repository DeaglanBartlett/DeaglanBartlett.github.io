---
title: "Symbolically regressing dark matter halo profiles using weak lensing"
collection: publications
date: 2026-01-08
venue: 'MNRAS (Submitted)'
citation: 'A. Martín, T. Yasin, D.J. Bartlett, H. Desmond and P.G. Ferreira (2026). &quot;Symbolically regressing dark matter halo profiles using weak lensing.&quot; <i>arXiv:2601.05203</i>.'
---

[Download paper here](https://arxiv.org/abs/2601.05203)

## Abstract
The structure of dark matter haloes is often described by radial density profiles motivated by cosmological simulations. These are typically assumed to have a fixed functional form (e.g. NFW), with some free parameters that can be constrained with observations. However, relying on simulations has the disadvantage that the resulting profiles depend on the dark matter model and the baryonic physics implementation, which are highly uncertain. Instead, we present a method to constrain halo density profiles directly from observations. This is done using a symbolic regression algorithm called Exhaustive Symbolic Regression (ESR). ESR searches for the optimal analytic expression to fit data, combining both accuracy and simplicity. We apply ESR to a sample of $149$ galaxy clusters from the HSC-XXL survey to identify which functional forms perform best across the entire sample of clusters. We identify density profiles that statistically outperform NFW under a minimum-description-length criterion. 
Within the radial range probed by the weak-lensing data ($R \sim 0.3 - 3$ h$^{-1}$ Mpc), the highest-ranked ESR profiles exhibit shallow inner behaviour and a maximum in the density profile. However, the inner slope itself remains weakly constrained due to limited signal at small radii. As a practical application, we show how the best-fitting ESR models can be used to obtain enclosed mass estimates. We find masses that are, on average, higher than those derived using NFW, highlighting a source of potential bias when assuming the wrong density profile. These results have important knock-on effects for analyses that utilise clusters, for example cosmological constraints on $\sigma_8$ and $\Omega_\text{m}$ from cluster abundance and clustering. Beyond the HSC dataset, the method is readily applicable to any data constraining the dark matter distribution in galaxies and galaxy clusters, such as other weak lensing surveys, galactic rotation curves, or complementary probes. 

![halo_example](/files/2026-01-08-lensing-halo.png)
*Plots of the top 2 best-fitting functions, together with the top analytically integrable functions discussed in the text. The NFW profile is also shown for comparison. 
The top panels correspond to cluster XLSSC 91, which has the highest SNR in the sample, while the bottom panels show cluster XLSSC 101, which is a medium SNR cluster. 
These two clusters are also shown in Fig. 1.
Left panels: ESD fits to the data. The horizontal dashed line marks zero.
Right panels: Corresponding density profiles plotted over a wide radial range. The vertical dashed lines indicate the radial range covered by the data. Shaded regions represent the 68% credible intervals derived from the posterior parameter distributions.*
