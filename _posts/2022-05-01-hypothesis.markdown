---
layout: post
title:  "Hypothesis Testing"
date:   2022-05-01 13:22:52 -0400
categories: jekyll update
image: /assets/images/SexDistHistogram.png
---

![]({{ page.image | relative_url }})

# Graph
Above is an overlaid histogram of the male and female prevention rates and a box-and-whisker plot. The purpose of creating the histogram is to see if our data were normally distributed across both sexes, which seems to be the case with a slight skew to the left. The hypothesis we decided to work from was to determine if there are any variances in the preventative measures succeession rates between males and females. Therefore, we selected the student t-test as our measurement tool.

Upon inspecting the graph, we notice that the men seemed to have an overall higher success rate in satisfying the CDC's preventative measures guidelines than the women. This observation ran contrary to Ben's expectations as he predicted the contrary.

# Methodology
We read our data into a Pandas dataframe in our local Python environment and then proceeded to separate the data into male and female dataframe objects. We then calculated the mean values of the preventative measures percentage columns for both the male and female dataframes. Then we aggregated the means by state. 

Before sending the data through scipy.stats's t-test_ind function, we needed to preprocess the data as the function could not handle numbers with such large precision values. To work around this issue, we passed the data through scipy.special's logsumexp function, which returns the log sum of the exponent of the input.  