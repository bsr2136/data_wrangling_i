Data Import
================
Barik Rajpal

## Load in a Dataset

``` r
## Do something that reads in a dataset

litters_data <- read_csv("./Data/FAS_litters.csv")
litters_data <- janitor::clean_names(litters_data)

pups_data <- read_csv("./Data/FAS_pups.csv")
pups_data <- janitor::clean_names(pups_data)
```

## Importing in other ways

``` r
litters_data = read_csv(file = "./Data/FAS_litters.csv",
    col_types = cols(
    Group = col_character(),
    `Litter Number` = col_character(),
    `GD0 weight` = col_double(),
    `GD18 weight` = col_double(),
    `GD of Birth` = col_integer(),
    `Pups born alive` = col_integer(),
    `Pups dead @ birth` = col_integer(),
    `Pups survive` = col_integer()
    )
)
```

## Same but XL

``` r
mlb_data <- read_excel("./Data/mlb11.xlsx")
```

## Read in SAS …

``` r
pulse_data <- haven::read_sas("./Data/public_pulse_data.sas7bdat")
```
