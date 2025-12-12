# FUTURE_ML_01
Project Overview
================
This project represents an end-to-end predictive analytics solution that aims to forecast sales in the retail industry for a period of 24 months. This project has used machine learning in Business Intelligence to convert raw relational data into valuable business insights.

Contrary to a file analysis, in this project, it was necessary to combine several datasets (Sales Transactions + Store Metadata) in order to examine performance in various store types using Rossmann Store Sales data.
 
**Business Problem**

Retail managers are having trouble anticipating how much product would be needed in the future due to seasonality and holiday sales. The aim of this project was to:
Revenue Forecast: Project revenue patterns for a period of 2 years.

*Manage Risk*: Use Best Case vs. Worst Case estimates for confidence intervals.

A) An analysis of seasonality in a product.

**Tech Stack**
*Python*: Core programming language.
*Pandas*: Advanced data manipulation, joining of relation tables (train data + stores data), grouping.
*Facebook Prophet*: Handling seasonality, including yearly and weekly seasonality, as well as holidays.
*Jupyter Notebook*: Used for exploratory data analysis as well as developing models.
*Power BI*: To create the interactive dashboard for displaying the final forecast.

**Project Workflow**

1. Data Engineering with Python and Pandas

Ingestion  Loads raw transaction data (~1M rows) and stores metadata.

*Cleaning*: Managed missing data, edited date formats, and removed data for closed store days.

*Aggregation*: Aggregated large transaction data by Store Type (a, b, c, d) to support scalable forecasting.


2. **Machine Learning (Facebook Prophet)**

*Modeling*:
        A separate Prophet model has been trained for different Store Types.
        
*Feature Engineering*:
        Introduced US Holidays as a feature that takes into account the sudden increase in sales that occurs due to Black Friday and Christmas.

*Forecasting*: 
         Created a 24-month ahead forecast with 95% Confidence Intervals for y values, namely yhat

3. **Visualization (Power BI)**

*Data Modeling*:
          Imported Rossmann_Store_Forecast, a Python
          
*Trend Analysis*: 
          Comparison of line graphs of Historical Actuals and Future Forecasts.

**Uncertainty Modeling**
Tool tips of Upper and Lower bounds for Uncertainty Modeling. "Interactivity: Slicers to filter forecasts by specific Store Type." KPI Tracking: Cards displaying total projected revenue. Key Insights "Seasonality: There is a huge increase in revenue for every type of store in November and December, proving that there needs to be an increase in inventory in Q4." Store *Variability*:
 Store Type B has different rates of growth than Store Type A, which indicates a different approach to marketing for different types of stores. Growth Trajectory: There would be a constant yearly increase, with a "Best Case" for Aggressive goals.
 <img width="2225" height="1260" alt="image" src="https://github.com/user-attachments/assets/54452237-a944-4d8d-8e1f-c54ce2583198" />
