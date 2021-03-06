# mixopt

Empirical comparisons of algorithms for solving the "mixture
distribution" optimization problem. See
[here](https://pcarbo.github.io/mixopt) for the
code and results.

## Setup

To reproduce the results of the analyses, install these packages in R:

```R
install.packages(c("ggplot2","cowplot"))
```

## Running the code in the R Markdown documents

If you prefer to run the R Markdown documents as scripts, one simple
approach is to use the `purl` function from the `knitr` package, e.g.,

```R
source(purl("qpdemo.Rmd"))
```

## How to build the webpages

Run the following commands in R from the [analysis](analysis)
directory:

```R
library(rmarkdown)
render("index.Rmd",output_dir = "../docs")
render("qpdemo.Rmd",output_dir = "../docs")
render("qpdemo2.Rmd",output_dir = "../docs")
render("normmix.Rmd",output_dir = "../docs")
```
