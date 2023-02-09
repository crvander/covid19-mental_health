---
title: "R Notebook"
author: "Carlos van der Ley"
date: "02-08-2023"
output:
  html_document: 
    keep_md: yes
    

---


```r
library(tidyverse)
library(ggplot2)
library(haven)
library(data.table)
```


```r
df <- read_sav("data/Slovenia_COVID-19&Mental_Health.sav")
data.table(head(
  df |>
    select(Sex:Income), 10)
)
```

```
##     Sex Sex_Other Age Education Income
##  1:   2      <NA>  56        NA     NA
##  2:   2      <NA>  24         3      1
##  3:   2      <NA>  46         4      8
##  4:   2      <NA>  23         4      2
##  5:   2      <NA>  32         4     10
##  6:   2      <NA>  62         1      3
##  7:   2      <NA>  23         2      2
##  8:   2      <NA>  23         2      1
##  9:   1      <NA>  23         2      3
## 10:   2      <NA>  23         2      1
```
