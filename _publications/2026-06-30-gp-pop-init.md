---
title: "Evaluation of Population Initialization Methods for Genetic Programming-based Symbolic Regression"
collection: publications
date: 2026-06-30
venue: 'EUROCAST 2026: 20th International Conference on Computer Aided Systems Theory'
citation: L. Kammerer, G. Kronberger, D.J. Bartlett, H. Desmond, P.G. Ferreira, S. Winkler (2026). &quot;Evaluation of Population Initialization Methods for Genetic Programming-based Symbolic Regression.&quot; <i>arXiv:22606.31990</i>.
---

[Download paper here](https://arxiv.org/abs/2606.23838)

## Abstract
We analyze the effect of optimizing the initial population of genetic programming (GP) for symbolic regression (SR) on the accuracy and complexity of solutions. We compare three well-established random initialization methods as well as initialization with small optimized solutions from exhaustive symbolic regression (ESR) using a GP/SR implementation which is based on the multi-objective evolutionary algorithm NSGA-II. We compare the final Pareto fronts found with each initialization method on twelve synthetic problems of varying complexity and one real-world dataset. 
We find no significant differences in accuracy or model complexity among the initialization methods. The initial advantage of initialization with ESR  disappears after only a few generations.
Our results show that, given similar diversity in the initial population, the effect of the initialization method in GP-based symbolic regression on the final Pareto front is negligible.

![schematic](/files/2026-06-30-gp-pop-init.png)
*The distribution of test error over complexity of the Pareto-optimal models from each of the 1000 runs for each initialization method in the synthetic Problem 11 after four different numbers of generations. While the ESR-initialized population performs better initially, these differences shrink continuously after ten and 20 generations until they perform equally after 200 generations.*
