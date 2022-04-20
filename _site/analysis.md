Lab 03 - Using Propensity Scores
================
Lucy D’Agostino McGowan
2022-03-29

``` r
library(tidyverse)
library(smd)
```

## Exercise 1

``` r
df <- read_csv("coffee_town_df.csv")
```

    ## 
    ## ── Column specification ────────────────────────────────────────────────────────
    ## cols(
    ##   coffee_town = col_double(),
    ##   cups_of_coffee = col_double(),
    ##   age = col_double(),
    ##   job = col_character(),
    ##   smoke = col_character()
    ## )

``` r
head(df)
```

    ## # A tibble: 6 × 5
    ##   coffee_town cups_of_coffee   age job   smoke
    ##         <dbl>          <dbl> <dbl> <chr> <chr>
    ## 1           1              0  12.1 none  never
    ## 2           0              0  14.6 none  never
    ## 3           1              0  11.5 none  never
    ## 4           0              1  18.8 easy  never
    ## 5           0              0  15.0 none  never
    ## 6           1              0  11.5 none  never
