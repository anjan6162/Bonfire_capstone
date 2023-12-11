## Business Problem Statement
A retail convenience chain, Maverik, fuels adventures in more than 380 locations across 12 western states. Maverik is known for premium BonFire food, diesel and unleaded fuel, and in-store merchandise. The company is on an expansion spree and as part of its growth, it recently acquired “ Kum & Go” nearly doubling its store count.

The company is planning to open 30 new stores yearly in a new market, and it needs to forecast daily sales for the new store. This is crucial for financial planning and return on investment (ROI) assessment for these new stores. The challenge lies in predicting the first-year sales for these newly acquired stores accurately.

We have limited amount of data; therefore, we will be using currently available historical dataset to address analytical problems we will be addressing in this project are identifying trends and patterns in sales data, understanding the relationship between sales and other factors, and identifying outliers and anomalies. By addressing these analytical problems, we will be able to build a sales forecasting model.

We will develop a sales forecasting model that can accurately predict daily sales for the new store. We will be using a variety of forecasting methods, such as time series analysis, regression analysis, causal analysis, and machine learning. The model will be evaluated by comparing its prediction to actual sales data from a holdout dataset. The model performance will be evaluated using industry-standard metrics such as Forecast Accuracy Metrics (e.g. MAE, MAPE, RMSE) and its ability to update forecasts dynamically in response to new data.

This sales forecasting model will help the company to make informed decisions about staffing, inventory, and marketing for the new stores. This can help the company to maximize its profits and minimize its losses while maintaining customer satisfaction.

## Exploratory Data Analysis (EDA) Key Findings:

### Correlation Analysis:
The examination of store sales and demographic factors revealed notable correlations. Food service and inside sales demonstrated a high correlation, indicating a tendency for these categories to move in tandem. A moderate correlation was observed between diesel and food service sales, suggesting a positive relationship, albeit not as strong as that between food service and inside sales.

### Day-of-Week Trends:
Sales analysis across days highlighted significant trends. Sunday emerged as the slowest day, while Friday recorded the highest sales, indicating increased shopping activity on weekends. This insight suggests potential benefits for businesses to offer special promotions or discounts on Fridays. Moreover, holidays exhibited higher average sales, emphasizing the influence of festive occasions on consumer spending.

### Holiday-Specific Insights:
Christmas and Thanksgiving consistently recorded the highest average sales across all categories, underscoring their significance as peak shopping periods. Conversely, New Year's Day and New Year's Eve marked the lowest average sales, possibly due to a focus on celebratory activities rather than shopping.

### Demographic Factors and Sales Correlation:
The analysis identified correlations between store sales and demographic factors. Notably, the presence of bonfire_grill and pizza showed a strong positive correlation with food service sales. Additionally, a positive correlation was observed between the employee-to-population ratio and store sales, suggesting potential benefits for businesses located in areas with a higher employee-to-population ratio.

### Seasonal Store Openings:
A notable observation was the seasonal trend in store openings, with a higher frequency in summer and spring, and comparatively fewer openings in winter.

### Soft Opening Sales Trends:
Analyzing soft opening dates revealed consistent patterns. Day-2 of soft opening dates consistently recorded higher sales than Day-1 for the majority of stores. Similar trends were observed for week-2 surpassing week-1 and month-2 exceeding month-1 sales, indicating a positive trajectory in sales during initial operational phases.

### Data Preparation for Modeling:

#### Null Value Handling and Data Factorization:
Before proceeding with model building, data cleaning is imperative. Null values will be addressed, and datasets will be factorized for comprehensive handling. This step ensures a refined dataset for accurate model training.

#### Data Splitting:
The merged data will be split into training and testing sets using the 70-30 ratio method. This allows for an effective evaluation of model performance on unseen data, ensuring robustness and generalization.

### Modeling Approach:

#### Forecasting Models:
The forecast models will include Prophet, SARIMA, ARIMA, XGBoosting, and ETS. These models will be implemented based on industry-leading methods. Utilizing insights from EDA, these models will be compared to identify the most promising approach. This comparison will guide the selection of the final dataset and model type for subsequent stages of analysis.

### Continuous Analysis and Refinement:

#### Iterative Progress:
As the analysis progresses, continuous refinement and revisiting of the business problem will be prioritized. Any identified glitches or discrepancies in the findings will be addressed to ensure the model's accuracy and relevance to Maverik's business objectives.

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
