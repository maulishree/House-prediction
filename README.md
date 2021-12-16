# House-prediction


**Project description and summary**:

Purchasing a house is a big decision in a person’s life and requires an immense amount of thought and research. Traditional house price prediction lacks an accepted standard and a certification process, making house buying even more stressful. There lies a need to fill this gap with a more methodical approach. We have used the UCI Machine Learning Database as our dataset for predicting house prices. The UCI Machine Learning Database is used by students, educators, and researchers all over the world. It is a great source for statisticians, allowing them to perform data analysis on a variety of real-world examples. Of all these examples, we will be looking at one that involves real estate valuation from the Sindian District of New Taipei City, Taiwan (UCI, 2018)

**Goal:**

We have been provided a dataset from UCI Machine Learning Database, having 8 different factors: house price, transaction year, house age, distance to nearest MRT station, number of convenience stores, latitude, longitude, and transaction month. We will test these factors to see which of them, if any, significantly affect the real estate prices.

**Approach:**

In order to understand the dataset better, our first task at hand was to perform extensive exploratory data analysis. The purpose here was to identify variables where interesting patterns are observed. Similarly, we had to use feature engineering and variable selection to get the best model results. Another task at hand was performing model diagnostics to ensure that the model assumptions were remaining true. We applied various machine learning algorithms starting from Multiple Linear Regression, Ridge Regression, and Random Forest.
Feature Engineering was performed separately for each of the 3 models. Hyperparameters were tuned to achieve a lower root mean square error value. Our best model performance was observed using the Multiple Linear Regression with an RMSE value of **5.919964**.

**Conclusion:**

The purpose of this project was to propose a real estate valuation approach using the given set of features so that it overcomes the traditional approach. 
The independent variables included- transaction date,  age of the house, distance to nearest MRT station, number of convenience stores, latitude, longitude, and transaction month. 
The findings are as follows:

[1] In the Multiple Linear Regression model, we got the lowest prediction error by removing the Month variable, followed by applying log transformation on the target variable and the distance from the MRT stations

[2] When we compare the coefficients of the features MLR and Ridge regression, we note that the ridge penalty is shrinking the coefficient of the features that are less important. For instance, the coefficient of the number of stores is 1.214 in MLR, while it is 1.192532e-02 in Ridge regression. We observe a similar trend for the variables house age, latitude, longitude.

[3] Using the random forest model, we found that distance to the nearest MRT Station is the most important variable in determining a house price, followed by the Latitude (geographic location). Additionally, month and transaction date have the least importance when trying to determine the house price.




**References**:

UCI Machine Learning Repository: Real estate valuation data set Data Set. (2018, August 18). UCI Machine Learning Repository. https://archive.ics.uci.edu/ml/datasets/Real+estate+valuation+data+set

Hoerl, A. (n.d.). Ridge Regression: Biased Estimation for Nonorthogonal Problems on JSTOR. Jstor. 

What is Feature Engineering? Definition and FAQs | OmniSci. (n.d.). Omnisci. https://www.omnisci.com/technical-glossary/feature-engineering
