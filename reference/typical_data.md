# A small toy dataset of imaginary people

A dataset containing information about some randomly generated people,
created using the excellent `wakefield` package. It is created as
deliberately messy dataset.

## Usage

``` r
typical_data
```

## Format

A data frame with 5000 rows and 11 variables:

- ID:

  Unique identifier for each individual, a sequential character vector
  of zero-padded identification numbers (IDs). see ?wakefield::id

- Race:

  Race for each individual, "Black", "White", "Hispanic", "Asian",
  "Other", "Bi-Racial", "Native", and "Hawaiin", see ?wakefield::race

- Age:

  Age of each individual, see ?wakefield::age

- Sex:

  Male or female, see ?wakefield::sex

- Height(cm):

  Height in centimeters, see ?wakefield::height

- IQ:

  vector of intelligence quotients (IQ), see ?wakefield::iq

- Smokes:

  whether or not this person smokes, see ?wakefield::smokes

- Income:

  Yearly income in dollars, see ?wakefield::income

- Died:

  Whether or not this person has died yet., see ?wakefield::died
