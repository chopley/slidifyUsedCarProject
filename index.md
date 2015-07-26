---
title       : Predicting Used Car Prices
subtitle    : An App learns the price of used cars using online data
author      : Charles Copley
job         : Researcher
framework   : io2012       # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## What does it do?

1. Scrapes unstructured data from a used car website (www.autotrader.co.za) using parallel R scrapers. 
2. Extracts car make, model, mileage, engine size, year, selling price.
3. Uses Gradient Boosted Regression to 'learn' from the data and make predictions of car prices given unseen information
4. Deploys an R-Shiny App for interface to the user.
5. Plots the price of car, as well as information about estimated depreciation.

--- .class #id 

## Give it some inputs and predict a Price?


```r
model<-'audi'
make<-'a4'
year<-2014
engineSize<-1.8
mileage<-100000
```




The price is then given by the priceEstimate variable

```r
priceEstimate[2]
```

```
## $y
## [1] 240655
```

--- .class #id

## Can Also Predict Depreciation





![plot of chunk simpleplot](assets/fig/simpleplot-1.png) 

---

## Summary

  * Predictive App for Price estimation
  * Takes Model, Make, Year, Mileage and Engine Size as Inputs
  * Can be used for depreciation
