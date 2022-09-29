This post is to exercise different modeling methods for detecting anomalies. 
There are many ways to set the tolerance band that identifies which does not belong into the band, and therefore is safe to call 'outliers'.
Here I am practicing 4 different modeling techniques that has different perspectives in terms of detecting anomalies. 4 techniques are as follows. 

1. Simple moving average (SMA)
    : treats every past datapoints equally.
2. Exponential smoothing (EMA)
    : assigns more importance into more recent datapoints
3. Seasonal-Trend Decomposition (STD)
    : decomposes data into seasonal, trend, and residual. By subtracting season and trend, what is remaining would be residuals, which are just noise.
4. Prophet module
    : assumes time series data can be subcategorized into trend, seasonality, and holiday effects.

For a successfull application of modelings, it is imperative to have explored the data and features being engineered accordingly. For instance, we need to make sure how many columns exist in what format, and if there is any missing values that need careful attention. After a proper exploratory data analysis, you can decide feature engineering that you think is necessary (e.g. imputation, lumping categories into smaller pieces, etc.) You can check out the EDA and FE as first steps into this analysis.

The dataset used is hourly energy consumption data in Megawatts, measured for more than 10 years. Dataset is retrieved from a Kaggle post, authored by Rob Mulla and you can access the dataset's source from the following url.

https://www.kaggle.com/datasets/robikscube/hourly-energy-consumption
