# GEMAI – Jewellery Sales Demand Forecasting

## Project Overview

GEMAI – Jewellery Sales Demand Forecasting is a data analytics and time-series forecasting project that analyzes historical jewellery sales data to understand sales patterns and estimate future product demand.

The project focuses on transforming historical transaction data into meaningful business insights and a forward-looking demand forecast that can support inventory and business planning.

---

## Business Problem

Jewellery businesses need to understand how much product customers are likely to purchase in the future.

If demand is underestimated, businesses may not have enough stock to meet customer requirements. If demand is overestimated, businesses may hold excess inventory and tie up resources.

Relying only on historical reports or assumptions makes it difficult to anticipate future demand.

The key business problem addressed in this project is:

> **How can historical jewellery sales data be analyzed to understand demand patterns and forecast future monthly demand?**

---

## Why This Project?

I selected this project because demand forecasting is a practical business analytics problem where historical data can be used to support future planning.

Instead of only analyzing what happened in previous sales periods, this project focuses on using historical patterns to estimate what may happen in future periods.

This helped me apply Data Analyst skills to a business problem involving:

- Data cleaning
- Exploratory data analysis
- Time-series analysis
- Feature engineering
- Demand forecasting
- Model evaluation
- Data visualization
- Business interpretation

---

## Who Can Benefit From This Analysis?

The analysis can be useful for business teams involved in:

- Inventory planning
- Sales planning
- Procurement
- Operations
- Product planning
- Business management

For example, a business manager could use demand estimates as one input when deciding how much inventory may be required for future periods.

The forecast is intended to support decision-making, not replace business judgment.

---

## Why Is Demand Forecasting Important?

Demand forecasting provides a forward-looking view of expected product demand.

For product-based businesses, understanding future demand can help with inventory planning, resource allocation and operational planning. Forecasting can also help businesses prepare for changes in demand rather than responding only after the change occurs. :contentReference[oaicite:1]{index=1}

For jewellery businesses, this can be particularly useful when demand varies across different time periods or product categories.

The purpose of this project is therefore not simply to create a forecast, but to demonstrate how a Data Analyst can transform historical data into information that can support business planning.

---

# Project Objective

The main objectives of this project are to:

- Analyze historical jewellery sales data
- Understand sales and demand patterns
- Identify differences across jewellery categories
- Prepare the data for time-series analysis
- Aggregate sales quantity at a monthly level
- Develop a demand forecasting model using Prophet
- Forecast future monthly demand up to 2026
- Evaluate the forecasting results using statistical metrics
- Estimate potential revenue based on forecasted demand
- Translate analytical results into business-oriented insights

---

# Dataset

**Source:** Kaggle Jewellery Sales Dataset

The dataset contains historical jewellery transaction information.

### Dataset Size

- **80,626 records**
- Transaction-level historical sales data

### Main Features

| Feature | Description |
|---|---|
| `Datetime` | Date and time of the transaction |
| `Category` | Jewellery product category |
| `Price` | Product price |
| `Quantity` | Quantity sold |

---

# Problem → Analysis → Solution

### Problem

Historical sales data contains useful information, but raw transaction records do not directly show future demand.

### Analysis

I analyzed the historical data to identify:

- Sales trends
- Monthly demand patterns
- Category-level differences
- Seasonal patterns
- Changes in sales quantity over time

### Solution

I developed a time-series forecasting workflow using **Prophet** to estimate future monthly jewellery demand.

The forecast can then be used as an analytical input for future inventory and business planning.

---

# What I Did

As part of this project, I worked on the complete analytics workflow.

### 1. Data Understanding

I first examined the dataset structure, columns, data types and available sales information.

### 2. Data Cleaning

I prepared the dataset for analysis by:

- Converting the `Datetime` column into the correct datetime format
- Checking missing values
- Removing missing values in important fields such as Category and Price
- Reviewing the quality and consistency of the data

### 3. Feature Engineering

I created additional time-related features from the transaction date:

- Year
- Month
- Day
- Weekday
- Quarter
- Season

These features helped analyze sales patterns across different time periods.

### 4. Exploratory Data Analysis

I analyzed the historical sales data to understand:

- Monthly sales trends
- Product category performance
- Demand patterns
- Seasonal behavior
- Changes in quantity sold over time

Visualizations were used to make these patterns easier to understand.

### 5. Monthly Demand Aggregation

Since individual transactions are not directly suitable for the final forecasting objective, I aggregated the sales quantity at a monthly level.

This created a time series representing monthly jewellery demand.

### 6. Time-Series Forecasting

I used **Prophet** to model the historical monthly demand and generate future forecasts.

The forecasting workflow was designed to estimate future monthly demand through 2026.

### 7. Forecast Evaluation

I evaluated the forecasting results using:

- MAE — Mean Absolute Error
- RMSE — Root Mean Square Error
- MAPE — Mean Absolute Percentage Error
- Forecast accuracy calculation

These metrics were used to understand how closely the forecast represented the available historical data.

### 8. Business Interpretation

Finally, I interpreted the analysis from a business perspective rather than looking only at model output.

The focus was on understanding:

- Which categories show stronger demand
- How demand changes over time
- What future demand may look like
- How forecast information could support inventory planning
- How predicted quantity can be used for revenue estimation

---

# Forecasting Approach

The forecasting process uses **Prophet**, a time-series forecasting model.

The historical transaction data was first converted into a monthly demand time series.

The forecasting process then:

1. Prepared historical monthly demand
2. Identified the time-based structure of the data
3. Trained the forecasting model
4. Generated future monthly predictions
5. Evaluated the forecast
6. Interpreted the results for business use

The purpose of the model is to provide an estimate of future demand based on historical patterns.

---

# Technologies Used

### Programming

- Python

### Data Analysis

- Pandas
- NumPy

### Data Visualization

- Matplotlib

### Forecasting

- Prophet

### Model Evaluation

- Scikit-learn

### Development Environment

- Jupyter Notebook

---

# Key Results

The analysis helped identify:

- Historical jewellery sales and demand patterns
- Differences in demand across product categories
- Monthly demand trends
- Seasonal patterns in the historical data
- Future monthly demand estimates through 2026
- Forecast evaluation metrics
- Potential revenue estimates based on predicted quantity

The project demonstrates how historical transaction data can be converted into a forward-looking analytical output.

---

# Real-World Business Value

This project shows how historical jewellery sales data can be used to forecast future demand and support business planning. The insights can help businesses plan inventory, prepare for expected demand, and make more informed operational decisions.

---

# What I Learned

Through this project, I developed experience in:

- Working with transaction-level datasets
- Cleaning and preparing real-world-style data
- Performing exploratory data analysis
- Creating time-based features
- Working with time-series data
- Aggregating transaction data into meaningful business metrics
- Building a forecasting workflow using Prophet
- Evaluating forecasting performance
- Creating analytical visualizations
- Interpreting model outputs
- Connecting technical analysis with business problems

---

# Project Challenges

Some important challenges involved:

- Preparing raw transaction data for analysis
- Handling date and time information correctly
- Converting transaction-level data into a suitable time series
- Understanding seasonal and monthly demand patterns
- Selecting appropriate evaluation metrics
- Interpreting forecasts from a business perspective

These challenges helped me understand that successful data analysis requires both technical skills and business understanding.

---

# Limitations

This project is based primarily on historical sales data.

The forecast does not represent every factor that can affect future jewellery demand, such as:

- Marketing campaigns
- Competitor activity
- Economic conditions
- Major festivals or events
- Changes in customer preferences
- Pricing changes
- External market conditions

Therefore, the forecast should be treated as an analytical estimate rather than a guaranteed future outcome.

---

# Future Improvements

The project can be extended by:

- Incorporating additional external factors
- Including promotional and pricing information
- Building category-level forecasting models
- Comparing Prophet with other forecasting approaches
- Creating an interactive Power BI dashboard
- Developing a Streamlit application
- Adding automated forecast updates
- Connecting the model to regularly updated sales data

---

# Project Outcome

This project demonstrates my ability to work through a complete Data Analytics and forecasting problem:

**Understand the problem → Prepare the data → Analyze patterns → Build a forecasting solution → Evaluate the results → Interpret the findings → Connect the results to a real business use case.**

The main objective was to move beyond simply analyzing historical sales and demonstrate how data can be used to create a forward-looking view of product demand.

---

# Author

**Anusuya S**

Data Analyst

### Connect With Me

- **Portfolio:** [https://anusuya0805.github.io/](https://anusuya0805.github.io/)
- **LinkedIn:** [https://www.linkedin.com/in/anusuya-s-1aa138295](https://www.linkedin.com/in/anusuya-s-1aa138295)
- **GitHub:** https://github.com/anusuya0805

---

## Project Focus

**Data Analytics | Time-Series Analysis | Demand Forecasting | Business Insights | Inventory Planning Support**
