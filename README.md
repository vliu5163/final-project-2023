# Proposal

The data:  
2021 Yellow Taxi Trip Data (30M rows) 


The modeling goal: 
I’d like to use different column values (borough, time of day, weekend vs not weekend, payment type) to predict whether or not the rider gives the driver a tip. Since tip amount is a continuous variable, instead I could categorize this variable as more or less than 15% tip (compared with the fare amount).  


The methods or models you intend to use (at least three):  
I intend to use linear regression, k-nearest neighbors, and random forest. For k-nearest neighbors, I will probably use a variety of distance metrics between different rides, including cosine similarity, Euclidean distance, and Minkowski distance. For linear regression, I am curious to know which column will have the greatest effect on tip amount. I will regress against single variables, combinations of variables, and all variables to see which column explains the most variance in the results. Finally, I would like to use random forest for classification to classify trips as more or less than 15% tip. 
Shapley value

Use random forest to predict the amount of tip, given calendar and borough information

Shapley is a permutation method, looks at all combinations of features (costly in terms of computation)
Fit linear model for SHAP by minimizing the loss function


# Sources

https://catalog.data.gov/dataset/nyc-taxi-zones
https://www.nyc.gov/assets/tlc/downloads/pdf/data_dictionary_trip_records_yellow.pdf
https://cran.r-project.org/web/packages/hydroTSM/index.html
https://www.nyc.gov/assets/tlc/downloads/pdf/data_dictionary_trip_records_yellow.pdf
