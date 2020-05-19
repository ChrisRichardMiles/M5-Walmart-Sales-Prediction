# M5-Walmart Sales Prediction
This is a case study of my efforts in the M5 competitions, both hosted on kaggle. The [accuracy competiton](https://www.kaggle.com/c/m5-forecasting-accuracy) asks for the point forecasts of product sales, aggregaged accross 12 levels, and the [uncertainty competition] asks for prediction confidence intervals of product sales, aggregated across the same 12 levels. I will research and implement machine learning methods, as well as statistical methods, in search of the highest performing model, or ensemble of models, with respect to the M5 competition dataset and scoring metric. Although we could define various business objectives and performance metrics, the focus of this case study will be to find a methodology that specifically minimizes the competition metrics, as outlined in the competition guidlines. 


# Objective
1. Develop a process that will produce point estimates, as well as confidence intervals for day to day sales of Walmart products, across 12 levels of aggregation.

# Metric: Weighted Root Mean Squared Scaled Error (WRMSSE)



# Business problem
Retailers 
Retail businesses have two problems that arrise from an inadequate understanding of demand. 
1. Oversupply: When a store overstocks an item, they incur costs from storing the surplus of product, as well as throwing away perishable food items. 
2. Undersupply: When a store runs out of a product, they miss out on the sales that would have occured if the product was in stock. 


# What is the M5 competition? 
To get a thorough understanding of the exact descriptions of the competiton, one must read the [competition guide](https://mk0mcompetitiont8ake.kinstacdn.com/wp-content/uploads/2020/02/M5-Competitors-Guide_Final-1.pdf), however, I will highlight the main points here. 
## Objective: 
The objective of the M5 forecasting competition is to advance the theory and practice of forecasting by
identifying the method(s) that provide the most accurate point forecasts for each of the 42,840 time
series of the competition, as well as the methods that elicit information to estimate the uncertainty
distribution of the realized values of these series as precisely as possible.

To that end, the participants of M5 are asked to provide 28 days ahead point forecasts (PFs) for all the
series of the competition, as well as the corresponding median and 50%, 67%, 95%, and 99% prediction
intervals (PIs).

## The dataset 
The dataset
The M5 dataset, generously made available by Walmart, involves the unit sales of various products sold
in the USA, organized in the form of grouped time series. More specifically, the dataset involves the unit
sales of 3,075 products, classified in 3 product categories (Hobbies, Foods, and Household) and 7 product
departments, in which the above-mentioned categories are disaggregated. The products are sold across
10 stores, located in 3 States (CA, TX, and WI). In this respect, the bottom-level of the hierarchy, i.e.,
product-store unit sales, can be mapped either across product categories or geographical regions, as
follows:

Table 1: Number of M5 series per aggregation level.
Level
id
Aggregation Level Number
of series
1 Unit sales of all products, aggregated for all stores/states 1
2 Unit sales of all products, aggregated for each State 3
3 Unit sales of all products, aggregated for each store 10
4 Unit sales of all products, aggregated for each category 3
5 Unit sales of all products, aggregated for each department 7
6 Unit sales of all products, aggregated for each State and category 9
7 Unit sales of all products, aggregated for each State and department 21
8 Unit sales of all products, aggregated for each store and category 30
9 Unit sales of all products, aggregated for each store and department 70
10 Unit sales of product x, aggregated for all stores/states 3,049
11 Unit sales of product x, aggregated for each State 9,147
12 Unit sales of product x, aggregated for each store 30,490
Total 42,840
