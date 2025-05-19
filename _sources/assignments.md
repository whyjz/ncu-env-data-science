# Assignments

## Problem set #1

1. Complete Exercise 4.1 in Hsieh's book.
2. Complete Exercise 4.5 in Hsieh's book. (Source data: `SWE_Nino_Nina.csv`)
3. Complete Exercise 4.6 in Hsieh's book. (Source data: `nino12_long_anom.csv` & `nino34_long_anom.csv`)
4. For the SWE data in `SWE_Nino_Nina.csv`, calculate the 95% CI of their median value using bootstrapping. Be sure to avoid the percentile method.
5. Reproduce the figure for Q3 in the Pre-course Quiz. ([Figure Link](https://drive.google.com/file/d/15WejYTcSHDGM3VNoX32WaD5r8l-BNNF-/view?usp=sharing)) *Figure credit: Nicolas P. Rougier (2021)*.

## Problem set #2

1. Complete Exercise 5.7 in Hsieh's book. (Source data: `Milwaukee_wind_direction_ozone.csv`)
2. Visualize `SWE_tele.csv` and make a few arguments that the generated figures can visually support.
3. Complete Exercise 5.8 in Hsieh's book. (Source data: `SWE_tele.csv`)
4. Complete Exercise 5.9 in Hsieh's book. (Source data: `SWE_tele.csv`)

## Problem set #3

1. Complete Exercise 6.5 in Hsieh's book. Please use the cross-validation technique to tune at least one model hyperparameter. (Source data: `SWE_tele.csv`)
2. Complete Exercise 8.1 in Hsieh's book. Please tune the learning rate for the MLP NN model. I have generated the input data for you, which can be downloaded from [this link](https://drive.google.com/drive/folders/1_qCa8-g6zYXFj7Pz8RD1JEj3hgtImE5O?usp=sharing) (`data_noise-*.csv`). 
3. Visualize the regression results of Exercise 8.1 at least for the case with the Gaussian noise at 0.5 times the standard deviation of $ y_{\textrm{signal}}$. 

## Problem set #4

1. Complete Exercise 12.1 in Hsieh's book. For subquestion (a), visualize the results to reproduce Figure 12.1(b). Make sure to label/mark correct and incorrect predictions. (Source data: `forest_testing.csv` & `forest_testing.csv`)
2. Following the first question, use the support vector machine to classify the forest types in the given dataset. Feel free to choose one-versus-the-rest or one-versus-one approach (and specify your choice). Train using the first two predictors and compare the results with the linear discriminant analysis by visualizing them similarly.
3. Generate a synthetic signal with added noise $y = \sin x + 0.5 \times \mathcal{N}(0, 1)$ and collect 40 data points that are distributed within the range $x = [0, 4\pi]$. Now use (a) ridge regression, (b) kernel ridge regression, and (c) Gaussian process regression to model the data and give the prediction in the range $x = [0, 8\pi]$ with visualization. Describe and justify your kernel selection and hyperparameter tuning process whenever necessary. Compare the results from three regression methods.

## Problem set #5

1. Complete Exercise 12.5 in Hsieh's book. Please use the Linear Discriminant Analysis (LDA) model. You'll need to determine some details about how to process the data. Specify them. (Source data: `SydneyAirport_weather.csv`)
2. Complete Exercise 14.3 in Hsieh's book. Please use the same preprocessing workflow as in the previous question for the data. Challenge yourself and see if you can build a better model than LDA! (Source data: `SydneyAirport_weather.csv`)
3. Complete Exercise 14.5 in Hsieh's book, including (b). Visualize the regression results by plotting the data and predictions alongside several important predictors. (Source data: `bike_sharing_daily_data.csv` & `bike_sharing_Readme.txt`)


<!-- 

## Problem set #5

Complete the following exercises in Hsieh's book with the specified requirements:

1. Exercise 14.2, including (c)
2. Exercise 12.5, but develop two prediction models instead of one. One of the models must be a random forest or a boosting model.
3. Exercise 14.4, including (b) -->