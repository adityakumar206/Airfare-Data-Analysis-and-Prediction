# Airfare Data Analysis and Prediction  

## Project Overview  
This project analyzes airfare data, performs statistical analysis, and creates static visualizations using Matplotlib. Additionally, an XGBoost-based machine learning model is developed to predict airfare prices.  

## Dataset  
- **Source:** Consumer Airfare Report ([data.gov](https://catalog.data.gov/dataset/consumer-airfare-report-table-5-detailed-fare-information-for-highest-and-lowest-fare-mark))  
- **Machine Learning Model:** XGBoost Regressor  

## Data Overview  
- **Total Entries:** 14,881  
- **Key Attributes:**  
  - Market Fare (mkt_fare)  
  - Year and Quarter  
  - Passenger Share (carpaxshare)  
  - Average Fare (caravgfare)  
  - Fare Distribution (fareinc_min, fareinc_max)  

## Data Processing  
- Removed missing values in `Geocoded_City1` and `Geocoded_City2`  
- Encoded categorical variables numerically  
- Normalized dataset for analysis  

## Exploratory Data Analysis (EDA)  
- **Histogram:** Right-skewed distribution of market fares  
- **Line Plot:** Fluctuating average fare trends over time  
- **Scatter Plot:** Weak positive correlation between passenger share and average fare  
- **Bar Chart:** Competition lowers fares in high-traffic cities  
- **Box Plot:** Identifies fare outliers  

## Statistical Findings  
- **Mean Market Fare:** $191.42  
- **Median Market Fare:** $225.69  
- **Standard Deviation:** $87.37  
- **95% Confidence Interval:** ($190.01, $192.82)  
- **Correlation (Passenger Share vs. Average Fare):** 0.033 (Weak correlation)  

## Machine Learning Model: XGBoost Regressor  
- **Mean Absolute Error (MAE):** $9.77  
- **Mean Squared Error (MSE):** $287.01  
- **Root Mean Squared Error (RMSE):** $16.94  
- **R-squared Score (R²):** 0.9628 (96.28% accuracy)  

## Key Insights  
- Market fares fluctuate over time and location.  
- Passenger share weakly affects pricing, suggesting competition influences fares.  
- The XGBoost model predicts fares with high accuracy (96.28% R²).  

## Recommendations  
- Airlines should adjust pricing based on demand trends.  
- Incorporating additional factors (e.g., fuel prices, seasonality) could enhance predictions.  
- Future work could use time-series forecasting (e.g., ARIMA) for long-term fare trends.  

