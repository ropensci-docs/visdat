# Package index

## Visualise the whole dataframe, class, and missing data

Tools for creating preliminary visualisations to “get a look at the
data”

- [`vis_dat()`](https://docs.ropensci.org/visdat/reference/vis_dat.md) :
  Visualises a data.frame to tell you what it contains.
- [`data_vis_dat()`](https://docs.ropensci.org/visdat/reference/data-vis-dat.md)
  : Return data used to create vis_dat plot
- [`vis_histogram()`](https://docs.ropensci.org/visdat/reference/vis_histogram.md)
  : Visualise histogram of numeric columns in a data.frame

## Focus on the missing data

Specifically display information about the missingness

- [`vis_miss()`](https://docs.ropensci.org/visdat/reference/vis_miss.md)
  : Visualise a data.frame to display missingness.
- [`data_vis_miss()`](https://docs.ropensci.org/visdat/reference/data-vis-miss.md)
  : Return data used to create vis_miss plot

## Compare two dataframes

Only takes dataframes of the same dimensions

- [`vis_compare()`](https://docs.ropensci.org/visdat/reference/vis_compare.md)
  : Visually compare two dataframes and see where they are different.

## Visualise whether a value you expect is in a data frame

Visualise where certain conditions or values are TRUE in your data.

- [`vis_expect()`](https://docs.ropensci.org/visdat/reference/vis_expect.md)
  : Visualise whether a value is in a data frame

## Visualise correlations in a dataframe

Show the correlation amongst variables in simple function

- [`vis_cor()`](https://docs.ropensci.org/visdat/reference/vis_cor.md) :
  Visualise correlations amongst variables in your data as a heatmap
- [`data_vis_cor()`](https://docs.ropensci.org/visdat/reference/data-vis-cor.md)
  : Return data used to create vis_cor plot

## Display the best guess of what each cell contains

Potentially reveal other classes in your dataset

- [`vis_guess()`](https://docs.ropensci.org/visdat/reference/vis_guess.md)
  : Visualise type guess in a data.frame

## Display binary values (0,1) in a data frame

Explore data that is only binary in your data

- [`vis_binary()`](https://docs.ropensci.org/visdat/reference/vis_binary.md)
  : Visualise binary values

## Display the values of each cell

Potentially reveal hidden patterns by seeing scaled values

- [`vis_value()`](https://docs.ropensci.org/visdat/reference/vis_value.md)
  : Visualise the value of data values

## Example data provided with visdat

Data is provided for exploring different functions in visdat

- [`dat_bin`](https://docs.ropensci.org/visdat/reference/dat_bin.md) : A
  small toy dataset of binary data with missings.
- [`typical_data`](https://docs.ropensci.org/visdat/reference/typical_data.md)
  : A small toy dataset of imaginary people
- [`typical_data_large`](https://docs.ropensci.org/visdat/reference/typical_data_large.md)
  : A small toy dataset of imaginary people

## Misc helper functions

Functions that might be useful for users

- [`abbreviate_vars()`](https://docs.ropensci.org/visdat/reference/abbreviate_vars.md)
  : Abbreviate all variables in a data frame
