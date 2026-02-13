GEMAI – Jewellery Sales Demand Forecasting

Project Overview
GEMAI is a data analytics and time series forecasting project designed to predict future jewellery sales demand using historical transaction data. The objective of this project is to analyze past sales patterns and forecast demand up to the year 2026 using Prophet.

Dataset
Source: Kaggle Jewellery Sales Dataset

Features Used:
- Datetime
- Category
- Price
- Quantity

Data Preprocessing
- Converted Datetime column into proper datetime format
- Extracted Year, Month, Day, Weekday, and Quarter
- Created a new Season column (Winter, Spring, Summer, Autumn)
- Removed missing values in Category and Price
- Aggregated monthly sales quantity for forecasting

Technologies Used
- Python
- Pandas
- Matplotlib
- Prophet
- Scikit-learn

Project Workflow
1. Data Cleaning and Feature Engineering
2. Exploratory Data Analysis
3. Monthly Sales Aggregation
4. Time Series Forecasting using Prophet
5. Future Forecast until 2026
6. Revenue Estimation based on predicted quantity
7. Cross-validation and Model Performance Evaluation

Model Evaluation Metrics
- MAE (Mean Absolute Error)
- RMSE (Root Mean Square Error)
- MAPE (Mean Absolute Percentage Error)
- Forecast Accuracy Calculation

Results
- Identified top selling jewellery categories
- Forecasted monthly demand until 2026
- Estimated total revenue for 2026
- Calculated forecast accuracy using cross-validation

Future Improvements
- Deploy as an interactive dashboard
- Integrate real-time sales data
- Build a web application using Streamlit
- Implement advanced pricing prediction models

Author
Anusuya S
Aspiring Data Analyst

