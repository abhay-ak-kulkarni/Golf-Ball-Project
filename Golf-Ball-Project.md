Golf-Ball-Project
================
Abhay Kulkarni
26/06/2019

  - [Introduction](#introduction)
      - [Libraries/Packages](#librariespackages)
      - [Set Working Directory](#set-working-directory)
      - [Import Dataset](#import-dataset)
      - [Import Dataset"](#import-dataset-1)
  - [Assumptions](#assumptions)

# Introduction

" Par Inc., is a major manufacturer of golf equipment. Management
believes that Par’s market share could be increased with the
introduction of a cutresistant, longer-lasting golf ball. Therefore,
the research group at Par has been investigating a new golf ball coating
designed to resist cuts and provide a more durable ball. The tests with
the coating have been promising. One of the researchers voiced concern
about the effect of the new coating on driving distances. Par would like
the new cut-resistant ball to offer driving distances comparable to
those of the current-model golf ball. To compare the driving distances
for the two balls, 40 balls of both the new and current models were
subjected to distance tests. The testing was performed with a mechanical
hitting machine so that any difference between the mean distances for
the two models could be attributed to a difference in the design. The
results of the tests, with distances measured to the nearest yard, are
contained in the data set “Golf”. Prepare a Managerial Report

1.  Formulate and present the rationale for a hypothesis test that par
    could use to compare the driving distances of the current and new
    golf balls

2.  Analyze the data to provide the hypothesis testing conclusion. What
    is the p-value for your test? What is your recommendation for Par
    Inc.?

3.  Provide descriptive statistical summaries of the data for each model

4.  What is the 95% confidence interval for the population mean of each
    model, and what is the 95% confidence interval for the difference
    between the means of the two population?

5.  Do you see a need for larger sample sizes and more testing with the
    golf balls?
Discuss."

## Libraries/Packages

``` r
library("readxl")
```

## Set Working Directory

``` r
setwd("Z:/Projects for Github/Hypothesis Testing/GOLF BALL/Golf-Ball-Project")
getwd()
```

    ## [1] "Z:/Projects for Github/Hypothesis Testing/GOLF BALL/Golf-Ball-Project"

## Import Dataset

``` r
mydata <- read_excel("Golf .xls")
```

## Import Dataset"

``` r
mydata
```

    ## # A tibble: 40 x 2
    ##    Current   New
    ##      <dbl> <dbl>
    ##  1     264   277
    ##  2     261   269
    ##  3     267   263
    ##  4     272   266
    ##  5     258   262
    ##  6     283   251
    ##  7     258   262
    ##  8     266   289
    ##  9     259   286
    ## 10     270   264
    ## # ... with 30 more rows

# Assumptions

" The sample size of the data set is 40 from each model of golf ball.
Central Limit Theorem states that irrespective of the shape of the
original population, the sampling distribution of the mean will approach
a normal distribution as the size of the sample increases and becomes
large (\>30). We also assume that the sample estimate will be reflective
of the reality."
