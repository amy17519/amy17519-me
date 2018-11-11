---
title: A Relocation Guidebook for Data Scientists and Tech Professionals
author: Amy Tzu-Yu Chen
date: '2016-10-04'
slug: a-relocation-guidebook-for-data-scientists-and-tech-professionals
categories: ["R", "Project"]
tags: ["R", "Project"]
---

![](https://raw.githubusercontent.com/amy17519/RelocationPlan-RViz/master/blog_img/00cover.jpg)

This was my first data visualization project at NYC Data Science Academy and also my first published work. It was featured on Open Data Science Conference website on Sep.19, 2016. 

- [Github](https://github.com/amy17519/RelocationPlan-RViz)
- [Slides](https://github.com/amy17519/RelocationPlan-RViz/blob/master/RelocationPlanRmdCode.pdf)

# Introduction

If you are a data scientist and you are offered a job in another city - or if your current employer asks you to relocate - would you make the move? Many may happily accept the offer and begin a new chapter of their life. Others may struggle to write down a comprehensive cost benefit analysis to avoid making a mistake. It is possible to use data visualization to quickly compare and contrast living standards and make an informed choice in a few simple steps.

# Job Market for Data Scientists

![](https://raw.githubusercontent.com/amy17519/RelocationPlan-RViz/master/blog_img/01jobs.png)

The first thing for jobseekers to consider is whether their potential new city offers abundant career opportunities. This is also important for people who are transferred by their current employer because they will want to ensure they are still in demand in their new city. This analysis provides an overview of the job market for data scientists by searching the keyword "data scientist" on major job hunting websites including LinkedIn, Indeed, and Glassdoor. As of July 13, 2016, the top six cities with the best career outlook for data scientists are San Francisco, New York, Washington DC, San Jose, Boston, and Seattle. Congratulations if any of these cities is on your list for consideration.

# Living Expense

![](https://raw.githubusercontent.com/amy17519/RelocationPlan-RViz/master/blog_img/02expense.png)

Once you are certain about career opportunities in the new destination, the next step is to consider another practical factor: cost of living. We will consider the top six cities with the most data scientist job opportunities in the following graphics. Numeo, an online user contributed database of living expenses, publishes rankings of living expense levels for cities and countries worldwide, which can be used to estimate and compare cost of living. Numeo breaks down living expenses into several categories of indices including cost of living (e.g., restaurants, groceries) and rent. Note that cost of living index only includes the prices of goods and services and excludes rent.

Based on published Numeo data it is easy to compare and contrast cost of living and rent levels in the selected six cities. New York City earns 100 points in both cost of living and rent indices. Interestingly, NYC is not the most expensive city among all candidates in terms of rent. San Francisco's rent index is 125, which is 25% higher than that of NYC. A San Franciscan may spend slightly less for goods and services than a New Yorker, but he/she will likely need to pay much higher rent. In fact, one can observe the same pattern of discrepancies between cost of living and rent in other cities. San Jose ranked No.3 in rent, but the cost of living is lower than other five candidate cities. Seattle's rent index is only half of that of San Francisco yet its cost of living index exceeds those of San Jose and Boston. To summarize, it is important to consider both cost of living and rent levels as meaningful factors as they are not necessarily consistent.

Data Source: [Numeo](http://www.numbeo.com/cost-of-living/comparison.jsp) is the World’s largest database of user contributed data about cities and countries worldwide. It provides current and timely information on world living expenses. Standard of living is divided into various categories of index including cost of living, rent, restaurant, and groceries etc.

# Rent Comparison

No matter where you choose to live, housing expense eats up a large portion of your income. This section discusses both the current rental prices as well as the 2015-2016 rental market trends in four of the six cities. After reading this analysis, you will not only know whether relocation is a practical decision, but also have a general idea about what type of room to look for in the new city.

The chosen datasets for this section are Zillow's Rent Index. Zillow is an online real estate database company that publishes up-to-date rent data for public use. The datasets comprise median rent for each room type in geographic regions across the United States. Zillow uses room type as the main grouping attribute to ensure the data are unaffected by mix of homes. Also, the company tracks rents from a consistent pool of houses, which makes the time-based comparisons of rent more valid. I have decided to include only one bedroom, two bedroom, and three bedroom apartments in this discussion for two reasons. First, Zillow has complete datasets with no missing values for these types of apartments. Second, the selected room types are probably the most common choice for a city's newcomer.

## Total Rent Price

![](https://raw.githubusercontent.com/amy17519/RelocationPlan-RViz/master/blog_img/03medianrent.png)

The graph below shows the rankings of median rental prices for all room types.  The cities rank from most to least expensive are:  San Francisco, San Jose, New York City, and Seattle. This is mostly consistent with the ranking of Numeo's rent index except that San Jose has higher median rents than NYC for all room types. Seattle is the only place where you can easily find rent an apartment of any room type for less than $2,000 a month and you may not easily find a good apartment for less than this in the other three cities.

## Rent Price per Square Foot

![](https://raw.githubusercontent.com/amy17519/RelocationPlan-RViz/master/blog_img/04medianrent2.png)

Information about rent price per square foot is more useful for one to estimate the real cost per person and decide the best value by room type in the new city. The ranking of median price per square foot by city is consistent for one and two bedrooms but varies for three bedrooms. One can more easily observe trends in the rental market in the below chart since it is on a per unit basis. For instance, the trend that rental prices in NYC and San Jose are merging becomes apparent in this graph.

### San Francisco

You should think twice about relocating to San Francisco if you care about sharing an apartment with others since one bedroom prices are so high. The rent level in San Francisco is the highest and it continues to rise for all room types. Although it seems that the rent for one bedroom and two bedroom apartments had stabilized in the first five months of 2016, the price you have to pay to get a smaller apartment is going to be much higher than other three cities. The least expensive choice is to share a three bedroom apartment with others. However, the price for three bedroom apartments is increasing at a relatively fast rate, which is a trend we can observe in all four cities.

### New York City

NYC can finally shed the label of the most expensive city in the United States; at least, for a moment. The median rents for all room types are all less than San Francisco and San Jose. From the beginning of 2016, one can observe increasing rent prices for all room types. The rent level in NYC is on the whole increasing and is converging to the rent level of San Jose. The most economic choice if you want to relocate to NYC is most likely two bedroom apartments since three bedroom apartments have the highest price per square foot among all cities.

### San Jose

The rents for one bedroom and two bedroom apartments in San Jose briefly surpassed San Francisco last summer, but San Francisco returned to No. 1 towards the end of 2015. The rent levels for one bedroom and two bedroom apartments stabilized in 2016, but the price for three bedroom apartments is increasing. If San Jose is your next destination, you can consider renting a two bedroom or even one bedroom apartment since the rent price has been decreasing since the end of 2015.

### Seattle

Seattle can easily win the contest of having the best value apartments. The prices for all types of apartments are notably cheaper than Bay Area and NYC. Although the rental prices had been constantly increasing in the past year and a half, it would most likely take a while before it reach the level of the other candidate cities.

## Best Time to Move?

![](https://raw.githubusercontent.com/amy17519/RelocationPlan-RViz/master/blog_img/05move.png)

In addition to all living expense comparisons, you may wonder what would be the best time of a year to move. In this graph, you are seeing the number of maximum and minimum rent occurrences for each room type in the 12 cities with most data scientist job vacancies from 2011 to 2016. For example, if the lowest median rent for one bedroom apartments in Los Angeles in 2013 occurred in January, then January gets one point in the minimum occurrence plot. As one can see from the graph, January may be the best time of a year to relocate. In contrast, you may risk signing a relatively more expensive lease in May.

Data Source: [Zillow](http://www.zillow.com/research/data/) is an online real estate database company who provides free up-to-date real estate data for public use by consumers, media, analysts, and academics.

# Conclusion

## Things to Consider

- SF, NYC, DC, San Jose, Boston, and Seattle have most data scientist jobs, so you may consider relocation for better career outlook
- Cost of living standards may not be consistent with cost of renting an apartment, so be sure to consider both factors when you choose a destination
- Although living in a 3-bedroom apartment has the lowest rent per sqft, the overall price level is steadily increasing in NYC, San Francisco, San Jose, and Seattle
- In terms of rent, NYC is not as expensive as San Jose and SF. However, rents in NYC and San Jose are converging

## Final Tips

- NYC and San Jose: 2-bedroom apartment has the best value
- SF: 3-bedroom apartment has the best value
- Seattle: your best destination to save money! Although the rent has been increasing, it is still ~66% less expensive than the Bay Area and NYC
Relocate in January to get the best deal and avoid signing your lease just before summer
