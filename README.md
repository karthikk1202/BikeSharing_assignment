# Bike Sharing Demand Prediction  

This project applies linear regression to predict daily demand for shared bikes based on various environmental and seasonal factors. The goal is to understand which features influence bike rentals the most and to build a reliable regression model for demand forecasting.  

## Problem Statement  
The dataset contains information about daily bike rentals along with weather, seasonal, and calendar details. The objective is to:  
- Identify key drivers of bike rental demand  
- Build and validate a linear regression model  
- Provide business recommendations for improving operations and demand planning  

## Approach  
1. Data Cleaning and Preparation  
   - Handled categorical variables by creating dummy variables (avoiding dummy variable trap using drop_first).  
   - Checked for missing values and outliers.  
   - Scaled numerical features where required.  

2. Exploratory Data Analysis (EDA)  
   - Analyzed categorical variables such as season, weather, month, holiday, and weekday.  
   - Found that season and weather have the strongest effect on demand.  
   - Verified correlations using pair plots (temperature showed the highest correlation with demand).  

3. Model Building  
   - Built multiple linear regression models.  
   - Checked for multicollinearity using Variance Inflation Factor (VIF).  
   - Validated assumptions of linear regression: linearity, multicollinearity, homoscedasticity, normality of residuals, independence of errors.  

4. Model Evaluation  
   - Compared models on training and test data.  
   - Identified top predictors of demand.  

## Key Insights  
- Temperature is the strongest predictor of bike demand.  
- Summer and Fall seasons show significantly higher rentals compared to Winter.  
- Clear weather days attract more rentals, while rain/snow conditions reduce demand.  
- Holidays have minimal impact as demand is mainly driven by commuters.  

## Final Model & Top Predictors  
- Temperature (temp): higher temperatures → more rentals (up to a point).  
- Season (summer): seasonality plays a major role in demand.  
- Weather situation (clear days): boosts bike usage significantly.  

## Tech Stack  
- Python (Pandas, NumPy, Matplotlib, Seaborn, Statsmodels, Sklearn)  
- Jupyter Notebook for analysis and modeling  
- Linear Regression for prediction and feature analysis  

## Applications  
- Forecast daily demand to optimize bike availability.  
- Support decision-making for fleet allocation and pricing.  
- Guide marketing strategies by focusing on favorable weather/season periods.  
