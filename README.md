# Canada Household Expenditure Analysis & Forecasting

## Project Overview

This project analyzes **household spending patterns across Canada** using publicly available data from Statistics Canada. The goal is to uncover key economic trends, identify major expenditure categories, and forecast future spending using time series modeling.

The analysis combines **data cleaning, exploratory data analysis (EDA), and forecasting techniques** to deliver insights into how household expenditures evolve over time across provinces.

---

## Objectives

* Understand the structure and quality of economic data
* Identify the **highest and lowest household expenditure categories**
* Analyze **trends in spending over time (2010–2021)**
* Compare **provincial expenditure patterns**
* Forecast **future expenditure (2022–2024)** using time series models

---

## Tools & Technologies

* **R** (dplyr, ggplot2, zoo, forecast, patchwork)
* **Excel** (data viewing and validation)
* **Time Series Modeling** (ARIMA)

---

## Data Description

The dataset contains:

* Household expenditure data across Canadian provinces
* Income quintile segmentation
* Multiple expenditure categories (e.g., shelter, food, transport)
* Annual data from **2010 to 2021**

---

## Data Cleaning & Preparation

* Removed irrelevant columns (metadata and identifiers)
* Standardized column names using snake_case
* Filtered out categories with missing values
* Removed duplicate records
* Focused analysis on **“All quintiles”** to represent overall population behavior
* Converted variables into appropriate data types (factors)

---

## Exploratory Data Analysis (EDA)

### Key Findings:

* **Shelter** is the **highest expenditure category** across Canada
* Annual expenditure on shelter shows a **consistent upward trend**, peaking around **2021 (~$240,000)**
* Significant variation exists across provinces in total spending patterns

### Visualizations:

* Line plots showing **yearly expenditure trends**
* Category-wise expenditure summaries
* Province-level comparison charts

---

## Time Series Forecasting

### Model Used:

* **ARIMA (AutoRegressive Integrated Moving Average)**

### Approach:

* Filtered dataset for **total expenditure per province**
* Converted data into time series format using `zoo`
* Applied `auto.arima()` for model fitting
* Forecasted **3 future years (2022–2024)**

---

## Forecast Interpretation

Each forecast visualization includes:

* **Black Line** → Actual historical data
* **Red Dashed Line** → Model fitted values
* **Blue Dashed Line** → Forecasted values
* **Blue Shaded Area** → 80% confidence interval

### Insights:

* **Ontario** shows a **narrow confidence interval**, indicating more reliable forecasts
* **Alberta** exhibits **higher uncertainty**, reflected by a wider interval
* Provinces display **different expenditure behaviors**:

  * Some show steady growth
  * Others demonstrate volatility or fluctuations

---

## Provincial Trends

* **Alberta**:

  * Highest expenditure overall
  * Notable drop observed in **2019**

* **Prince Edward Island**:

  * Lowest initial expenditure
  * Gradual increase after **2016**

* Overall:

  * Clear **regional variation in spending behavior**
  * Economic trends differ significantly across provinces

---

## Key Takeaways

* Household spending in Canada is **dominated by shelter costs**
* Expenditure trends are generally **increasing over time**
* **Forecasting reveals varying levels of economic stability** across provinces
* Time series modeling can effectively capture and project **macro-level economic patterns**

---

## Future Improvements

* Incorporate **external economic indicators** (inflation, income levels)
* Compare **ARIMA with ETS or Prophet models**
* Perform **quintile-level analysis** instead of aggregated data
* Build an **interactive dashboard (Power BI / Tableau)**

---

## Project Structure

```
├── data/
├── scripts/
│   └── analysis.R
├── outputs/
│   ├── plots/
│   └── forecasts/
├── README.md
```

---

## Author

**Shuvam Jaggi**
Business Analytics | Data Analysis | Forecasting | BI

---

## Final Note

This project demonstrates the ability to:

* Work with **real-world government datasets**
* Perform **end-to-end data analysis**
* Apply **time series forecasting techniques**
* Translate data into **meaningful economic insights**

---
