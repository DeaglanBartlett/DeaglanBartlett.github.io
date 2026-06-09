---
title: "CMBolic: Symbolic emulators for the Cosmic Microwave Background. I. Lensing"
collection: publications
date: 2026-06-05
venue: 'A&A (Submitted)'
citation: 'D.M.J. Vokrouhlicky, C. Skordis, D.J. Bartlett, H. Desmond, P.G. Ferreira (2026). &quot;CMBolic: Symbolic emulators for the Cosmic Microwave Background. I. Lensing.&quot; <i>arXiv:2606.07745</i>.'
---

[Download paper here](https://arxiv.org/abs/2606.07745)

## Abstract
We present the first installment of CMBolic: a suite of symbolic cosmic microwave background (CMB) emulators. In this instance,
we emulate the CMB lensing potential power spectrum $C_\ell^{\phi\phi}$ for the widely used extended $\Lambda$CDM model which simultaneously includes massive neutrinos
and evolving dark energy modelled using the Chevallier-Polarski-Linder (CPL) parameterization. 
We achieve comparable precision to existing neural network emulators, with the added benefit of simpler handling as our emulators are analytic functions of the model parameters and multipole $\ell$. 
On independent validation spectra evaluated in the range $2\leq \ell \leq 5500$, CMBolic achieves mean absolute fractional errors of 0.27% in the $\Lambda$CDM subspace and 0.32% across the 
full extended parameter space. This emulation error is well below even the most optimistic noise forecasts from CMB Stage 4 experiments. 
We apply CMBolic to cosmological parameter estimation with Bayesian inference using the lensing-only likelihoods from ACT DR6 and Planck.
We show excellent agreement between the posteriors obtained by CMBolic and the
Boltzmann code CLASS.
This demonstrates the practical use of CMBolic on cosmological parameter estimation, reducing the runtime from 2 weeks to under 3 minutes. 

## Code
Symbolic emulators are available as a part of the CMBolic suite on GitHub in various languages for simple usage, as well as the implementation of our emulator as a theory class in Cobaya:
[access here](https://github.com/dvokrouhlicky/CMBolic).

![nonlinear_prescription_comparison_with_cmbolic](/files/2026-06-05-cmbolic-lensing.png)
*Comparison of nonlinear matter-power prescriptions for a Planck-like fiducial cosmology. The upper panel shows the scaled lensing-potential spectrum for HMcode 2020, Halofit, the linear matter power spectrum, and CMBolic. The lower panel shows fractional differences relative to HMcode 2020, the prescription used to generate the CMBolic training data. The CMBolic residual for the fiducial cosmology and the 68% and 95% validation residual bands, shown in red and highlighted in the inset, are much smaller than these modelling differences.*
