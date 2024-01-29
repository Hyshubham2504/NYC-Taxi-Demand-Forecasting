NYC Yellow Taxi Demand Prediction using Machine Learning

Business Understanding
In 2011, Uber was launched and since then the usage of yellow taxis came to a decline. It mostly happened because Uber allowed anyone to enroll as a taxi driver with their own private vehicle and making it as easy as a click in the UBer app to book a ride. The most importance thing is to minimize the vacant driving time, and it is important to know the location of passengers.

Solution:- To make an application with a great UI or We can do analysis and leverage machine learning to help the drivers relocate to a place with higher demand.

Objective:- 
1) Do intensive data analysis to give a tip to drivers on when and where in particular they can find demand.
2) Predict the number of pickups as accurate as possible for each region in a given time interval.

Sub-Problem for ML mapping:-
1) Dividing NYC into smaller regions - Unsupervised ML
2) Time Series prediction problem - Predicting the number of pickups

Performance Metric Used:-
Mean Absolute Precentage Error

Conclusion:-
1) The Manhattan(downtown) has the highest demand in the entire NYC which comprises of 93.88% of total pickups.
2) Friday has the highest demand followed by weekends.
3) There is no trend in the data but we have a seasonality of 1 day.
4) Exponential Weighted Averages worked as the best baseline model for featurization for supervised ML.
5) Through XGB, we found an MAPE to be 14.2%

Challenges to address:-
1) Latency in providing insights to the driver for the region with high density
2) Need to integrate weather data, as it has a great influence on taxi services. This is something we saw during analysis, during 25-27 Jan 2016, there was a blizzard in NYC,
which disrupted the taxi service for 3 days.
3) We analysed on 1 month data(12.5 million records), a better way will be to analyse for a couple of years.
4) We used smoothing to deal with 0 pickups during some time interval which may impact the model accuracy.
