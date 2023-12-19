diamond-sizes
================
Anubha Nagar
31/08/2021

``` r
library(ggplot2)
library(dplyr)
```

    ## 
    ## Attaching package: 'dplyr'

    ## The following objects are masked from 'package:stats':
    ## 
    ##     filter, lag

    ## The following objects are masked from 'package:base':
    ## 
    ##     intersect, setdiff, setequal, union

``` r
smaller <- diamonds %>% 
  filter(carat <= 2.5)
```

We have data about 53940 diamonds. Only 126 are larger than 2.5 carats.
The distribution of the remainder is shown below:

![](Diamond-sizes_files/figure-gfm/unnamed-chunk-2-1.png)<!-- -->

# Striking features:

-   Buyers prefer buying less than 1 carat diamonds since it’s cheaper.

-   If a buyers wants to buy above 1 carat they prefer buying 1 carat,
    1.5 carat, 2 carat(people barely buy between these values).

-   Very less people buy diamonds below 0.25 carat and above 2 carat.

-   Maximum diamonds are bought around 0.25 carat since its the
    cheapest.
