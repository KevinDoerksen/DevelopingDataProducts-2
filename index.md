---
title       : Regression Model Shiny App
subtitle    : Now with widgets!
author      : In honor of Billy Mays
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : mathjax       # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides

---

## Regression modelling: the old way
### A model of frustration

Do you still evaluate in your regression models by hand?  <span style="color:red; font-weight:bold">Good luck</span> calculating those coefficients!

<div>$$ Y_i = \beta_1 X_{1i} + \beta_2 X_{2i} + \cdots + \beta_p X_{Pi} + \epsilon_i = \sum_{k = 1}^{p} X_{ik}\beta_j + \epsilon_i$$</div>



<hr>

Perhaps you use the R command line to evaluate your regression models?

* Half the time, you <span style="color:red; font-weight:bold">can't</span> remember the names of the variables! 
* You have to try <span style="color:red; font-weight:bold">dozens</span> of different regression models!
* When you finally build a model, you face a <span style="color:red; font-weight:bold">wall of information</span> to interpret:




```r
summary(lm(rating ~ complaints, data = attitude))
```



--- 

## The old way: such a complicated output


```
## 
## Call:
## lm(formula = rating ~ complaints, data = attitude)
## 
## Residuals:
##      Min       1Q   Median       3Q      Max 
## -12.8799  -5.9905   0.1783   6.2978   9.6294 
## 
## Coefficients:
##             Estimate Std. Error t value Pr(>|t|)    
## (Intercept) 14.37632    6.61999   2.172   0.0385 *  
## complaints   0.75461    0.09753   7.737 1.99e-08 ***
## ---
## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
## 
## Residual standard error: 6.993 on 28 degrees of freedom
## Multiple R-squared:  0.6813,	Adjusted R-squared:  0.6699 
## F-statistic: 59.86 on 1 and 28 DF,  p-value: 1.988e-08
```


--- 

## The New Regression Model Shiny App
### We have an app for that

* <span style="color:black; font-weight:bold">Easy to use</span>

  * Just select your predictor variables and press <span style="color:blue; font-weight:bold">Run Simulation</span>
  
* <span style="color:black; font-weight:bold">Efficient output:</span> you only see what you need

  * The formula,
  * A measure of the variance explained by your model,
  * Residuals plots

* <span style="color:black; font-weight:bold">Fast</span>

  * Don't like the linear model you chose?  Not to worry, select new predictor variables and re-run the simulation
  

  

---

## But wait there's more!

This app is a good proof-of-concept app <span style="color:blue; font-weight:bold">ready</span> for expanded development

* We show that this design works well with the attitude dataset 
* With enough interest, we can expand the app to work with any dataset

But that's not all folks, because we're <span style="color:blue; font-weight:bold">doubling</span> the order!

* That's right!  You get two copies of the Shiny app with each order.
    * <span style="color:lightgrey">Second app not included with some orders</span>

### Did someone say "New car"?

Be among the first 100 app testers and you will be entered in to a draw to <span style="color:blue; font-weight:bold">win a brand new car</span> <span style="color:lightgrey">door hinge!</span>
