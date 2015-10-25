BMI Calculator
========================================================
author: Theagarajan
date: Oct 25th 2015

Simply Shiny App for BMI Calculator
========================================================

BMI Calculator App has two inputs namely 
1. Height in cms.
2. Weight in kgs.

Input Widgets
========================================================
Inputs are collected by two Sliders.

    sliderInput("kgs",
                "Weight in kgs",
                min = 1,
                max = 250,
                value = 60),
    sliderInput("cms",
                "Height in cms",
                min = 1,
                max = 300,
                value = 180)
    
Input is provided in slider format,so that user can change the weight to see whether they can achieve normal weight by reducing or increasing weight. 

Output
========================================================

BMI(Body Mass Index) is an approximate measure for calculating the health of a person.

It is Weight/Height^2

Weight should in kgs and Height should be in meters.

Example
========================================================

BMI of a person with 78 kgs in weight and 170 cm in height is the following.


```r
Height = 170
Weight = 78
BMI = Weight/(Height/100)^2
BMI 
```

```
[1] 26.98962
```

The Application link 

https://theagarajan.shinyapps.io/BMIcalc


