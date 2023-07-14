# Bike Sharing Assignment
> Objective is to build a required model that predict the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. Based on the model prediction/ demand understand, the stretegy will be manipulated to meet the demand levels and meet the customer's expectations. The most fit model will be further way for understand the demand dynamics of a new market.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Analysis Involved] (#analysis-involved)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- Dataset of bike sharing details from the company
- The objective is to predict the booking demand by various independent variables
- day.csv (Bike booking data)

## analysis-involved

1. *Univariate Analysis:*
- Humidity is high between 50-70
- No Outliers

2. *Bivariate Analysis:*
- Season (Fall seem to have more bookings)
- The next year the booking numbers is grown
- Booking in Jun, Jul, Aug, Sep and Oct are high. Sep has high no of booking among them
- Year-end and Year-Beginning have less amount of bookings
- When its not holiday booking has less numbers
- Fri, Sat and Sunday has more no of bookings
- In Clear weather set, The booking numbers are increasing.

2. *Correlation Analysis:*
- between temp and atemp the correlation is 0.99 which is almost 1, indicating that these two varaibles has linear relationship
- temp & atemp has linear relationship with cnt (Target Variable)

3. *Correlation Coefficient:*
- cnt has a good correlation with temp, yr & atemp
- Season Spring with Jan & Feb has a correaltion
- winter with oct & nov has a good correlation
- hum with Misty has a good correlation
- cnt has a positive correlation with temp

4. *Building Model:*
- Model_1 (workingday has high VIF value-Dropped)
- Model_2 (hum has high VIF value-Dropped)
- Model_3 (sat has high p-value-Dropped)
- Model_4 (Has the perfect p-value for all the variables, and has the good r2(0.8409) and adjusted-r2(0.8313))

5. *Error Distribution:*
- From the train dataset actual and predicction-Errors are normally distributed with 0 as mean value

6. *R2 & Adjusted R2 Comparision:*
- R2 of test dataset-0.808
- Ajdusted R2 of test dataset-0.7969

## Conclusion
**Model_4 is the best fit for the cnt prediction**

Bike booking is depends on the following variables:<br><br>
- Season (Summer & Fall)
- Year
- Month (Jun, Jul, Aug, Sep and Oct)
- Holiday
- Weekend (Sunday)
- Weather sit (Clear, Misty, Cloudy)
- temp
- windspeed

*Having best r2 and adjusted r2 between train & test datasets*

These variables can be considered in the prediction of booking demand

## Technologies Used
- seaborn - version 0.12.2
- pandas - version 2.0.3
- matplotlib - version 3.7.2
- numpy - version
- statsmodels - version 0.14.0
- scikit-learn - version 1.3.0

## Contact
Created by [@rgurum](https://www.linkedin.com/in/gurumoorthiramanathan/) - feel free to contact me!