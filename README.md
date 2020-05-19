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
To get a thorough understanding of the exact descriptions of the competiton, one must read the [competition guide](https://mk0mcompetitiont8ake.kinstacdn.com/wp-content/uploads/2020/02/M5-Competitors-Guide_Final-1.pdf), however, I will summarize the main points here. 
## Objective: 
The objective of the M5 forecasting competition is to advance the theory and practice of forecasting by
identifying the method(s) that provide the most accurate point forecasts for each of the 42,840 time
series of the competition, as well as the methods that elicit information to estimate the uncertainty
distribution of the realized values of these series as precisely as possible.

To that end, the participants of M5 are asked to provide 28 days ahead point forecasts (PFs) for all the
series of the competition, as well as the corresponding median and 50%, 67%, 95%, and 99% prediction
intervals (PIs).
