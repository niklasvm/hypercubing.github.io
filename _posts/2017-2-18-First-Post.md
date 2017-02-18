---
title: "Untitled"
author: "Niklas von Maltzahn"
date: "18 February 2017"
output: html_document
---



## R Markdown

This is an R Markdown document. Markdown is a simple formatting syntax for authoring HTML, PDF, and MS Word documents. For more details on using R Markdown see <http://rmarkdown.rstudio.com>.

When you click the **Knit** button a document will be generated that includes both content as well as the output of any embedded R code chunks within the document. You can embed an R code chunk like this:


{% highlight r %}
summary(cars)
{% endhighlight %}



{% highlight text %}
##      speed           dist       
##  Min.   : 4.0   Min.   :  2.00  
##  1st Qu.:12.0   1st Qu.: 26.00  
##  Median :15.0   Median : 36.00  
##  Mean   :15.4   Mean   : 42.98  
##  3rd Qu.:19.0   3rd Qu.: 56.00  
##  Max.   :25.0   Max.   :120.00
{% endhighlight %}

## Including Plots

You can also embed plots, for example:

![center](/to_publish/figs/2017-2-18-First-Post/pressure-1.png)

Note that the `echo = FALSE` parameter was added to the code chunk to prevent printing of the R code that generated the plot.


{% highlight r %}
library(tidyverse)
ggplot(diamonds,aes(x=cut,y=price))+
  geom_jitter(aes(col=clarity))+
  geom_boxplot(alpha=0.5)
{% endhighlight %}

![center](/to_publish/figs/2017-2-18-First-Post/unnamed-chunk-4-1.png)

