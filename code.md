```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE)
```

```{r}
library(tidyverse)
library(ggplot2)
library(haven)
```

## Covid19 mental health studies

```{r}
df <- read_sav("data/Slovenia_COVID-19&Mental_Health.sav")
head(df, 10)
```