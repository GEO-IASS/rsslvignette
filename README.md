Vignette introducing RSSL
===============
Authors: Jesse H. Krijthe

This repository contains the code to generate/reproduce the paper "RSSL: Semi-supervised Learning in R".

# Abstract

In this paper, we introduce a package for semi-supervised learning research in the R programming language called RSSL. We cover the purpose of the package, the methods it includes and comment on their use and implementation. We then show, using several code examples, how the package can be used to replicate well-known results from the semi-supervised learning literature.

# How to use this code
To run the example code in the paper or to reproduce the paper, we require a recent R version and the installation of some dependencies. The dependencies can be installed from within R using:
```{r}
install.packages(c("RSSL","ggplot2","plot3D","ggthemes","scales","dplyr")
```

The example code can be found in the rsslvignette.Rnw file. The simplest way to run the examples or generate the whole document is to open the file in Rstudio. Alternatively, one can also run all the examples and generate the document by running the following commands from the terminal (in Linux or macOS):
```{bash}
Rscript -e 'knitr::knit("optimisticssl.Rnw")'
pdflatex optimisticssl
bibtex optimisticssl
pdflatex optimisticssl
pdflatex optimisticssl
```
