---
layout: post
title:  "Data Curation"
date:   2022-04-30 09:22:52 -0400
categories: jekyll update
image: /assets/images/Whiteboard.png
---

## Data Curators
The CDC is a U.S. Government entity charged with the responsibility of protecting the citizens of the United States from any illness, virus or disease that poses a threat to our country's well-being. The members of the CDC often conduct scientific experiments, collect data, host and conduct public-health seminars all in order to make efforts to disseminate information to the public.

## PLACES Motivation
The purpose of PLACES was to provide information on a zip code-by-zip code basis, identify key health problems, develop localized plans moving forward, and differentiate the health threats affecting citizens living in various areas such as urban, rural or suburban areas.

## Potential Bias
We identified a few weaknesses of the dataset where bias may affect ongoing or future analysis predicated on this dataset and datasets curated in a similar fashion. 

First, this dataset is a survey over the phone to various participants across the country whose responses must all be 'yes' to every preventative measure the CDC outlines in its guidelines in order to be counted in the survey. For this reason alone, this may explain why the response rate or signal is relatively low (approximately 35% across all states and regions). 

Second, some states such as California and Texas have way more participating locations than other states such as Alaska or North Dakota. While this trend should makes logical sense if the motivation is to study as many people as possible, the consequence or potential source of bias manifests in the lack of representation of less populated areas of the country. Furthermore, there wasn't a single rural or suburban location or locus of participants in this dataset, which means that no information was gathered for people living in these types of environments.

## Data Quality
The dataset we selected was nowhere near ready for analysis. The main focus of this dataset is targeting population groups in different geographic areas, but the data for the geolocations were nested inside of a data object in the form of strings. This made geospatial analysis impossible to conduct as is because the software we used (GeoPandas and Shapely) required the data to be in a different format.

Additionally, most of the metadata on the CDC's websites hardly explained any of the actual fields of the dataset we worked with. The methodology seemed to explain more about the data rather than the documentation which was rather unsettling if the CDC is determined to inform the public about health matters. Navigating through the dataset was not difficult, rather it took mostly common sense to parse through the meaningless pieces of information to select the meaningful parts. Additionally, having Bethlehem's expertise in healthcare made understanding the data easier, which made the analysis more straightforward.

The dataset has no security or privacy protections as this came from the CDC, whose objectives include disseminating health-related information to the American public.

In conclusion, while this dataset being highly available is useful as well as the CDC offering free visualization tools to interact with the data on its website, it has many flaws when it comes to conducting analysis outside of their website. Having the dataset not being prepared in a suitable format for analysis and subsequent extracting, loading and transforming does come with the territory of Data Analytics, it does make one wonder how the CDC manages to achieve their goals of disseminating data with this dataset having so few variables and documentation with little to no explanatory power.