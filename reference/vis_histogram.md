# Visualise histogram of numeric columns in a data.frame

`vis_histogram` visualises the distribution of every numeric column in a
dataframe and displays it using a faceted ggplot object.

## Usage

``` r
vis_histogram(x, ...)
```

## Arguments

- x:

  a data.frame

- ...:

  Other arguments are passed as geom_histogram arguments.

## Value

`ggplot2` object displaying the guess of the type of values in the data
frame and the position of any missing values.

## Examples

``` r

vis_histogram(airquality, bins = 30)

```
