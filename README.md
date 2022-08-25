<!-- README.md is generated from README.Rmd. Please edit that file -->

# tillsfunctionpackage

<!-- badges: start -->

<!-- badges: end -->

TODO: Describe what the package does... How to write readme: <https://monashbioinformaticsplatform.github.io/2017-11-16-open-science-training/topics/rmarkdown.html>

StableEstim description looks like this:

A collection of methods to estimate the four parameters of stable distributions. The package also provides functions to compute characteristic functions and tools to run Monte Carlo simulations.

The main functions of package StableEstim are briefly described below:

-   main function: Estim() estimates the parameters by various methods. Also gives the associated asymptotic properties of the estimators.
-   estimation functions for specific methods: these functions are called by Estim() but can be used directly, as well. The methods provided so far are:
    -   the maximum-likelihood (MLParametersEstim()),
    -   the generalised method of moments with a finite (GMMParametersEstim()) or continuum moment conditions (CgmmParametersEstim()),
    -   the iterative Koutrouvelis regression method (KoutParametersEstim()),
    -   the fast Kogon-McCulloch method used for first guess estimation (IGParametersEstim).
-   characteristic function: the characteristic function (ComplexCF()) and its Jacobian (jacobianComplexCF()) can be computed and will return a vector (respectively a matrix) of complex numbers.
-   Monte Carlo simulation: a tool to run a Monte Carlo simulation (Estim_Simulation()) is provided and can save output files and/or produce statistical summary.

The package is developed by Tarak Kharrat and Georgi N.Boshnakov.

## Installation

You can install the development version of tillsfunctionpackage from [GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("cedricjuessen/tillsfunctionpackage")
```

## Example

This is a basic example which shows you how to solve a common problem:

``` r
library(tillsfunctionpackage)
## basic example code
```

## Start Delete from here to end

What is special about using `README.Rmd` instead of just `README.md`? You can include R chunks like so:

``` r
summary(cars)
#>      speed           dist       
#>  Min.   : 4.0   Min.   :  2.00  
#>  1st Qu.:12.0   1st Qu.: 26.00  
#>  Median :15.0   Median : 36.00  
#>  Mean   :15.4   Mean   : 42.98  
#>  3rd Qu.:19.0   3rd Qu.: 56.00  
#>  Max.   :25.0   Max.   :120.00
```

You'll still need to render `README.Rmd` regularly, to keep `README.md` up-to-date. `devtools::build_readme()` is handy for this. You could also use GitHub Actions to re-render `README.Rmd` every time you push. An example workflow can be found here: <https://github.com/r-lib/actions/tree/v1/examples>.

You can also embed plots, for example:

<img src="man/figures/README-pressure-1.png" width="100%"/>

In that case, don't forget to commit and push the resulting figure files, so they display on GitHub and CRAN.
