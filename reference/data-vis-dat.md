# Return data used to create vis_dat plot

Return data used to create vis_dat plot

## Usage

``` r
data_vis_dat(x, ...)

# Default S3 method
data_vis_dat(x, ...)

# S3 method for class 'data.frame'
data_vis_dat(x, ...)

# S3 method for class 'grouped_df'
data_vis_dat(x, ...)
```

## Arguments

- x:

  data.frame

- ...:

  extra arguments (currently unused)

## Value

data frame

## Examples

``` r
data_vis_dat(airquality)
#> # A tibble: 918 × 4
#>     rows variable valueType value
#>    <int> <chr>    <chr>     <chr>
#>  1     1 Day      integer   41   
#>  2     1 Month    integer   190  
#>  3     1 Ozone    integer   7.4  
#>  4     1 Solar.R  integer   67   
#>  5     1 Temp     integer   5    
#>  6     1 Wind     numeric   1    
#>  7     2 Day      integer   36   
#>  8     2 Month    integer   118  
#>  9     2 Ozone    integer   8    
#> 10     2 Solar.R  integer   72   
#> # ℹ 908 more rows

if (FALSE) { # \dontrun{
#return vis_dat data for each group
library(dplyr)
airquality |>
  group_by(Month) |>
  data_vis_dat()
} # }
```
