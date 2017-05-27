---
title: "Developing Data Products"
author: "Ukykr"
date: '27 07, 2017'
output:
  ioslides_presentation:
    incremental: yes
    transition: default
    widescreen: yes
  slidy_presentation:
    incremental: yes
mode: selfcontained
hitheme: tomorrow
highlighter : highlight.js
subtitle: Interactive Model Evaluation
framework: io2012
widgets: []
 
--- 
## The Chatterjee\-Price Attitude Data





```r
kable(head(attitude))
```



| rating| complaints| privileges| learning| raises| critical| advance|
|------:|----------:|----------:|--------:|------:|--------:|-------:|
|     43|         51|         30|       39|     61|       92|      45|
|     63|         64|         51|       54|     63|       73|      47|
|     71|         70|         68|       69|     76|       86|      48|
|     61|         63|         45|       47|     54|       84|      35|
|     81|         78|         56|       66|     71|       83|      47|
|     43|         55|         49|       44|     54|       49|      34|



Source:


Chatterjee, S. and Price, B. (1977) Regression Analysis by Example. New York: Wiley. (Section 3.7, p.68ff of 2nd ed.(1991).)



--- 

## 

|            | coefficients.Estimate| coefficients.Std..Error| coefficients.Pr...t..| r.squared|
|:-----------|---------------------:|-----------------------:|---------------------:|---------:|
|(Intercept) |            14.3763194|               6.6199860|             0.0385083| 0.6813142|
|complaints  |             0.7546098|               0.0975329|             0.0000000| 0.6813142|

![plot of chunk unnamed-chunk-3](assets/fig/unnamed-chunk-3-1.png)

---



## Linear model, residuals plot.
        

|           | coefficients.Estimate| coefficients.Std..Error| coefficients.Pr...t..| r.squared|
|:----------|---------------------:|-----------------------:|---------------------:|---------:|
|complaints |             0.9624407|               0.0199801|                     0| 0.9876561|

![plot of chunk unnamed-chunk-4](assets/fig/unnamed-chunk-4-1.png)


---

## Machine learning models.

svmLinear, svmPoly, svmRadial - Support Vector Machines

glm - Generalized Linear Model

rf - Random Forest

cubist - Cubist
