---
title       : Exploratory Study of 'mtcars' using Linear Regressions
subtitle    : A Shiny App
author      : tankokhua
job         : Engineer
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Introduction

1. Shiny App
2. 'mtcars' dataset
3. Linear Regression
4. User Interface
5. Running the App
6. Results
7. Conclusion

--- .class #id 
## Shiny App
1. A 'Shiny' (http://shiny.rstudio.com) app is used to build the user interface to study 'mtcars' dataset.
2. The objective is to study the impact of certain aspects of the car designs on fuel consumption.
3. This app helps the user to perform quick first pass analysis to determine the possible
   regressors.
4. A 'Shiny' app can be built with minimal effort.

--- .class #id 
## 'mtcars' dataset
1. The 'mtcars' dataset has 11 variables.

```
##  [1] "mpg"  "cyl"  "disp" "hp"   "drat" "wt"   "qsec" "vs"   "am"   "gear"
## [11] "carb"
```
A data frame with 32 observations on 11 variables.

 Abbrev.  |  Description
 ---------|--------------------------------------------
 mpg      |  Miles/(US) gallon                        
 cyl      |  Number of cylinders                      
 disp     |  Displacement (cu.in.)                    
 hp       |  Gross horsepower                        
 drat     |  Rear axle ratio                        
 wt       |  Weight (lb/1000)                      
 qsec     |  1/4 mile time                        
 vs       |  V/S                                 
 am       |  Transmission (0 = automatic, 1 = manual)
 gear     |  Number of forward gears            
 carb     |  Number of carburetors             

--- .class #id 
## Linear Regression
* In this app, linear regression is used to predict a response variable from one or more
  predictor variables or regressors.
* The objective is to identify the potential regressors which can be used to provide an equation
  for predicting the response variable, in this case, 'mpg'.

--- .class #id 
## User Interface
![alt Input ](./interface.png)

--- .class #id 
## Running the App
* Open the "server.R" or "ui.R" file from R Studio
* Click on "Run App" button to launch the application.
* Select one or more regressors/predictors.
* The formula for linear regression will be displayed.
* Click on "Go!" Button to generate the regression coefficients and residual plots.

--- .class #id 
## Results
1. The output panel consists of
  + Coefficients of linear regression
  + Residual Plots
2. The coefficients show which regressors may be significant in explaining the model.
3. The residual plots give an indication of the 'correctness' of the model.

--- .class #id 
## Conclusion
* This is a simple illustration of developing data products using 
  + Shiny App to create the user interface
  + Slidify (http://slidify.github.io) to pitch about the data product.
* Developers can dedicate more time on the research topics, and make use of these
  efficient tools to produce impressive presentations/products.

### Note: This presentation deck is built using "Slidify".


