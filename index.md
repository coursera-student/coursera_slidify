---
title       : Coursera Slidify Project
subtitle    : Reproducible Pitch Presentation
author      : Coursera-student
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## The Project

This Slidify presentation is one of the assignments that fufills the requirements for the "Developping Data Products" class offered on [Coursera](https://www.coursera.org/course/devdataprod).

<img class ='center'src='./image/DevelopingDataProducts.jpg' height=200px/>

The goal of this Slidify presentation is to give a brief overview of a my Shiny Web Application. The app uses the "ozone" dataset from the Element of Statistical Learning package and displays a scatterplot of the relationship between the X and Y variables that the user specifies from a drop down menu. A loess curve is added to the scatterplot. 


The code for this Slidify presentation is available on [Github]()


---

## The Data


```r
library(ElemStatLearn) # install.packages("ElemStatLearn")
data(ozone)
summary(ozone)
```

```
##      ozone         radiation    temperature        wind      
##  Min.   :  1.0   Min.   :  7   Min.   :57.0   Min.   : 2.30  
##  1st Qu.: 18.0   1st Qu.:114   1st Qu.:71.0   1st Qu.: 7.40  
##  Median : 31.0   Median :207   Median :79.0   Median : 9.70  
##  Mean   : 42.1   Mean   :185   Mean   :77.8   Mean   : 9.94  
##  3rd Qu.: 62.0   3rd Qu.:256   3rd Qu.:84.5   3rd Qu.:11.50  
##  Max.   :168.0   Max.   :334   Max.   :97.0   Max.   :20.70
```

---

## Access to the Shiny Application

The Shiny application can be access in three ways:

1. Via the [shinyapps.io]() website.
2. By going to the next slide.
3. By accessing the raw source from [Github](): download the `server.R` and `ui.R` files. Open R and set the working directory to be inside the folder that contains both files. Then run the following commands:

```
library(shiny)
runApp()
``` 


---


<iframe src=http://coursera-student.shinyapps.io/coursera-shiny></iframe>
