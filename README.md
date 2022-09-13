# BoomBikes Sharing-Linear-Regression-Assignment
> A Multiple Linear Regression Model using RFE.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## Problem Statement
A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.


A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state. 


In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.


They have contracted a consulting company to understand the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market. The company wants to know:

Which variables are significant in predicting the demand for shared bikes.
How well those variables describe the bike demands
Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the American market based on some factors. 


## Business Goal
You are required to model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market. 

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- We did train-test split with train_size = 70% and test_size=30%.
- We built Linear Regression Model for the given problem statement.
- Temp alone can explain 41.1 % of the variance for counts.
- We adopted RFE for feature selection.
- All the assumptions that are for Linear Regression all have been tested ( Normal distribution , Autocorrelation, Multicollinearity )
- Analysis on the Residuals have been done as well.
- We have a Mean Squared Error close to 0 on the training dataset, meaning our model is able to correctly predict all variances in the data.
- On the test validation dataset, MSE is 0.01 also close to zero, meaning our model is able perform similarly on unknown data sets too.
- We have a R-squared value of 83.66 % on train data and 80.4% on test data (Model Accuracy = 80.4 %)
- Best fit line is
- Count = 0.1430 + 0.2350 x year + 0.0411 x workingday + 0.4890 x temp - 0.1462 x windspeed + 0.0672 x Sep + 0.0561 x Mon - 0.2717 x Light Snow - 0.0787 x (Mist + Cloudy)  - 0.0604 x Spring + 0.0592 x Summer + 0.0957 x Winter


## Technologies Used
- numpy - 1.21.5
- pandas - 1.4.2
- matplotlib - 3.5.1
- seaborn - 0.11.2
- statsmodels - 0.13.2
- pandas_profiling - 3.3.0
- sklearn - 1.0.2



