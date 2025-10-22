---
title: "Symbolic Emulators for Cosmology: Accelerating Cosmological Analyses Without Sacrificing Precision"
collection: publications
date: 2025-10-22
venue: 'Philosophical Transactions A (Submitted)'
citation: 'D.J. Bartlett, and S. Pandey (2025). &quot;Symbolic Emulators for Cosmology: Accelerating Cosmological Analyses Without Sacrificing Precision.&quot; <i>arXiv:2510.18749</i>.'
---

[Download paper here](https://arxiv.org/abs/2510.18749)

## Abstract
In cosmology, emulators play a crucial role by providing fast and accurate predictions of complex physical models, enabling efficient exploration of high-dimensional parameter spaces that would be computationally prohibitive with direct numerical simulations. Symbolic emulators have emerged as promising alternatives to numerical approaches, delivering comparable accuracy with significantly faster evaluation times. While previous symbolic emulators were limited to relatively narrow prior ranges, we expand these to cover the parameter space relevant for current cosmological analyses. 
We introduce approximations to hypergeometric functions used for the $\Lambda$CDM comoving distance and linear growth factor which are accurate to better than 0.001\% and 0.05\%, respectively, for all redshifts and for $\Omega_{\rm m} \in [0.1, 0.5]$.
We show that integrating symbolic emulators into a Dark Energy Survey-like $3\times2$pt analysis produces cosmological constraints consistent with those obtained using standard numerical methods. Our symbolic emulators offer substantial improvements in speed and memory usage, demonstrating their practical potential for scalable, likelihood-based inference.

## Code
Implementations of the analytic emulators can be [accessed here](https://github.com/DeaglanBartlett/symbolic_pofk).

![hyper_error](/files/2025-10-22-wider-syren-hyper.png)
*Fractional errors on our approximations to the hypergeometric functions required to evaluate the radial comoving distance (left) and linear growth factor (right) for a $\Lambda$CDM cosmology. In both cases, $x \equiv a^3 (\Omega_{\rm m} - 1) / \Omega_{\rm m}$, for scale factor $a$ and present-day matter density parameter $\Omega_{\rm m}$. The approximations were obtained for $x$ in the grey shaded region (corresponding to the prior range in Table 1), and they thus show very good extrapolation behaviour, particularly for values of $x$ relevant for cosmology (red hatched region).*

![corner_all](/files/2025-10-22-wider-syren-corner.png)
*Marginalised posterior distributions of all parameters considered in our mock DES-Y1 analysis. The `exact' model is computed using CAMB, and we see that its contours (red) are very similar to those obtained using our symbolic emulators (blue), demonstrating that the emulators are sufficiently accurate for such an analysis. This is in contrast to applying HALOFIT to the E&H approximation (green contours), for which significant discrepancies are seen.*