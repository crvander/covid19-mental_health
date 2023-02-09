    library(tidyverse)

    ## ── Attaching packages ─────────────────────────────────────── tidyverse 1.3.2 ──
    ## ✔ ggplot2 3.4.0      ✔ purrr   1.0.1 
    ## ✔ tibble  3.1.8      ✔ dplyr   1.0.10
    ## ✔ tidyr   1.2.1      ✔ stringr 1.5.0 
    ## ✔ readr   2.1.3      ✔ forcats 0.5.2 
    ## ── Conflicts ────────────────────────────────────────── tidyverse_conflicts() ──
    ## ✖ dplyr::filter() masks stats::filter()
    ## ✖ dplyr::lag()    masks stats::lag()

    library(ggplot2)
    library(haven)

## Covid19 mental health studies

    df <- read_sav("data/Slovenia_COVID-19&Mental_Health.sav")
    head(df, 10)

    ## # A tibble: 10 × 86
    ##    Sex       Sex_Other   Age Educat…¹ Income   Reside…² Region   House…³ Child…⁴
    ##    <dbl+lbl> <chr>     <dbl> <dbl+lb> <dbl+lb> <dbl+lb> <dbl+lb>   <dbl>   <dbl>
    ##  1 2 [Woman] <NA>         56 NA       NA       NA       NA            NA      NA
    ##  2 2 [Woman] <NA>         24  3 [Col…  1 [0 -…  2 [Rur…  2 [Dra…       5       0
    ##  3 2 [Woman] <NA>         46  4 [Mas…  8 [146…  2 [Rur…  2 [Dra…       4       1
    ##  4 2 [Woman] <NA>         23  4 [Mas…  2 [365…  2 [Rur… 10 [Gor…       7       0
    ##  5 2 [Woman] <NA>         32  4 [Mas… 10 [nad…  1 [Urb…  8 [Cen…       1       0
    ##  6 2 [Woman] <NA>         62  1 [Ele…  3 [550…  2 [Rur…  1 [Mur…       5       2
    ##  7 2 [Woman] <NA>         23  2 [Tec…  2 [365…  1 [Urb…  9 [Upp…       2       0
    ##  8 2 [Woman] <NA>         23  2 [Tec…  1 [0 -…  1 [Urb…  8 [Cen…       2       0
    ##  9 1 [Man]   <NA>         23  2 [Tec…  3 [550…  2 [Rur… 10 [Gor…       7       0
    ## 10 2 [Woman] <NA>         23  2 [Tec…  1 [0 -…  1 [Urb…  9 [Upp…       4       0
    ## # … with 77 more variables: Employment <dbl+lbl>, Employment_Other <chr>,
    ## #   Changes_Work <dbl+lbl>, Changes_Work_Other <chr>, Share_Wage <dbl>,
    ## #   Work_Quantity <dbl+lbl>, Increased_Risk <dbl+lbl>,
    ## #   Increased_Risk_Household <dbl+lbl>, Job_Loss <dbl+lbl>,
    ## #   Job_Loss_Risk <dbl+lbl>, Vulnerable <dbl+lbl>,
    ## #   Vulnerable_Closeones <dbl+lbl>, Infection <dbl+lbl>,
    ## #   Infection_Signs <dbl+lbl>, Infection_Probability <dbl+lbl>, …
