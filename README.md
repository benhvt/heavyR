
<!-- README.md is generated from README.Rmd. Please edit that file -->

# heavyR

<!-- badges: start -->
<!-- badges: end -->

The goal of heavyR is to exercice ourself

## Installation

You can install the development version of heavyR like so:

``` r
# FILL THIS IN! HOW CAN PEOPLE INSTALL YOUR DEV PACKAGE?
```

## Example

This is a basic example which shows you how to solve a common problem:

``` r
library(heavyR)
## basic example code
matrice <- cbind(c(1, 2), c(3,4), c(5,6))
matrice
#>      [,1] [,2] [,3]
#> [1,]    1    3    5
#> [2,]    2    4    6
mean_M <- c(0,0)
varcovM <- diag(1, 2)
mvnpdf(matrice, mean_M, varcovM = varcovM, Log = FALSE)
#> $mat
#>      [,1] [,2] [,3]
#> [1,]    1    3    5
#> [2,]    2    4    6
#> 
#> $vect
#> [1] 1.306423e-02 5.931153e-07 9.033134e-15
```

What is special about using `README.Rmd` instead of just `README.md`?
You can include R chunks like so:

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

You’ll still need to render `README.Rmd` regularly, to keep `README.md`
up-to-date. `devtools::build_readme()` is handy for this. You could also
use GitHub Actions to re-render `README.Rmd` every time you push. An
example workflow can be found here:
<https://github.com/r-lib/actions/tree/v1/examples>.

You can also embed plots, for example:

<img src="man/figures/README-pressure-1.png" width="100%" />

In that case, don’t forget to commit and push the resulting figure
files, so they display on GitHub and CRAN.
