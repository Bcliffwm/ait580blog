---
layout: post
title:  "Descriptive Analysis"
date:   2022-04-16 10:22:52 -0400
categories: jekyll update
image: /assets/images/metadata.jpg
---
# Jupyter Notebook image
![]({{ page.image | relative_url }})

The dataset we selected was rather messy before we started our analysis. For example, for the map projections, using the 'GeoLocation' column was not possible unless we decoupled the object and converted the string data into a floating-point data type. Furthermore, the dataset contained many columns or fields of metadata regarding this dataset which was worthless for any analysis (starting with about 30 columns), so we dropped more than half of the original columns. The image above shows our end product of data cleansing using Python with the Pandas library.  

<img src="/ait580blog/assets/images/descriptiveStatistics.jpeg">

Above is a picture of the descriptive statistics of the dataset we used for our analysis.