
<!-- README.md is generated from README.Rmd. Please edit that file -->

# featurette git repo

<!-- badges: start -->

<!-- badges: end -->

The goal of featurette is to feature and test out development projects.

  - [2023-10-28-diamonds-barlabs/diamonds-barlabs.html](https://evamaerey.github.io/featurette/2023-10-28-diamonds-barlabs/diamonds-barlabs.html)
  - [2023-10-26-tswift-keys/tswift-keys.html](https://evamaerey.github.io/featurette/2023-10-26-tswift-keys/tswift-keys.html)
  - [2023-10-26-horror-articles/horror-articles.html](https://evamaerey.github.io/featurette/2023-10-26-horror-articles/horror-articles.html)
  - [2023-10-25-tswift-keys/tswift-keys.html](https://evamaerey.github.io/featurette/2023-10-25-tswift-keys/tswift-keys.html)
  - [2023-09-13-ggcirclepack-global-human-day/global\_human\_day.html](https://evamaerey.github.io/featurette/2023-09-13-ggcirclepack-global-human-day/global_human_day.html)

-----

# code to write new featurette

``` r
new_experiment <- function(name){
  
  dir <- paste0(Sys.Date(),"-", name)
  
  dir.create(dir)
  readLines("template.Rmd") |>
    writeLines(con = paste0(dir,"/", name, ".Rmd"))
  
} 

new_experiment("diamonds-barlabs")
```
