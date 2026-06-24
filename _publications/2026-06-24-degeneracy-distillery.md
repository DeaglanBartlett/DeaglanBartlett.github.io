---
title: "The Degeneracy Distillery"
collection: publications
date: 2026-06-24
venue: 'Submitted'
citation: T.L. Makinen, D.J. Bartlett, N. Jeffrey, B.D. Wandelt (2026). &quot;The Degeneracy Distillery.&quot; <i>arXiv:2606.23838</i>.'
---

[Download paper here](https://arxiv.org/abs/2606.23838)

## Abstract
When two or more parameters or labels produce similar data, they are
*degenerate*, or hard to distinguish.
Degeneracies render both label prediction and inverse problems difficult,
since both machine learning algorithms and probabilistic samplers rely on the
distinguishability of data and its gradients with respect to parameters.
However, identifying degeneracies in physical models or real-world datasets
can be elucidating about the choice of model or the underlying process that
produces the data.
We present the *degeneracy distillery*, a method that
(1) detects and (2) resolves degenerate parameter combinations
(a) automatically and (b) symbolically, from parameter-data
(or parameter-simulation) pairs alone, through estimation and flattening of
the Fisher information matrix. By exploring the information geometry of the likelihood, we characterize degeneracies as an intrinsic property of the physical model, requiring no realised data observation.
We demonstrate our approach on a range of synthetic and real-world problems,
discovering symbolic coordinate transformations that identify the
combinations of parameters of a model which yield independent effects on the
data. The resulting coordinates flatten the Fisher information in expectation *globally*,
in contrast to posterior-based methods that flatten only at a single point, and substantially reduce the simulation budget required for downstream neural posterior estimation. In test cases we require up to $10\times$ fewer simulations for posterior estimation at matched validation calibration whilst simultaneously gaining physical insight on the system. 

![schematic](/files/2026-06-24-degeneracy-distillery.png)
*Degeneracy distillery pipeline in three steps.
(1) Parameter-data pairs $(\theta, \textbf{x})$ are passed to an ensemble of Fishnet networks to learn approximations to the Fisher matrix at each parameter value. (2) A "flattener" network is trained so that its Jacobian maps the learned metric to the identity as a function of $\theta$.
(3) Symbolic regression is performed on each output $\eta$
coordinate to obtain short, nonlinear, degeneracy-resolving expressions.*
