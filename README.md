
<!-- README.md is generated from README.Rmd. Please edit that file -->

# featurette git repo

<!-- badges: start -->

<!-- badges: end -->

The goal of featurette is to feature and test out projects and
packages\!

Repo: <https://github.com/EvaMaeRey/featurette>

0.  [template.html](https://evamaerey.github.io/featurette/template.html)
    **[source](https://github.com/evamaerey/featurette/blob/master/template.Rmd)**
1.  [2023-11-07-ggplot-pie-charts/ggplot-pie-charts.html](https://evamaerey.github.io/featurette/2023-11-07-ggplot-pie-charts/ggplot-pie-charts.html)
    **[source](https://github.com/evamaerey/featurette/blob/master/2023-11-07-ggplot-pie-charts/ggplot-pie-charts.Rmd)**
2.  [2023-11-02-help-quote-mtcars/help-quote-mtcars.html](https://evamaerey.github.io/featurette/2023-11-02-help-quote-mtcars/help-quote-mtcars.html)
    **[source](https://github.com/evamaerey/featurette/blob/master/2023-11-02-help-quote-mtcars/help-quote-mtcars.Rmd)**
3.  [2023-10-30-stat-smooth-mtcars/stat-smooth-mtcars.html](https://evamaerey.github.io/featurette/2023-10-30-stat-smooth-mtcars/stat-smooth-mtcars.html)
    **[source](https://github.com/evamaerey/featurette/blob/master/2023-10-30-stat-smooth-mtcars/stat-smooth-mtcars.Rmd)**
4.  [2023-10-30-ggformula-penguins/ggformula-penguins.html](https://evamaerey.github.io/featurette/2023-10-30-ggformula-penguins/ggformula-penguins.html)
    **[source](https://github.com/evamaerey/featurette/blob/master/2023-10-30-ggformula-penguins/ggformula-penguins.Rmd)**
5.  [2023-10-28-diamonds-barlabs/diamonds-barlabs.html](https://evamaerey.github.io/featurette/2023-10-28-diamonds-barlabs/diamonds-barlabs.html)
    **[source](https://github.com/evamaerey/featurette/blob/master/2023-10-28-diamonds-barlabs/diamonds-barlabs.Rmd)**
6.  [2023-10-26-tswift-keys/tswift-keys.html](https://evamaerey.github.io/featurette/2023-10-26-tswift-keys/tswift-keys.html)
    **[source](https://github.com/evamaerey/featurette/blob/master/2023-10-26-tswift-keys/tswift-keys.Rmd)**
7.  [2023-10-26-horror-articles/horror-articles.html](https://evamaerey.github.io/featurette/2023-10-26-horror-articles/horror-articles.html)
    **[source](https://github.com/evamaerey/featurette/blob/master/2023-10-26-horror-articles/horror-articles.Rmd)**
8.  [2023-09-13-ggcirclepack-global-human-day/global\_human\_day.html](https://evamaerey.github.io/featurette/2023-09-13-ggcirclepack-global-human-day/global_human_day.html)
    **[source](https://github.com/evamaerey/featurette/blob/master/2023-09-13-ggcirclepack-global-human-day/global_human_day.Rmd)**

-----

# code to write new featurette

``` r
new_experiment <- function(name){
  
  dir <- paste0(Sys.Date(),"-", name)
  
  dir.create(dir)
  readLines("template.Rmd") |>
    writeLines(con = paste0(dir,"/", name, ".Rmd"))
  
} 

new_experiment("ggplot-pie-charts")
```
