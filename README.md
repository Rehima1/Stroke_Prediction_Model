# Stroke Prediction using Machine Learning 🧠

## Project Overview

This project aims to predict the likelihood of a stroke using machine learning models. It uses a dataset containing various health-related features to train and evaluate different classification algorithms.

## Dataset

The project utilizes the "Healthcare Dataset Stroke Data" dataset, which can be found [here](https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset/data). The dataset includes information about patient demographics, medical history, and lifestyle factors.

## Features

The following features are used for prediction:

- **gender:** Gender of the patient
- **age:** Age of the patient
- **hypertension:** Whether the patient has hypertension (0 or 1)
- **heart_disease:** Whether the patient has heart disease (0 or 1)
- **ever_married:** Whether the patient has ever been married (Yes or No)
- **work_type:** Type of work the patient does (children, Govt_jov, Never_worked, Private, or Self-employed)
- **Residence_type:** Whether the patient lives in a rural or urban area (Rural or Urban)
- **avg_glucose_level:** Average glucose level in the blood
- **bmi:** Body mass index
- **smoking_status:** Smoking status of the patient (formerly smoked, never smoked, smokes, or Unknown)

## Target Variable

The target variable is **stroke**, which indicates whether the patient had a stroke (0 or 1).

## Methodology

1. **Data Loading and Preprocessing:** The dataset is loaded using pandas, and missing values are handled (e.g., filling missing BMI values with the mean). Categorical features are encoded using LabelEncoder.
2. **Exploratory Data Analysis:** Data is explored using visualizations like countplots, heatmaps, and pairplots to understand the distribution and relationships between features.
3. **Data Splitting:** The dataset is split into training and testing 
4. **Data Balancing:** SMOTE (Synthetic Minority Over-sampling Technique) is used to address class imbalance in the target variable.
5. **Model Training and Evaluation:** Multiple models are trained, including Random Forest, Logistic Regression, and Support Vector Machine (SVM). Their performance is evaluated using metrics like accuracy, F1 score, AUC-ROC score.
6. **Model Comparison:** The models are compared based on their performance metrics to identify the best-performing model.
7. **Feature Importance Analysis:** The importance of features in the Random Forest model is analyzed.

## Results
Random Forest achieved the highest performance with an F1 score of 94% and an AUC-ROC score of 98%
Logistic Regression and SVM provided reasonable performance but were outperformed by the Random Forest model.

![image](https://github.com/user-attachments/assets/3115647d-2d74-4356-9fc2-712648c58d26)

## Feature Importance

![image](https://github.com/user-attachments/assets/9903316a-7650-4424-8ada-159d03b7dbac)

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, feel free to open an issue or submit a pull request.
