# mixopt

Empirical comparisons of algorithms for solving the "mixture
distribution" optimization problem. See
[here](https://pcarbo.github.io/mixopt) for the
code and results.

## How to build the webpages

Run the following commands in R from the [analysis](analysis)
directory:

```
library(rmarkdown)
render("index.Rmd",output_dir = "../docs")
render("qpdemo.Rmd",output_dir = "../docs")
render("normmix.Rmd",output_dir = "../docs")
```
