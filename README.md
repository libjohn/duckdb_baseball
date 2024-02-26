# README

<!-- badges: start -->

<!-- badges: end -->

```
library(Lahman)
library(tidyverse)


batting <- copy_to(con, Lahman::Batting)
batting

batting %>% show_query()
batting %>% explain()

batting |> 
  count(teamID, sort = TRUE)
```