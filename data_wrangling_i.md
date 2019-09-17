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

## Including Plots

You can also embed plots, for example:

![](data_wrangling_i_files/figure-gfm/pressure-1.png)<!-- -->
