
# Thesis Title (MTech Project)

HEADWAY BASED BUS BUNCHING PREDICTION IN URBAN HETEROGENOUS TRAFFIC ENVIRONMENTS 


## Authors

- [@Balasaheb Mule](https://github.com/Balasaheb-Mule)


## Intoduction
This thesis addresses the problem of bus bunching by proposing a headway-based bus bunching prediction model which will predict the bunching phenomena at least five stops ahead with adequate accuracy using machine learning (ML) algorithms. 
## About Dataset
Bus GPS trajectory data was collected from West Bengal Transportation Corporation (WBTC) for a period of 2 months of Kolkata City. Data consists of variables like bus ID, its latitude, and longitude with respect to time stamps. It has many other features like 'location_data_id', 'entry_date', 'device_id', 'event_location', 'segment_id', 'region_id' & 'journey_id'. Data showing updated positions of buses every 01 to 02 minutes. High-frequency bus routes are considered for this study. Selected routes are AC1 down which starts from Howrah station & terminates at Jadhavpur.
## Methodology
**1. Identification of Bus Bunching Instances :**
<br> A "bus bunching" event occurs when the headway between two buses is less than a certain threshold, denoted by α. Mathematically, it's defined as: BBk = 1 if hk < α, and 0 otherwise. Here, α is typically based on scheduled data, and in our case, we set it to α = hk/3, where hk is the scheduled headway. The objective is to construct a model, f(X), capable of forecasting the probability of bus bunching for every pair of buses operating along the same route.

**2. Prediction of bus bunching**
<br> For single step model : The independent features which were input to this prediction model were headway between leading and following buses at current stop, travel time of leading vehicle from current stop to next stop, dwell time of both the vehicles at current stop, historical mean and standard deviation  of travel time of following bus from current stop till next stop, dwell time of both the vehicles at current stop, historical mean of time headway of next stop. These features were input to the models as independent variables and time headway between that pair of leading & following buses at next stop was dependent variable which were to be predicted.
## Model Evaluation Matrix
The performance of the trained regression model of headway prediction was evaluated using various metrics, including R-squared (R2) score, adjusted R-squared score, mean squared error (MSE), root mean squared error (RMSE), and mean absolute error (MAE), mean absolute percentage error (MAPE). MAPE provides insights into the percentage deviation between predicted and actual values, offering a measure of the model's accuracy in predicting bus bunching instances. Additionally, the model's performance was assessed on the entire dataset to evaluate its generalization ability.
## Analysis & Results
The trained model exhibited promising performance, as evidenced by high R-squared scores and low error metrics. Collinearity among features was assessed using a correlation matrix, providing insights into the relationships between different features and their impact on the model's predictive capabilities. Overall, the developed headway based predictive model provides a valuable tool for transit agencies to anticipate and mitigate instances of bus bunching in both single and multiple stop segments, contributing to improved efficiency and reliability of transit services.

## Conclusion
•	SVM model outperformed over other machine learning models with  R-squared values of 0.92 & 0.86 for single and multi step model with RMSE values of headway were 42 seconds and 62 seconds, which is acceptable, proves positive performance of model
<br> •	Addition of variables based on historical data aided model performance. Hence, utilization of historical data along with real time inputs is recommended
<br> •	Prediction horizon till next 5 stops was achieved with acceptable RMSE values.

## Detailed Thesis Report
The comprehensive thesis report can be accessed via this google drive link for any further clarification :
https://drive.google.com/drive/folders/1nzXzQ01KGi7MeUarfBmJ0ruZR391GYXb?usp=sharing
