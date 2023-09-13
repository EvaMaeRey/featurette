
<!-- README.md is generated from README.Rmd. Please edit that file -->

# featurette git repo

<!-- badges: start -->

<!-- badges: end -->

The goal of featurette is to feature projects.

  - [2023-09-13-global\_human\_day/global\_human\_day.html](https://evamaerey.github.io/featurette/2023-09-13-global_human_day/global_human_day.html)

-----

# code to write new featurette

``` r
new_experiment <- function(name){
  
  dir <- paste0(Sys.Date(),"-", name)
  
  dir.create(dir)
  readLines("template.Rmd") |>
    writeLines(con = paste0(dir,"/", name, ".Rmd"))
  
} 

new_experiment("global_human_day")
```
