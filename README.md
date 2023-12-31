
# concordancer

<!-- badges: start -->
[![R-CMD-check](https://github.com/troyjcross/concordancer/actions/workflows/R-CMD-check.yaml/badge.svg)](https://github.com/troyjcross/concordancer/actions/workflows/R-CMD-check.yaml)
[![](https://www.r-pkg.org/badges/version/concordancer)](https://cran.r-project.org/package=concordancer)
[![](http://cranlogs.r-pkg.org/badges/grand-total/concordancer)](https://cran.r-project.org/package=concordancer)
<!-- badges: end -->


The goal of concordancer is to provide an Rcpp implementation of Lin's Concordance Correlation Coefficient (CCC).

## Installation

Install the latest release from CRAN:

``` r
install.packages("concordancer")
```

You can install the development version of concordancer from [GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("troyjcross/concordancer")
```

## Example

This is a basic example which shows you how to solve a common problem:

``` r
library(concordancer)

# Create x and y
x <- rnorm(100, sd = 1)
y <- rnorm(length(x), sd = 0.5)

# Calculate CCC
result <- ccc(x,y)

print(result)

```

