# phygen
Phylogenetic methods S2020


---
title: "phylo_exc_1"
output: html_document
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE)
```

## R Markdown

This is an R Markdown document. Markdown is a simple formatting syntax for authoring HTML, PDF, and MS Word documents. For more details on using R Markdown see <http://rmarkdown.rstudio.com>.

When you click the **Knit** button a document will be generated that includes both content as well as the output of any embedded R code chunks within the document. You can embed an R code chunk like this:

```{r cars}
summary(cars)
```

## Including Plots

You can also embed plots, for example:

```{r pressure, echo=FALSE}
plot(pressure)
```

Note that the `echo = FALSE` parameter was added to the code chunk to prevent printing of the R code that generated the plot.

################################
---
title: "Getting Started"
author: "Eager PhyloMeth student"
date: "`r format(Sys.time(), '%d %B, %Y')`"
output: html_document
---

R calls in R markdown go within sections delimited by three backticks (`, the character just to the left of the 1 on US English keyboards; YMMV on other keyboards). For R code to execute, you must include {r} after the first three.

```{r}
2+3
library(ape)
plot(rcoal(5))
```

Look at the Markdown Cheatsheet [PDF](https://www.rstudio.com/wp-content/uploads/2015/02/rmarkdown-cheatsheet.pdf) for more info.

*To do*

Take the following lines and do what they say.

**MAKE THIS LINE BOLD**

MAKE THE WORD *ITALIC* ITALICIZED

MAKE THE FOLLOWING R CODE CREATE A PLOT IN THIS DOCUMENT

```{r}
plot(density(rnorm(1000)))
```

### R exercise

Edit this document so that this code all runs properly. You can create the final document by doing `rmarkdown::render("gettingstarted_exercise.Rmd")` in R or hitting the knit button in Rstudio.


```{r}
# Experience with coding.

GetHowManyTrees <- function(ntax) {
    #ape can compute this for us. help(package="ape") for help on ape.
    result <- howmanytrees(ntax)
    return(result)
}
```



```{r}
GetHowManyTrees(20)
