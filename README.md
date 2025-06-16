# LR_Delivery_Time_Estimation (Porter Food Delivery)

This repository contains a complete data science pipeline for predicting food delivery times using Linear Regression. The project explores operational, temporal, and order-based features to build an accurate, interpretable model aimed at enhancing customer satisfaction and optimizing fleet management for Porter.

---

##  Project Overview

This notebook-based project is built on real-world food delivery data. It follows a structured machine learning workflow that includes:

* Data loading and cleaning
* Feature engineering (e.g., time features, one-hot encoding)
* Exploratory Data Analysis (EDA)
* Outlier handling and normalization
* Linear regression modeling and performance evaluation
* Business-focused insights and recommendations

The objective is to predict `time_taken` (in minutes) for food delivery based on various features like order size, distance, number of dashers, and time of day.

---

##  Key Features

### 1. End-to-End Workflow

A full ML pipeline is implemented using Python and libraries such as `pandas`, `matplotlib`, `seaborn`, and `sklearn`.

### 2. Feature Engineering

Created features like:

* `hour`, `day_of_week`, `isWeekend`
* Dummy variables for `store_primary_category` and `order_protocol`
* Target variable: `time_taken` from order timestamps

### 3. Exploratory Data Analysis (EDA)

* Distribution plots, boxplots, scatter plots
* Correlation heatmap
* Insights on peak hours, order complexity, and delivery patterns

### 4. Outlier Detection & Treatment

* Used IQR-based clipping to retain most data while handling extreme values

### 5. Predictive Modeling

* Trained a Linear Regression model with R² ≈ 0.86
* Performed Recursive Feature Elimination (RFE) to identify top predictors
* Conducted residual analysis to validate model assumptions

### 6. Business Recommendations

* Emphasize order size in ETA estimates
* Dynamically allocate delivery partners during peak hours
* Use complexity-based pricing for better revenue planning
* Improve restaurant operations for large orders

---

##  Visualizations Included

* Histograms & KDE plots for numeric features
* Boxplots for outlier detection
* Scatter plots for feature-target relationships
* Correlation matrix heatmap
* Residual diagnostics (Q-Q plots, residual vs. predicted)
* Feature importance bar charts

---

##  Assumptions

* Distance and price features are on natural scales (e.g., kilometers, INR).
* Timestamp conversions are in the dataset's original timezone.
* No rows were deleted—extreme values were clipped, not removed.

---

##  Files in This Repository

* `LR_Delivery_Time_Estimation_Starter_Manish_Atwal.ipynb` – Jupyter Notebook with full implementation
* `LR_Delivery_Time_Estimation_Starter_Manish_Atwal.pdf` – Final report with executive summary, EDA, and business insights

---

##  Reference

This project is inspired by real-world delivery optimization use cases and follows standard machine learning and EDA methodologies.

---

##  Author

**Manish Atwal**
