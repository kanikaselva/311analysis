# A Predictive and Cluster-Based Analysis of 311 Service Calls in Pittsburgh

### 90803 Machine Learning Foundations with Python

### By Kanika Selvapandian, Claire Woodrow, Chengyi Cai

## Background:

Pittsburgh implemented its first official 311 system in 2006. Similarly to today, community members could report issues and request service in many ways: over the phone, through the mail, or in in-person, among others. Since 2006, the 311 system’s management software has been updated several times, bringing improvements to the operation.

Our project’s goal is to help the Allegheny County 311 system managers decrease their response time to reports. In many cases, while 311 calls are not emergencies, the reported problems have public health and safety implications. It is important to have more efficient response times and better closure rates, especially for health and safety-related reports, because it could significantly improve resident safety.

We hope to increase efficiency by way of predicting the amount of time it will take each type of case to close. While we work to achieve our main goal of improved, more efficient service, we also hope to maintain equity in the length of response time among neighborhoods.

## Objectives:

1. **Analyzing Trends Across Neighborhoods to Identify Underlying Factors**
   Leverage unsupervised learning methods to uncover hidden patterns in the 311 data and compare it with Pittsburgh’s neighborhood data. By analyzing trends across neighborhoods and incorporating additional factors such as demographics, infrastructure, and local conditions, we can identify the root causes of varying closure times and call volumes.
2. **Predicting How Long it Will Take to Address Requests**
   By using machine learning algorithms, such as regression models or time series analysis, we can estimate the closure time for each new service request based on factors such as request type, neighborhood, department, and other factors. This predictive model will allow city agencies to anticipate the resources needed to address specific issues and allocate personnel, equipment, and budget accordingly. The outcome variable used here is time_taken.
3. **Forecasting the Number of Future Service Requests**
   As requests vary seasonally, we plan to analyze past data on the frequency and types of requests in previous years or months to identify recurring patterns or anomalies. These forecasts will enable municipalities and service departments to anticipate periods of higher demand and plan accordingly. The outcome variable used would be the number of future service requests in a specific time frame, categorised by request type and origin.

## Instructions:

* Clone our github repository to your local machine using `https://github.com/kanikaselva/311analysis`
* Go to `https://data.wprdc.org/dataset/311-data/resource/29462525-62a6-45bf-9b5e-ad2e1c06348d` and download 311 Data in csv format and add it to the Data folder of this repository locally.
* Run `0. FilterData.ipynb` to filter the dataset to the most recent 5 years
* Run the following files in order to clean, perform EDA and analysis using machine learning models:
  * CleanData.ipynb
  * EDA.ipynb
  * NeighborhoodAnalysis.ipynb
  * PredictTimeTaken.ipynb
  * SeasonalForecast.ipynb
  * BiasAudit.ipynb

## Packages to Install:

To run all the files smoothly, the following packages have to be installed:

1. pandas
2. numpy
3. scikit
4. matplotlib
5. plotly
6. seaborn
7. sklearn
8. xgboost
9. warnings

If not installed, these files can be added by running the code `pip install (package name)` in the terminal.
