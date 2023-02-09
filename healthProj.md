    library(tidyverse)
    library(ggplot2)
    library(haven)
    library(DT)

## Covid19 mental health studies

    df <- read_sav("data/Slovenia_COVID-19&Mental_Health.sav")

    datatable(head(df |>
                select(Sex:Income), 10)
    )

<div class="datatables html-widget html-fill-item-overflow-hidden html-fill-item" id="htmlwidget-f0984a1799850d0be7dd" style="width:100%;height:auto;"></div>
<script type="application/json" data-for="htmlwidget-f0984a1799850d0be7dd">{"x":{"filter":"none","vertical":false,"data":[["1","2","3","4","5","6","7","8","9","10"],[2,2,2,2,2,2,2,2,1,2],[null,null,null,null,null,null,null,null,null,null],[56,24,46,23,32,62,23,23,23,23],[null,3,4,4,4,1,2,2,2,2],[null,1,8,2,10,3,2,1,3,1]],"container":"<table class=\"display\">\n  <thead>\n    <tr>\n      <th> <\/th>\n      <th>Sex<\/th>\n      <th>Sex_Other<\/th>\n      <th>Age<\/th>\n      <th>Education<\/th>\n      <th>Income<\/th>\n    <\/tr>\n  <\/thead>\n<\/table>","options":{"columnDefs":[{"className":"dt-right","targets":[1,3,4,5]},{"orderable":false,"targets":0}],"order":[],"autoWidth":false,"orderClasses":false}},"evals":[],"jsHooks":[]}</script>
