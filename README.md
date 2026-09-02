# Delivery Performance and Delay Analysis Using Python

## Project Overview

This project focuses on analyzing logistics delivery performance using Python and data science techniques.

The project uses a logistics dataset containing **25,000 delivery records**. The analysis identifies delivery delays, studies factors affecting delivery performance, creates visualizations, and applies machine learning to predict delivery time.

The project was completed in four stages:

- Week 1: Strategic Planning and Data Exploration
- Week 2: Data Cleaning and Preprocessing
- Week 3: Advanced Data Analysis and Visualization
- Week 4: Predictive Modeling and Optimization

---

## Objectives

- Analyze logistics delivery performance.
- Identify factors associated with delivery delays.
- Clean and preprocess logistics data.
- Calculate important logistics KPIs.
- Create meaningful visualizations.
- Predict delivery time using machine learning.
- Evaluate predictive model performance.
- Suggest optimization strategies for logistics operations.

---

## Dataset

**Dataset:** Delivery Logistics Dataset – India Multi-Partner

The dataset contains **25,000 delivery records** and **15 columns**.

### Main Features

- Delivery Partner
- Package Type
- Vehicle Type
- Delivery Mode
- Region
- Weather Condition
- Distance
- Package Weight
- Delivery Time
- Expected Time
- Delay Status
- Delivery Status
- Delivery Rating
- Delivery Cost

---

## Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Git
- GitHub

---

# Week 1 – Strategic Planning and Data Exploration

The first stage focused on understanding the logistics problem, exploring the dataset, and identifying key performance indicators.

### Key KPIs

- Total Deliveries: **25,000**
- Delayed Records: **6,669**
- Delay Rate: **26.68%**
- On-Time Rate: **73.32%**
- Average Delivery Time: **6.25 hours**
- Average Delivery Cost: **864.94**

---

# Week 2 – Data Cleaning and Preprocessing

The second stage focused on preparing the dataset for analysis.

### Main Activities

- Data loading and inspection
- Checking missing values
- Checking data types
- Checking duplicate records
- Handling incorrectly formatted time variables
- Converting variables into usable formats
- Preparing numerical and categorical features
- Normalizing selected numerical variables

The cleaned dataset was used for the analysis and machine learning stages.

---

# Week 3 – Advanced Data Analysis and Visualization

The third stage focused on identifying patterns in delivery performance.

### Key Findings

- Overall delay rate: **26.68%**
- Stormy weather delay rate: **41.45%**
- Rainy weather delay rate: **37.35%**
- Foggy weather delay rate: **30.32%**
- Express delivery delay rate: **73.78%**
- Same-day delivery delay rate: **32.54%**
- Standard delivery delay rate: **0%**
- Two-day delivery delay rate: **0.43%**

Distance and delivery time had a correlation of approximately **0.69**.

Distance and delivery cost showed a very strong correlation of **0.99**.

### Visualizations

The project includes:

- Delivery Status Distribution
- Delay Rate by Weather
- Delay Rate by Vehicle Type
- Delay Rate by Delivery Mode
- Delay Rate by Region
- Distance vs Delivery Time
- Average Delivery Cost by Mode
- Correlation Heatmap

---

# Week 4 – Predictive Modeling and Optimization

The fourth stage applies machine learning to predict delivery time.

### Prediction Target

`delivery_time_hours`

### Features Used

- Distance
- Package Weight
- Expected Delivery Time
- Delivery Mode
- Vehicle Type
- Weather Condition
- Region
- Delivery Partner

### Models

Two regression models are used:

1. Linear Regression
2. Random Forest Regression

### Data Split

The dataset was divided into:

- **80% training data – 20,000 records**
- **20% testing data – 5,000 records**

### Evaluation Metrics

The models are evaluated using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

### Optimization Strategies

The predictive analysis is used to propose:

- Route optimization
- Weather-based scheduling
- Express delivery prioritization
- Vehicle allocation
- Dynamic delivery-time estimation
- Better resource allocation

---

# Project Structure

```text
delivery-performance-analysis/
│
├── data/
│   └── cleaned_delivery_data.csv
│
├── notebooks/
│   ├── delivery_analysis.ipynb
│   ├── week2_data_preprocessing.ipynb
│   ├── week3_analysis.ipynb
│   └── week4_predictive_modeling.ipynb
│
├── visualizations/
│   ├── delivery_status.png
│   ├── delay_by_weather.png
│   ├── delay_by_vehicle.png
│   ├── delay_by_mode.png
│   ├── distance_vs_delivery_time.png
│   ├── cost_by_delivery_mode.png
│   ├── correlation_heatmap.png
│   ├── actual_vs_predicted_delivery_time.png
│   └── feature_importance.png
│
├── README.md
├── requirements.txt
└── .gitignore
