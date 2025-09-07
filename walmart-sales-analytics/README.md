# Walmart Sales Analytics Project
**Predicting Sales & Forecasting Demand for Walmart Stores**

## Problem

Walmart operates 45 stores across the US and faces challenges due to unforeseen demand fluctuations. Sales are impacted by holidays, promotions, and economic factors such as CPI and unemployment. The main objectives of this project are:

1. Identify stores with maximum and minimum sales.
2. Determine stores with high sales variability (standard deviation) and compute the coefficient of mean to standard deviation.
3. Analyze quarterly growth rates, especially in Q3 2012.
4. Investigate holidays with higher or lower than average sales.
5. Provide monthly and semester sales insights.
6. Build prediction models to forecast demand accurately, assisting Walmart in planning and inventory management.

## Approach

**1. Data Understanding & Cleaning**

- Loaded historical sales data for 45 stores (2010–2012).
- Checked for missing values and data types.
- Created additional columns for Day, Month, and Year.

**2. Exploratory Data Analysis (EDA)**

- Identified stores with minimum and maximum total sales.
- Calculated standard deviation and coefficient of variation for each store.
- Analyzed quarterly growth rates to find high-performing stores.
- Investigated the impact of holidays (Super Bowl, Labour Day, Thanksgiving, Christmas) on sales.
- Provided monthly, semester, and yearly sales insights with visualizations.

**3. Feature Engineering & Outlier Handling**

- Detected outliers in features such as Temperature, Fuel_Price, CPI, and Unemployment.
- Filtered out extreme outliers to improve model performance.

**4. Modeling & Forecasting**

- Selected features: Store, Fuel_Price, CPI, Unemployment, Day, Month, Year.
- Target variable: Weekly_Sales.
- Split data into training and testing sets (80:20).
- Implemented Linear Regression and Random Forest Regressor.
- Evaluated models using R² score, MAE, MSE, RMSE, and visualized predicted vs actual sales.

## Tools & Libraries

- Python Libraries: pandas, numpy, matplotlib, seaborn, datetime
- Machine Learning: scikit-learn (Linear Regression, Random Forest Regressor)
- Visualization: Matplotlib, Seaborn

## Impact & Results

**Store Insights:**

- Store with maximum sales: #20
- Store with minimum sales: #33
- Store with highest standard deviation: #14
- Store with best quarterly growth in Q3 2012: #4

**Holiday Insights:**

- Sales increased during Thanksgiving, decreased during Christmas.
- Identified holidays with sales above the non-holiday mean.

**Model Performance:**

- Model	Accuracy             (%)	  MAE        RMSE
- Linear Regression        	13	    469,136	    568,758
- Random Forest Regressor	94.37	72,406	    144,281

**Business Impact:**

- Provided actionable insights for Walmart to optimize inventory and reduce stockouts.
- Forecasting model can guide promotional planning and holiday demand management.
