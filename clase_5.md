Clase 5. Manipulación de datos
================
SVR
22-03-2022

Hello There!

``` r
library(tidyverse)
```

    ## Warning: package 'tidyverse' was built under R version 4.1.2

    ## -- Attaching packages --------------------------------------- tidyverse 1.3.1 --

    ## v ggplot2 3.3.5          v purrr   0.3.4     
    ## v tibble  3.1.5          v dplyr   1.0.7     
    ## v tidyr   1.1.4          v stringr 1.4.0.9000
    ## v readr   2.0.2          v forcats 0.5.1

    ## -- Conflicts ------------------------------------------ tidyverse_conflicts() --
    ## x dplyr::filter() masks stats::filter()
    ## x dplyr::lag()    masks stats::lag()

``` r
library(palmerpenguins)


penguins %>% 
  count(species)
```

    ## # A tibble: 3 x 2
    ##   species       n
    ##   <fct>     <int>
    ## 1 Adelie      152
    ## 2 Chinstrap    68
    ## 3 Gentoo      124

``` r
ggplot(penguins) +
  geom_bar(aes(x = species, fill = species))
```

![](clase_5_files/figure-gfm/unnamed-chunk-1-1.png)<!-- -->
