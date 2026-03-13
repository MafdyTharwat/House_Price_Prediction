# House Prices Prediction (End-to-End ML Pipeline)

## Project Overview
This project demonstrates a complete Machine Learning workflow, starting from **synthetic data generation** with realistic noise and outliers, moving through **exploratory data analysis (EDA)**, and ending with a **predictive model** for house prices.

The goal was to simulate a real-world scenario where data is "messy" and requires significant cleaning before it can be used for modeling.

## Tech Stack
* **Language:** Python
* **Libraries:** Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn

## Key Features & Workflow

### 1. Data Generation & "Messiness" Injection
* Generated a dataset of 2,825 houses with features like `LotArea`, `TotalRooms`, `YearBuilt`, and `Neighborhood`.
* Injected **Outliers** (e.g., a house with 1,000,000 sqm area, a house priced at $50).
* Added **Missing Values** (NaNs) and **Categorical Inconsistencies** (e.g., 'Yes', 'yes', 'Y').

### 2. Exploratory Data Analysis (EDA)
* Used **Correlation Heatmaps** to identify relationships between features.
* Visualized the impact of outliers using **Scatter Plots**, observing how a single outlier can skew the entire model's perception of data.

### 3. Data Preprocessing
* **Missing Value Imputation:** Filled NaNs using median values.
* **Outlier Removal:** Strategically removed extreme values (e.g., Area > 100k, Price < 1k).
* **Categorical Encoding:** Applied One-Hot Encoding for neighborhoods and property types.

### 4. Machine Learning Modeling
* Implemented **Linear Regression** as a baseline model.
* Achieved an **R-squared ($R^2$) score of ~0.90** after proper data cleaning.

## 📊 Visualizations
> **Note:** Here I observed how removing the $1M$ area outlier transformed the correlation from 0.01 to a strong positive relationship.
