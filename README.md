# Heart Attack Prediction Project

This project focuses on predicting heart attack likelihood based on various medical parameters using machine learning models.

## Overview

The dataset consists of various features that are indicators of heart disease. Using these features, we implement and compare two machine learning models:
- **Support Vector Machine (SVM)**
- **Random Forest Classifier**

We use these models to classify patients into two categories:
- **1**: Higher chance of a heart attack
- **0**: Lower chance of a heart attack

## Dataset

The dataset used in this project contains 303 records with 14 attributes. The target variable is `output`, which indicates the likelihood of a heart attack.

### Features:
- `age`: Age of the patient
- `sex`: Gender of the patient (1 = Male, 0 = Female)
- `cp`: Chest pain type (0-3)
- `trtbps`: Resting blood pressure (in mm Hg)
- `chol`: Cholesterol level (in mg/dl)
- `fbs`: Fasting blood sugar (>120 mg/dl) (1 = True, 0 = False)
- `restecg`: Resting electrocardiographic results (values 0, 1, 2)
- `thalachh`: Maximum heart rate achieved
- `exng`: Exercise induced angina (1 = Yes, 0 = No)
- `oldpeak`: ST depression induced by exercise relative to rest
- `slp`: Slope of the peak exercise ST segment
- `caa`: Number of major vessels colored by fluoroscopy (0-4)
- `thall`: Thalassemia (0-3)
- `output`: Target variable (0 = Less chance, 1 = More chance)

## Models Used

### 1. Support Vector Machine (SVM)
- **Kernel**: Linear
- **Accuracy**: 86.88%

### 2. Random Forest Classifier
- **Random State**: 3
- **Accuracy**: 90.16%

## Data Preprocessing

- Checked for missing values.
- Performed normalization using the `Normalizer` from `sklearn.preprocessing` to standardize the feature values.
- Split the dataset into training (80%) and testing (20%) sets using `train_test_split`.


