# Student Performance ML

## Overview

A machine learning project that predicts student GradeClass using demographic, academic, and extracurricular features.

## Dataset

The dataset contains information about students including:

- Age
- Gender
- Ethnicity
- Parental Education
- Study Time Weekly
- Absences
- Tutoring
- Parental Support
- Extracurricular Activities
- Sports
- Music
- Volunteering

`StudentID` was removed because it is only an identifier.

`GPA` was also excluded from the features because GradeClass is closely related to GPA, which could cause data leakage.

## Machine Learning Models

Three models were tested:

1. Random Forest
2. Logistic Regression
3. Gradient Boosting

## Results

| Model | Accuracy | Macro F1 |
|---|---:|---:|
| Random Forest | 71.40% | 0.54 |
| Random Forest (Balanced) | 67.01% | 0.51 |
| Logistic Regression | **72.65%** | **0.54** |
| Gradient Boosting | 68.48% | 0.53 |

### Best Model

Logistic Regression achieved the highest test accuracy of **72.65%**.

However, the dataset is imbalanced, with GradeClass 4 containing significantly more students than the other classes. Therefore, accuracy alone should not be used to judge model performance.

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Jupyter Notebook

## Project Workflow

```text
Dataset
   ↓
Data Exploration
   ↓
Data Preprocessing
   ↓
Train/Test Split
   ↓
Model Training
   ↓
Predictions
   ↓
Model Evaluation
