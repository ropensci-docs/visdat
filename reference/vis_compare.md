# Visually compare two dataframes and see where they are different.

`vis_compare`, like the other `vis_*` families, gives an at-a-glance
ggplot of a dataset, but in this case, hones in on visualising **two**
different dataframes of the same dimension, so it takes two dataframes
as arguments.

## Usage

``` r
vis_compare(df1, df2)
```

## Arguments

- df1:

  The first dataframe to compare

- df2:

  The second dataframe to compare to the first.

## Value

`ggplot2` object displaying which values in each data frame are present
in each other, and which are not.

## See also

[`vis_miss()`](https://docs.ropensci.org/visdat/reference/vis_miss.md)
[`vis_dat()`](https://docs.ropensci.org/visdat/reference/vis_dat.md)
[`vis_guess()`](https://docs.ropensci.org/visdat/reference/vis_guess.md)
[`vis_expect()`](https://docs.ropensci.org/visdat/reference/vis_expect.md)
[`vis_cor()`](https://docs.ropensci.org/visdat/reference/vis_cor.md)

## Examples

``` r

# make a new dataset of iris that contains some NA values
aq_diff <- airquality
aq_diff[1:10, 1:2] <- NA
vis_compare(airquality, aq_diff)
```
