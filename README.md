
<!-- README.md is generated from README.Rmd. Please edit that file -->

# RcppViridis

RcppViridis is designed to map viridis colours to variables

## Installation

Install the development version from
[GitHub](https://github.com/SymbolixAU/RcppViridis) with:

``` r
# install.packages("devtools")
devtools::install_github("SymbolixAU/RcppViridis")
```

## Example

``` r
df <- data.frame(a = 10, x = 1:256)
df$col <- colour_variables(df$x, palette = "viridis")
barplot(height = df$a, col = df$col, border = NA, space = 0)
```

<img src="man/figures/README-unnamed-chunk-4-1.png" width="100%" />

``` r
df <- data.frame(a = 10, x = 1:256)
df$col <- colour_variables(df$x, palette = "plasma")
barplot(height = df$a, col = df$col, border = NA, space = 0)
```

<img src="man/figures/README-unnamed-chunk-5-1.png" width="100%" />

``` r
df <- data.frame(a = 10, x = 1:256)
df$col <- colour_variables(df$x, palette = "magma")
barplot(height = df$a, col = df$col, border = NA, space = 0)
```

<img src="man/figures/README-unnamed-chunk-6-1.png" width="100%" />

``` r
df <- data.frame(a = 10, x = 1:256)
df$col <- colour_variables(df$x, palette = "inferno")
barplot(height = df$a, col = df$col, border = NA, space = 0)
```

<img src="man/figures/README-unnamed-chunk-7-1.png" width="100%" />
