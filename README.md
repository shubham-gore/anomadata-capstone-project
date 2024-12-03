# AnomaData : Automated Anomaly Detection for Predictive Maintenance

## Problem Statement:
Many different industries need predictive maintenance solutions to reduce risks and gain actionable insights through processing data from their equipment.
Although system failure is a very general issue that can occur in any machine, predicting the failure and taking steps to prevent such failure is most important for any machine or software application.
Predictive maintenance evaluates the condition of equipment by performing online monitoring. The goal is to perform maintenance before the equipment degrades or breaks down.
This Capstone project is aimed at predicting the machine breakdown by identifying the anomalies in the data.
The data we have contains about 18000+ rows collected over few days. The column ‘y’ contains the binary labels, with 1 denoting there is an anomaly. The rest of the columns are predictors.  

## Overview
This project aims to develop a machine learning solution for predictive maintenance by identifying anomalies in machine data. Using a dataset of sensor readings, the project focuses on predicting potential equipment failures to enable proactive maintenance, minimizing downtime and improving operational efficiency.

## Features
### Exploratory Data Analysis (EDA):
- Identified trends, correlations, and missing data.
- Visualized data relationships to inform feature engineering.

### Data Preprocessing:
- Handled missing values with mean imputation.
- Scaled features using StandardScaler for uniformity.
- Addressed class imbalance using SMOTE.

### Feature Engineering:
- Features with high correlation or redundant information.

### Model Development:
- Built a robust Random Forest Classifier for anomaly detection.
- Optimized model parameters using GridSearchCV.
- Achieved high accuracy and ROC-AUC on the test set.

### Deployment Ready Pipeline:
- Saved the trained model and scaler for reuse.
- Designed a script to process and predict new data.
- Outputs predictions and probabilities for anomalies.

## Installation
1. Clone this repository:

    git clone https://github.com/shubham-gore/anomadata-capstone-project.git

2. Place the dataset (AnomaData.xlsx) in the data folder.

3. Usage

    **Train the Model**
    To train the model on the dataset, run the code in anoma-data-project.IPYNB fie in notebooks folder. This will generate the trained model (anomaly_detector_model.pkl) and scaler (scaler.pkl) in the models folder.

    **Predict on New Data**
    To predict anomalies in new data:

    **Place the new dataset in the data folder (e.g., new_data.xlsx)**
    Run the prediction code in file prediction.IPYNB in notebooks folder. Results are saved to predictions.csv in the project root. Includes Anomaly_Prediction and Anomaly_Probability columns.

License
This project is licensed under the Apache License Version 2.0. See the LICENSE file for details.
