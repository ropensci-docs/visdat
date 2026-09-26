# Return data used to create vis_cor plot

Return data used to create vis_cor plot

Create a tidy dataframe of correlations suitable for plotting

## Usage

``` r
data_vis_cor(x, ...)

# Default S3 method
data_vis_cor(x, ...)

# S3 method for class 'data.frame'
data_vis_cor(
  x,
  cor_method = "pearson",
  na_action = "pairwise.complete.obs",
  ...
)

# S3 method for class 'grouped_df'
data_vis_cor(x, ...)
```

## Arguments

- x:

  data.frame

- ...:

  extra arguments (currently unused)

- cor_method:

  correlation method to use, from `cor`: "a character string indicating
  which correlation coefficient (or covariance) is to be computed. One
  of "pearson" (default), "kendall", or "spearman": can be abbreviated."

- na_action:

  The method for computing covariances when there are missing values
  present. This can be "everything", "all.obs", "complete.obs",
  "na.or.complete", or "pairwise.complete.obs" (default). This option is
  taken from the `cor` function argument `use`.

## Value

data frame

tidy dataframe of correlations

## Examples

``` r
data_vis_cor(airquality)
#> # A tibble: 36 × 3
#>    row_1   row_2     value
#>    <chr>   <chr>     <dbl>
#>  1 Ozone   Ozone    1     
#>  2 Ozone   Solar.R  0.348 
#>  3 Ozone   Wind    -0.602 
#>  4 Ozone   Temp     0.698 
#>  5 Ozone   Month    0.165 
#>  6 Ozone   Day     -0.0132
#>  7 Solar.R Ozone    0.348 
#>  8 Solar.R Solar.R  1     
#>  9 Solar.R Wind    -0.0568
#> 10 Solar.R Temp     0.276 
#> # ℹ 26 more rows

if (FALSE) { # \dontrun{
#return vis_dat data for each group
library(dplyr)
airquality |>
  group_by(Month) |>
  data_vis_cor()
} # }
data_vis_cor(airquality)
#> # A tibble: 36 × 3
#>    row_1   row_2     value
#>    <chr>   <chr>     <dbl>
#>  1 Ozone   Ozone    1     
#>  2 Ozone   Solar.R  0.348 
#>  3 Ozone   Wind    -0.602 
#>  4 Ozone   Temp     0.698 
#>  5 Ozone   Month    0.165 
#>  6 Ozone   Day     -0.0132
#>  7 Solar.R Ozone    0.348 
#>  8 Solar.R Solar.R  1     
#>  9 Solar.R Wind    -0.0568
#> 10 Solar.R Temp     0.276 
#> # ℹ 26 more rows
```
