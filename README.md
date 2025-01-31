## Business Problem Statement
A retail convenience chain, Maverik, fuels adventures in more than 380 locations across 12 western states. Maverik is known for premium BonFire food, diesel and unleaded fuel, and in-store merchandise. The company is on an expansion spree and as part of its growth, it recently acquired “ Kum & Go” nearly doubling its store count.

The company is planning to open 30 new stores yearly in a new market, and it needs to forecast daily sales for the new store. This is crucial for financial planning and return on investment (ROI) assessment for these new stores. The challenge lies in predicting the first-year sales for these newly acquired stores accurately.

We have limited amount of data; therefore, we will be using currently available historical dataset to address analytical problems we will be addressing in this project are identifying trends and patterns in sales data, understanding the relationship between sales and other factors, and identifying outliers and anomalies. By addressing these analytical problems, we will be able to build a sales forecasting model.

We will develop a sales forecasting model that can accurately predict daily sales for the new store. We will be using a variety of forecasting methods, such as time series analysis, regression analysis, causal analysis, and machine learning. The model will be evaluated by comparing its prediction to actual sales data from a holdout dataset. The model performance will be evaluated using industry-standard metrics such as Forecast Accuracy Metrics (e.g. MAE, MAPE, RMSE) and its ability to update forecasts dynamically in response to new data.

This sales forecasting model will help the company to make informed decisions about staffing, inventory, and marketing for the new stores. This can help the company to maximize its profits and minimize its losses while maintaining customer satisfaction.

#### Please see our full EDA and Modeling Notebook by clicking on the link below. You will also find a detailed explanation of our analytical findings.
https://github.com/only2venkat/Bonfire_capstone/blob/3a93c0dd35b2225a96c0a2d9080fa5b937cfe7a0/Model_notebook.ipynb

Time Series Forecasting and Analysis Overview:
This repository showcases our work on time series forecasting models for Maverik. Our analysis focused on various forecasting techniques, including ARIMA, SARIMA, ETS, and Prophet, driven by insights from exploratory data analysis revealing prominent seasonality patterns in the sales data.

#### Key Insights:
Decomposition and Stationarity: Identified distinct patterns in sales data and confirmed stationarity, vital for ARIMA and SARIMA models.
Clustering and Prophet Model: Cluster analysis revealed varied Prophet model performances across different sales categories, highlighting opportunities for refinement.
ARIMA and SARIMA Challenges: While ARIMA showed promise, challenges in capturing complex sales patterns were observed. SARIMA struggled with weekly seasonality and holiday considerations.

#### Next Steps:
Prophet Model Optimization: Deeper hyperparameter tuning and custom adjustments for improved accuracy, especially in Cluster 
1.Model Ensemble and Validation: Exploration of ensemble models for enhanced accuracy and thorough cross-validation techniques for validation and fine-tuning.
Communication and Reporting: Clear and concise communication of findings, emphasizing model strengths and limitations for effective decision-making.
Continuous Monitoring and Updating: Establishment of a monitoring system for ongoing model performance updates with new data.
Our goal is to refine existing models, explore alternative approaches, and elevate forecasting capabilities to provide actionable insights for Maverik's strategic decisions.
