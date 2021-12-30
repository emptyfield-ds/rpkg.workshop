
<!-- README.md is generated from README.Rmd. Please edit that file -->

# rpkg.workshop

<!-- badges: start -->

[![R-CMD-check](https://github.com/emptyfield-ds/rpkg.workshop/workflows/R-CMD-check/badge.svg)](https://github.com/emptyfield-ds/rpkg.workshop/actions)
<!-- badges: end -->

The goal of rpkg.workshop is to download learning materials for
Developing R Packages, as well as to install any required packages.
rpkg.workshop also allows you to open a given module in RStudio Cloud.

## Installation

You can install the latest version of rpkg.workshop with:

``` r
options(repos = c(
  emptyfieldds = "https://emptyfield-ds.r-universe.dev",
  CRAN = "https://cran.rstudio.com/"
))

install.packages("rpkg.workshop")
```

## Installing modules

`use_module()` will install the materials for a given module on your
computer. Then, it will open a new RStudio Project containing the files
you’ll need.

``` r
rpkg.workshop::use_module("module_name")
```

By default, this package downloads the materials to a conspicuous place
like your Desktop. You can also tell `use_module()` exactly where to put
the materials with `destdir`:

``` r
rpkg.workshop::use_module("module_name", destdir = "a/path/on/your/computer")
```

## Opening modules in RStudio Cloud

`browse_cloud()` opens a module in RStudio Cloud, where the materials
and all necessary tooling will be pre-installed. This requires an
RStudio Cloud account.

``` r
rpkg.workshop::browse_cloud("module_name")
```
