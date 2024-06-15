# Retial_Sales_Prediction_Project
Sales forecasting refers to the process of estimating demand for or sales of a particular product over a specific period.

![image](https://github.com/infojain/Retial_Sales_Prediction_Project/assets/143530568/d8586633-ce9c-4e9d-9daa-6f1a4d8721a1)

# Content
1. Problem Statement 
2. Data Summary 
3. Data Preprocessing 
4. Exploratory Data Analysis 
5. Feature Engineering 
6. Model Implementation 
7. Conclusion

# Problem Description
1.** Number of Stores: **XYZ operates over 3,000 stores in 7 different countries.
2. **Prediction Task:** Store managers need to predict daily sales for up to six weeks in advance.
3.** Influencing Factors:** Sales are affected by promotions, competition, school and state holidays, seasonality, and locality.
4. **Variation in Accuracy:** Due to the unique circumstances of each store, prediction accuracy varies among managers.
5. **Data Provided:** Historical sales data for 1,115 stores is available.
6. **Forecasting Goal:** The task is to forecast the "Sales" column for the provided test set.
7. **Temporary Closures:** Some stores were temporarily closed for refurbishment 

# Data Description
1. Data 1- 
  - Columns- 9,  
  - Rows- 1017210

2. Data 2 – 
  - Columns – 10, 
  - Rows – 1115
# Data fields :- Data 1
- Id - an Id that represents a (Store, Date) duple within the set
- Store - a unique Id for each store
- Sales - the turnover for any given day (Dependent Variable)
- Customers - the number of customers on a given day
- Open - an indicator for whether the store was open: 0 = closed, 1 = open
- State Holiday - indicates a state holiday. Normally all stores, with few exceptions, are closed on state holidays. Note that all - schools are closed on public holidays and weekends. a = public holiday, b = Easter holiday, c = Christmas, 0 = None
- School Holiday - indicates if the (Store) was affected by the closure of public schools

# Data fields :- Data 2
- Store Type - differentiates between 4 different store models: a, b, c, d
- Assortment - describes an assortment level: a = basic, b = extra, c = extended. An assortment strategy in retailing involves the number and type of products that stores display for purchase by consumers.
- Competition Distance – the distance in meters to the nearest competitor store
Competition Open Since[Month/Year] - gives the approximate year and month of the time the nearest competitor was opened
- Promo - indicates whether a store is running a promo on that day
- Promo2 - Promo2 is a continuing and consecutive promotion for some stores: 0 = store is not participating, 1 = store is participating -- Promo2  Since[Year/Week] - describes the year and calendar week when the store started participating in Promo2
- Promo Interval - describes the consecutive intervals Promo2 is started, naming the months the promotion is started anew. E.g. "Feb, May, Aug, Nov" means each round starts in February, May, August, and November of any given year for that store.

# Objective
  To create a robust sales forecasting model using historical sales data, considering the various factors that influence sales.
# Feature Engineering
1.Extracting week, month, year from Date and adding them in dataset. 
2. Merging both dataset. 
3. One hot encoding for Storetype, Assortment. 
4. Splitting dataset into Training and Test set and applying MinMaxScaler for scaling dataset.

# Models Implemented 
1. Linear Regression (Baseline Model) 
2. Lasso Regression 
3. Decision Tree Regress 
4. Random Forest Regressor

# Model Evaluation 
![image](https://github.com/infojain/Retial_Sales_Prediction_Project/assets/143530568/66525b42-5077-4b8c-af0a-33cc1fbe47c1)
