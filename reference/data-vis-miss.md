# Return data used to create vis_miss plot

Return data used to create vis_miss plot

Create a tidy dataframe of missing data suitable for plotting

## Usage

``` r
data_vis_miss(x, ...)

# Default S3 method
data_vis_miss(x, ...)

# S3 method for class 'data.frame'
data_vis_miss(x, cluster = FALSE, ...)

# S3 method for class 'grouped_df'
data_vis_miss(x, ...)
```

## Arguments

- x:

  data.frame

- ...:

  extra arguments (currently unused)

- cluster:

  logical - whether to cluster missingness. Default is FALSE.

## Value

data frame

tidy dataframe of missing data

## Examples

``` r
data_vis_miss(airquality)
#> # A tibble: 918 × 4
#>     rows variable valueType value
#>    <int> <chr>    <chr>     <chr>
#>  1     1 Day      FALSE     FALSE
#>  2     1 Month    FALSE     FALSE
#>  3     1 Ozone    FALSE     FALSE
#>  4     1 Solar.R  FALSE     FALSE
#>  5     1 Temp     FALSE     FALSE
#>  6     1 Wind     FALSE     FALSE
#>  7     2 Day      FALSE     FALSE
#>  8     2 Month    FALSE     FALSE
#>  9     2 Ozone    FALSE     FALSE
#> 10     2 Solar.R  FALSE     FALSE
#> # ℹ 908 more rows

if (FALSE) { # \dontrun{
#return vis_dat data for each group
library(dplyr)
airquality |>
  group_by(Month) |>
  data_vis_miss()
} # }
data_vis_miss(airquality)
#> # A tibble: 918 × 4
#>     rows variable valueType value
#>    <int> <chr>    <chr>     <chr>
#>  1     1 Day      FALSE     FALSE
#>  2     1 Month    FALSE     FALSE
#>  3     1 Ozone    FALSE     FALSE
#>  4     1 Solar.R  FALSE     FALSE
#>  5     1 Temp     FALSE     FALSE
#>  6     1 Wind     FALSE     FALSE
#>  7     2 Day      FALSE     FALSE
#>  8     2 Month    FALSE     FALSE
#>  9     2 Ozone    FALSE     FALSE
#> 10     2 Solar.R  FALSE     FALSE
#> # ℹ 908 more rows
```
