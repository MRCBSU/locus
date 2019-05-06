## locus – large-scale variational inference for combined covariate and response selection in sparse regression models

[![Travis-CI Build Status](https://travis-ci.org/hruffieux/locus.svg?branch=master)](https://travis-ci.org/hruffieux/locus)

## Overview

**locus** is an R package providing efficient variational algorithms for
simultaneous variable selection of covariates and associated responses based
on multivariate regression models. Dependence across responses linked to the 
same covariates is captured through the model hierarchical structure 
(H. Ruffieux, A. C. Davison, J. Hager, I. Irincheeva, Efficient inference 
for genetic association studies with multiple outcomes, *Biostatistics*, 2017). 

## Warning

**This is a development branch**, it is not guaranteed to be stable at any given time 
and features are subject to change. Please use the [stable version](https://github.com/hruffieux/locus),
unless you want to test and report issues.

## Installation

To install, run the following commands in R:

``` r
require(devtools) # after having installed devtools (install.packages("devtools"))
devtools::install_github("hruffieux/locus", ref = "devel")
```

## Algorithms

The algorithms for joint covariate and response selection provided in **locus**
implement inference for regression models with 

* identity link;
* logistic link;
* probit link;
* identity-probit link.

Inference on models for group selection and based on a spatial Gaussian process to 
encode the dependence structure of the candidate predictors are also implemented. 
Moreover, covariate-level external information variables can be incorporated to 
inform the selection.

## License and authors

This software uses the GPL v2 license, see [LICENSE](LICENSE).
Authors and copyright are provided in [DESCRIPTION](DESCRIPTION). Loris Michel
has also contributed to the development of this project.

## Issues

To report an issue, please use the [locus issue tracker](https://github.com/hruffieux/locus/issues) at github.com.
