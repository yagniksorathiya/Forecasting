# Forecasting

## Problem Statement

Forecast the CocaCola prices and Airlines Passengers data set. Prepare a document for each model explaining how many dummy variables you have created and RMSE value for each model. Finally which model you will use for Forecasting.

# ➳ Time Series Analysis and Forecasting

![temp](https://github.com/yagniksorathiya/Forecasting/assets/129974278/8416a0f3-ab17-458c-80fc-5eb8cb9b5094)

Time Series Analysis is a way of studying the characteristics of the response variable concerning time as the independent variable. To estimate the target variable in predicting or forecasting, use the time variable as the reference point. TSA represents a series of time-based orders, it would be Years, Months, Weeks, Days, Horus, Minutes, and Seconds. It is an observation from the sequence of discrete time of successive intervals. Some real-world application of TSA includes weather forecasting models, stock market predictions, signal processing, and control systems. Since TSA involves producing the set of information in a particular sequence, this makes it distinct from spatial and other analyses. We could predict the future using AR, MA, ARMA, and ARIMA models.

## ↳ What Is Time Series Analysis?

Time series analysis is a specific way of analyzing a sequence of data points collected over time. In TSA, analysts record data points at consistent intervals over a set period rather than just recording the data points intermittently or randomly.

### Objectives of Time Series Analysis

+ To understand how time series works and what factors affect a certain variable(s) at different points in time.
+ Time series analysis will provide the consequences and insights of the given dataset’s features that change over time.
+ Supporting to derive the predicting the future values of the time series variable.
+ Assumptions: There is only one assumption in TSA, which is “stationary,” which means that the origin of time does not affect the properties of the process under the statistical factor.

## ↳ Introduction

Time Series Analysis is a way of studying the characteristics of the response variable concerning time as the independent variable. To estimate the target variable in predicting or forecasting, use the time variable as the reference point. TSA represents a series of time-based orders, it would be Years, Months, Weeks, Days, Horus, Minutes, and Seconds. It is an observation from the sequence of discrete time of successive intervals. Some real-world application of TSA includes weather forecasting models, stock market predictions, signal processing, and control systems. Since TSA involves producing the set of information in a particular sequence, this makes it distinct from spatial and other analyses. We could predict the future using AR, MA, ARMA, and ARIMA models. In this article, we will be decoding time series analysis for you.

## ↳ What Is Time Series Analysis?

Time series analysis is a specific way of analyzing a sequence of data points collected over time. In TSA, analysts record data points at consistent intervals over a set period rather than just recording the data points intermittently or randomly.

### Objectives of Time Series Analysis

+ To understand how time series works and what factors affect a certain variable(s) at different points in time.
+ Time series analysis will provide the consequences and insights of the given dataset’s features that change over time.
+ Supporting to derive the predicting the future values of the time series variable.
+ Assumptions: There is only one assumption in TSA, which is “stationary,” which means that the origin of time does not affect the properties of the process under the statistical factor.

## ↳ How to Analyze Time Series?

To perform the time series analysis, we have to follow the following steps:

+ Collecting the data and cleaning it
+ Preparing Visualization with respect to time vs key feature
+ Observing the stationarity of the series
+ Developing charts to understand its nature.
+ Model building – AR, MA, ARMA and ARIMA
+ Extracting insights from prediction

### Significance of Time Series

TSA is the backbone for prediction and forecasting analysis, specific to time-based problem statements.

+ Analyzing the historical dataset and its patterns
+ Understanding and matching the current situation with patterns derived from the previous stage.
+ Understanding the factor or factors influencing certain variable(s) in different periods.

With the help of “Time Series,” we can prepare numerous time-based analyses and results.

+ **Forecasting:** Predicting any value for the future.
+ **Segmentation:** Grouping similar items together.
+ **Classification:** Classifying a set of items into given classes.
+ **Descriptive analysis:** Analysis of a given dataset to find out what is there in it.
+ **Intervention analysis:** Effect of changing a given variable on the outcome.

### Components of Time Series Analysis

Let’s look at the various components of Time Series Analysis:

+ **Trend** - The trend shows a general direction of the time series data over a long period of time. A trend can be increasing(upward), decreasing(downward), or horizontal(stationary).
+ **Seasonality** - The seasonality component exhibits a trend that repeats with respect to timing, direction, and magnitude. Some examples include an increase in water consumption in summer due to hot weather conditions.
+ **Cyclical Component** - These are the trends with no set repetition over a particular period of time. A cycle refers to the period of ups and downs, booms and slums of a time series, mostly observed in business cycles. These cycles do not exhibit a seasonal variation but generally occur over a time period of 3 to 12 years depending on the nature of the time series.
+ **Irregular Variation** - These are the fluctuations in the time series data which become evident when trend and cyclical variations are removed. These variations are unpredictable, erratic, and may or may not be random.
+ **ETS Decomposition** - ETS Decomposition is used to separate different components of a time series. The term ETS stands for Error, Trend and Seasonality.

![component of time series](https://github.com/yagniksorathiya/Forecasting/assets/129974278/71b66498-8812-4337-b194-a2fd30faaff5)

## ↳ What Are the Limitations of Time Series Analysis?

Time series has the below-mentioned limitations; we have to take care of those during our data analysis.

+ Similar to other models, the missing values are not supported by TSA
+ The data points must be linear in their relationship.
+ Data transformations are mandatory, so they are a little expensive.
+ Models mostly work on Uni-variate data.

## ↳ Data Types of Time Series

Let’s discuss the time series’ data types and their influence. While discussing TS data types, there are two major types – stationary and non-stationary.

**Stationary:** A dataset should follow the below thumb rules without having Trend, Seasonality, Cyclical, and Irregularity components of the time series.

+ The **mean** value of them should be completely constant in the data during the analysis.
+ The **variance** should be constant with respect to the time-frame
+ **Covariance** measures the relationship between two variables.

**Non- Stationary:** If either the mean-variance or covariance is changing with respect to time, the dataset is called non-stationary.

![type of datat](https://github.com/yagniksorathiya/Forecasting/assets/129974278/f1f70cc1-4030-47ef-8dfb-7722ce457047)

## ↳ Methods to Check Stationarity

During the TSA model preparation workflow, we must assess whether the dataset is stationary or not. This is done using **Statistical Tests**. There are two tests available to test if the dataset is stationary:

+ Augmented Dickey-Fuller (ADF) Test
+ Kwiatkowski-Phillips-Schmidt-Shin (KPSS) Test

### Augmented Dickey-Fuller (ADF) Test or Unit Root Test

The ADF test is the most popular statistical test. It is done with the following assumptions:

+ Null Hypothesis (H0): Series is non-stationary
+ Alternate Hypothesis (HA): Series is stationary

      p-value >0.05 Fail to reject (H0)
      p-value <= 0.05 Accept (H1)

### Kwiatkowski–Phillips–Schmidt–Shin (KPSS) Test

These tests are used for testing a NULL Hypothesis (HO) that will perceive the time series as stationary around a deterministic trend against the alternative of a unit root. Since TSA is looking for Stationary Data for its further analysis, we have to ensure that the dataset is stationary.

## ↳ Converting Non-Stationary Into Stationary

Let’s discuss quickly how to convert non-stationary to stationary for effective time series modeling. There are three methods available for this conversion – detrending, differencing, and transformation.

### Detrending

It involves removing the trend effects from the given dataset and showing only the differences in values from the trend. It always allows cyclical patterns to be identified.

### Differencing

This is a simple transformation of the series into a new time series, which we use to remove the series dependence on time and stabilize the mean of the time series, so trend and seasonality are reduced during this transformation.

+ Yt= Yt – Yt-1
+ Yt=Value with time

#### Transformation

This includes three different methods they are Power Transform, Square Root, and Log Transfer. The most commonly used one is Log Transfer.

## ↳ Moving Average Methodology

The commonly used time series method is the Moving Average. This method is slick with random short-term variations. Relatively associated with the components of time series.

**The Moving Average (MA) (or) Rolling Mean:** The value of MA is calculated by taking average data of the time-series within k periods.

Let’s see the types of moving averages:

+ Simple Moving Average (SMA),
+ Cumulative Moving Average (CMA)
+ Exponential Moving Average (EMA)

## ↳ Time Series Analysis in Data Science and Machine Learning

When dealing with TSA in Data Science and Machine Learning, there are multiple model options are available. In which the Autoregressive–Moving-Average (ARMA) models with [p, d, and q].

+ P==> autoregressive lags
+ q== moving average lags
+ d==> difference in the order

Before we get to know about Arima, first, you should understand the below terms better.

+ Auto-Correlation Function (ACF)
+ Partial Auto-Correlation Function (PACF)

### Auto-Correlation Function (ACF)

ACF indicates how similar a value is within a given time series and the previous value. (OR) It measures the degree of the similarity between a given time series and the lagged version of that time series at the various intervals we observed.

Python Statsmodels library calculates autocorrelation. It identifies a set of trends in the given dataset and the influence of former observed values on the currently observed values.

### Partial Auto-Correlation (PACF)

PACF is similar to Auto-Correlation Function and is a little challenging to understand. It always shows the correlation of the sequence with itself with some number of time units per sequence order in which only the direct effect has been shown, and all other intermediary effects are removed from the given time series.

## ↳ Types of Auto-Correlation

![The-plots-of-the-autocorrelation-function-ACF-and-partial-autocorrelation-function](https://github.com/yagniksorathiya/Forecasting/assets/129974278/9745f4a5-0f76-4f48-a341-f9cbd44e73f3)

#### Interpret ACF and PACF Plots

ACF	                      |   PACF	                 |    Perfect ML -Model
:-----------------------: | :----------------------: | :----------------------:
Plot declines gradually	  | Plot drops instantly	   | Auto Regressive model.
Plot drops instantly	    | Plot declines gradually	 | Moving Average model
Plot decline gradually	  | Plot Decline gradually	 | ARMA
Plot drop instantly	      | Plot drop instantly	     | You wouldn’t perform any model

Remember that both ACF and PACF require stationary time series for analysis.

## ↳ What Is an Auto-Regressive Model?

An auto-regressive model is a simple model that predicts future performance based on past performance. It is mainly used for forecasting when there is some correlation between values in a given time series and those that precede and succeed (back and forth).

An AR is a Linear Regression model that uses lagged variables as input. By indicating the input, the Linear Regression model can be easily built using the scikit-learn library. Statsmodels library provides autoregression model-specific functions where you must specify an appropriate lag value and train the model. It is provided in the AutoTeg class to get the results using simple steps.

+ Creating the model AutoReg()
+ Call fit() to train it on our dataset.
+ Returns an AutoRegResults object.
+ Once fit, make a prediction by calling the predict () function

The equation for the AR model (Let’s compare Y=mX+c)

**Yt =C+b1 Yt-1+ b2 Yt-2+……+ bp Yt-p+ Ert**

#### Key Parameters

+ p=past values
+ Yt=Function of different past values
+ Ert=errors in time
+ C=intercept

## ↳ Understanding ARMA and ARIMA

**ARMA** is a combination of the Auto-Regressive and Moving Average models for forecasting. This model provides a weakly stationary stochastic process in terms of two polynomials, one for the Auto-Regressive and the second for the Moving Average.

![ARMA -formula](https://github.com/yagniksorathiya/Forecasting/assets/129974278/a70b78b1-a1f4-4bab-beb0-dc1b1e42b1a6)

ARMA is best for predicting stationary series. **ARIMA** was thus developed to support both stationary as well as non-stationary series.

![ARIMA](https://github.com/yagniksorathiya/Forecasting/assets/129974278/fec91f47-d39c-4cb6-8cdf-a8d3758eae29)

+ AR ==> Uses past values to predict the future.
+ MA ==> Uses past error terms in the given series to predict the future.
+ I==> Uses the differencing of observation and makes the stationary data.

**AR+I+MA= ARIMA**

## ↳ Understand the signature of ARIMA

+ p==> log order => No of lag observations.
+ d==> degree of differencing => No of times that the raw observations are differenced.
+ q==>order of moving average => the size of the moving average window

### Implementation Steps for ARIMA

+ Plot a time series format
+ Difference to make stationary on mean by removing the trend
+ Make stationary by applying log transform.
+ Difference log transform to make as stationary on both statistic mean and variance
+ Plot ACF & PACF, and identify the potential AR and MA model
+ Discovery of best fit ARIMA model
+ Forecast/Predict the value using the best fit ARIMA model
+ Plot ACF & PACF for residuals of the ARIMA model, and ensure no more information is left.

## ↳ Process Flow (Re-Gap)

![flowchart-model-selection](https://github.com/yagniksorathiya/Forecasting/assets/129974278/fd66e2d2-3075-43fc-a394-1a9460d53636)

In recent years, the use of Deep Learning for Time Series Analysis and Forecasting has increased to resolve problem statements that couldn’t be handled using Machine Learning techniques.
