---
permalink: /research/
title: "Research Projects"
author_profile: true
redirect_from:
  - /md/
  - /research.html
---

## Nonlinear matrix recovery

The problem of nonlinear matrix recovery consists in estimating a matrix based on incomplete observations (affine measurements), under the assumptions that the columns of the matrix satisfy a specific geometric structure. Structures where nonlinear matrix recovery is known to be efficient include data scattered in clusters and algebraic varieties (e.g. unions of several linear subspaces).

Our code is based on the resolution of a nonconvex optimization problem, using [Riemannian optimization solvers](https://manopt.org). The code in both Matlab and Python is available on [Github](https://github.com/flgoyens/nonlinear-matrix-recovery) and is based on the research presented in this [paper](https://arxiv.org/abs/2109.06095).

## Point cloud registration on algebraic varieties


The registration problem consists in finding a transformation between two point clouds which describe the same object in different coordinate systems.

<!-- ![Registration image](/images/registration_image.png) -->

<img src="http://flgoyens.github.io/images/registration_image.png" width="800" height="200" />

Our code is based on the resolution of a nonconvex optimization problem, using [Riemannian optimization solvers](https://manopt.org). The code in both Matlab and Python is available on [Github](https://github.com/flgoyens/variety-registration). This package is described in Chapter 5 of [my doctoral thesis](http://flgoyens.github.io/files/dphil_thesis.pdf). A standalone paper is currently in preparation.
