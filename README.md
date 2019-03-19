
<!-- README.md is generated from README.Rmd. Please edit that file -->

[![Build
Status](https://api.travis-ci.org/dynverse/dyneval.svg)](https://travis-ci.org/dynverse/dyneval)
[![codecov](https://codecov.io/gh/dynverse/dyneval/branch/master/graph/badge.svg)](https://codecov.io/gh/dynverse/dyneval)
<img src="man/figures/logo.png" align="right" />

# Metrics to compare two trajectories

This R package implements several metrics for comparing two single-cell
trajectories.

These include:

  - **Specific metrics**, metrics which look at the similarity of a
    specific part of the trajectory, such as the topology or the
    cellular
ordering

| Name                       | Long name                          | Category          |
| :------------------------- | :--------------------------------- | :---------------- |
| cor<sub>dist</sub>         | Geodesic distance correlation      | cell positions    |
| MSE<sub>rf</sub>           | Random Forest MSE                  | neighbourhood     |
| NMSE<sub>rf</sub>          | Random Forest Normalised MSE       | neighbourhood     |
| R<sup>2</sup><sub>rf</sub> | Random Forest R²                   | neighbourhood     |
| NMSE<sub>lm</sub>          | Linear regression Normalised MSE   | neighbourhood     |
| MSE<sub>lm</sub>           | Linear regression MSE              | neighbourhood     |
| R<sup>2</sup><sub>lm</sub> | Linear regression R²               | neighbourhood     |
| edgeflip                   | Edge flip                          | topology          |
| HIM                        | Hamming-Ipsen-Mikhailov similarity | topology          |
| Isomorphic                 | isomorphic                         | topology          |
| F1<sub>branches</sub>      | Overlap between the branches       | branch assignment |
| F1<sub>milestones</sub>    | Overlap between the milestones     | branch assignment |

  - **Application metrics**, which assess the accuracy of some
    downstream analyses of trajectories

| Name                     | Long name                               |
| :----------------------- | :-------------------------------------- |
| cor<sub>features</sub>   | Feature importance correlation          |
| wcor<sub>features</sub>  | Feature importance weighted correlation |
| ks<sub>feature</sub>     | Feature importance enrichment ks        |
| wilcox<sub>feature</sub> | Feature importance enrichment wilcox    |

  - **Overall metrics**, which combine several specific and/or
    application metrics to analyse the overall similarity of two
    trajectories

| Name                      | Long name       |
| :------------------------ | :-------------- |
| mean<sub>harmonic</sub>   | Harmonic mean   |
| mean<sub>geometric</sub>  | Geometric mean  |
| mean<sub>arithmetic</sub> | Arithmetic mean |

## Latest changes

Check out `news(package = "dyneval")` or [NEWS.md](inst/NEWS.md) for a
full list of
changes.

<!-- This section gets automatically generated from inst/NEWS.md, and also generates inst/NEWS -->

### Recent changes in dyneval 0.2.3 (unreleased)

  - MINOR CHANGE: update categories of metrics

### Recent changes in dyneval 0.2.2 (21-11-2018)

  - DOCUMENTATION: Update and expand documentation.

  - BUG FIX: Update dyneval for dynwrap 0.3.1 (\#50).

  - MINOR CHANGE: Clean up imports and suggests.
