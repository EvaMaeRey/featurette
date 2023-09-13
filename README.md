
<!-- README.md is generated from README.Rmd. Please edit that file -->

# featurette git repo

<!-- badges: start -->

<!-- badges: end -->

The goal of featurette is to feature projects.

  - [](https://evamaerey.github.io/featurette/)

<!-- end list -->

``` r
new_experiment <- function(name){
  
  dir.create(paste0(Sys.Date(),"-", name))
  
} 

new_experiment("spam_email")
```
