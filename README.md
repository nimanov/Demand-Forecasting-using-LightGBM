# **Store Item Demand Forecasting with LightGBM**
* Competition source : https://www.kaggle.com/c/demand-forecasting-kernels-only
* We are given 5 years of store-item sales data and asked to predict 3 months of sales for 50 different items at 10 different stores.
* It is actually a **"Time Series problem"**. The interesting part is that I will try to handle it with a **Machine Learning** approach by using the **LightGBM model**.
* The challenge is here that normally machine learning algorithms can not be used for **"Time Series"** problems(because they are not time series algorithms) unless we are able to generate features that represent **"Time Series"** patterns for the Machine learning models. Once we are able to do that we actually convert the time series problem into **regression problem** which can be solved by various ML algorithms.
* Thus, the key point is here that being able to generate appropriate features for the Machine Learning model in order to handle **"Time Series problem"** as a regression problem. Let's start !
![image](https://user-images.githubusercontent.com/48281477/141088431-3d1f408f-5bb5-4659-91fc-2098d1f09d3b.png)

# **Business Problem**
* There are 10 different stores and 50 distinct item in each. We want to forecast a number for each distinct 50 items that tell us how many each item will be sold on each day for 3 months period in every 10 stores. 
