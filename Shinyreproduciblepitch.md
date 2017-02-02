Course Project: Shiny Application and Reproducible Pitch
========================================================
author: Albert Blanchart  
date: 2017/02/02
autosize: true

The assignment
========================================================

* For this week we will develop a shiny app using the R basic data set **trees**. More information about this database can be found [here](http://stat.ethz.ch/R-manual/R-devel/library/datasets/html/trees.html).   
* As we will see in next slides, this dataset is pretty simple and we will use it to show linear regression model and how these models change depending on the values included in the regression model.  
* therefore, this presentattion contains basic exploratory analysis of the variables and data, and links for the shiny app and its code in GitHub.  

Hope you enjoy it!


A first look: Exploratory analysis
========================================================

* First look att the dataset

```
'data.frame':	31 obs. of  3 variables:
 $ Girth : num  8.3 8.6 8.8 10.5 10.7 10.8 11 11 11.1 11.2 ...
 $ Height: num  70 65 63 72 81 83 66 75 80 75 ...
 $ Volume: num  10.3 10.3 10.2 16.4 18.8 19.7 15.6 18.2 22.6 19.9 ...
```
* It is not the biggest or more complicated dataset but it will serve to our purposes in these exercise.

How does the data correlate
========================================================

![plot of chunk unnamed-chunk-1](Shinyreproduciblepitch-figure/unnamed-chunk-1-1.png)
Well we can see a clear correlation between the variables *Girth* and *Volume*, lets see what happens if we fit a linear model (something basic) and check the results

R Squared:

```
[1] 0.9353199
```

Our last step
========================================================
* Now that we have seen this correlation between *Girth* and *Volume*, lets going to use shiny to build a little app that shows how this R square value changes upon withdraw or addition of values. The app is found [here](https://changomazo.shinyapps.io/DoYourOwnLm/), and you can toggle data points just dragging the mouse. R square, slope and confidence intervals will change as you remove or add values.  
* The ui.R and server.R files can be found in my repository in [gitHubs](https://github.com/Changomazo/shiny-and-linear-regression), as well as the code for this presentation.  
I hope you found it amusing or even a bit useful :)
