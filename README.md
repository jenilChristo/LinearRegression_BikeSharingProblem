# Bike Sharing - Demand Forecasting using Multiple Linear Regression

# Problem Statement

A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.


A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state. 


In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.


They have contracted a consulting company to understand the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market. The company wants to know:

Which variables are significant in predicting the demand for shared bikes.
How well those variables describe the bike demands
Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the American market based on some factors. 


# Business Goal

You are required to model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market. 


# Engineering Goals
- To identify the driving factors that increase the demand 
- To model the demand for shared bikes and use it to make approprite business decisions to solve the revenue issue
- The forecasting model should predict the demand accurately and this information can be leveraged by the company to meet the future demand spike.
- Achieve model accuracy the best posible and take care of multicollinearity 
- Validate all the assumptions of multiple linear regression



## Model Conclusions
- <b>Model Summary of FINAL MODEL:</b><br>
    ![Modelsummary](https://github.com/jenilChristo/LinearRegression_BikeSharingProblem/blob/main/final_model_summary.png)
  - The top 4 influence on the bike booking /demand

    - temp : A coefficient value of   4017.586 indicated that a unit increase in temp variable increases the bike demand by same number, provided all other variables are held constant

    - season_winter : A coefficient value of 459.0835 indicated that a unit increase in season_winter variable increases the bike demand by same number, provided all other variables are held constant

    - weathersit_clear : A coefficient value of 747.949 indicated that a unit increase in weathersit_clear variable increases the bike demand by same number, provided all other variables are held constant

    - yr : A coefficient value of 2033.1428 indicated that a unit increase in yr variable increases the bike demand by same number, provided all other variables are held constant

- Summary of train data 
     - Actual and predicted is almost same - The model is good
     - R2 score of y_train vs y_train_cnt is almost same as model R2 score
     R2_score of train data - 0.7819417778097163
     R2_Score of test data - 0.7759901851504777

- Summary of test data
     - Variance of the residuals (error terms) is constant across predictions. i.e error term does not vary much as the value of the predictor variable changes.
     - Actual and predicted is almost same on test data
     - R2 score of y_test vs y_test_cnt is almost same but has slight variation of .00595 which is acceptable when compared with R2 score of model
     
     ![Pred vs test](https://github.com/jenilChristo/LinearRegression_BikeSharingProblem/blob/main/actualvspredicted.jpeg)

     


## Technologies Used
- NumPy - version 1.21.6
- Pandas - version 1.1.5
- Matplotlib - version 3.2.1
- Seaborn - version 0.12.2
- statsmodels - version 0.11.0
- scikit-learn - version 0.22.1.

