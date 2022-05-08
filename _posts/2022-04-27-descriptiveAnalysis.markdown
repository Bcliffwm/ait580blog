---
layout: post
title:  "Descriptive Statistics"
date:   2022-04-27 10:22:52 -0400
categories: jekyll update
image: /assets/images/metadata.jpg
---
For this project, we explored survey data taken from Americans aged 65+ in 500 cities across the United States. The dataset we explored had information about adherence to CDC preventive measures and guidelines.   

The raw data that we explored was rather unorganized, and outliers, and had missing data. One of the biggest issues we faced was the inability to use one of the essential columns ‘GeoLocation’. We were not able to use this column until we decoupled the object and converted the string data into a floating-point data type.  
# Jupyter Notebook image
![]({{ page.image | relative_url }})


We also removed about 30 columns worth of data that were not relevant to our analysis. Below you will see the Metadata for the 13 columns that we were left with after completing data cleaning. The columns of the biggest interest are ‘DataValue’, ‘Short QuestionText’, while the columns ‘PouplationCount’, ‘CityName’, and ‘StateAbbr’ add value to our descriptive analysis as well.  


<img src="/ait580blog/assets/images/descriptiveStatistics.jpeg">

Looking into the specifics of the data, we can see the standard deviation, mean, and maximum values from the descriptive statistics above. 