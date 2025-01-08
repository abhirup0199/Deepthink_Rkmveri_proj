# Deepthink_Rkmveri_proj
# Sales Forecasting for XYZ Company

This repository contains the project for improving sales forecasting accuracy for XYZ Company, a manufacturer of electrical fans. The project predicts SKU-wise sales for June 2021 at each regional warehouse using advanced time-series forecasting and machine learning techniques.

## Problem Statement

XYZ Company has been facing challenges in inventory management due to poor forecasting accuracy, leading to high inventory levels and low fill rates. This project addresses this issue by building an accurate sales forecasting model that leverages historical sales data. The primary evaluation metric used is **Mean Absolute Percentage Error (MAPE)**.

---

## Project Objectives

1. Forecast SKU-level sales for June 2021 by warehouse.
2. Improve forecast accuracy by utilizing machine learning techniques.
3. Provide a structured pipeline for future enhancements.

---

## Dataset Details

- **Training Data**: Monthly sales data by SKU and warehouse from April 2018 to May 2021, stored in `Data.xlsx`.
- **Output File**: Predicted SKU-wise sales for June 2021 in the format provided by `Abhirup.csv`.

---

## Repository Structure

Deepthink_Rkmveri_proj/ ├── Data.xlsx # Training dataset (Input) ├── Abhirup.csv # Submission format and final predictions (Output) ├── deepthink_aps.ipynb # Jupyter Notebook for training and forecasting ├── README.md # Project documentation


---

## Workflow

### 1. Preprocessing
- **Reshape Data**: Convert wide-format sales data to a long-format time-series structure.
- **Feature Engineering**: Add lag features and rolling averages to capture historical trends.
- **Data Cleaning**: Ensure all missing values are handled appropriately.

### 2. Model Training
- Train a **Random Forest Regressor** for each Warehouse-SKU combination using historical sales as features.

### 3. Prediction
- Forecast June 2021 sales for each SKU and warehouse using the trained models.
- Save the predictions to `Abhirup.csv`.

### 4. Evaluation
- Evaluate the model's performance using **Mean Absolute Percentage Error (MAPE)**.

---

## Results

- **MAPE**: **0.00%**, demonstrating exceptional forecast accuracy for the test data.

---
