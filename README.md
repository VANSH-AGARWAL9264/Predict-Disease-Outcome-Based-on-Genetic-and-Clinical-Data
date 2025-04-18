# Predict-Disease-Outcome-Based-on-Genetic-and-Clinical-Data

## Problem Statement
The objective of this project is to develop a machine learning model to predict the outcome of breast cancer—whether a tumor is malignant or benign—based on genetic and clinical data. This model aims to support early diagnosis and improve clinical decision-making in medical applications.

## Dataset Information
- Source: Breast Cancer Wisconsin (Diagnostic) Dataset
- Total Samples: 569
- Features: 30 numeric attributes (e.g., radius, texture, perimeter, area, etc.)
- Target Variable: diagnosis (M = Malignant, B = Benign)

## Technologies Used
- Python
- Google Colab
- pandas, numpy
- seaborn, matplotlib
- scikit-learn

## Methodology

1. Data Cleaning  
   - Removed non-informative columns like `id` and `Unnamed: 32`.  
   - Encoded the `diagnosis` column to binary (M = 1, B = 0).

2. Feature Scaling  
   - Applied StandardScaler to normalize all features.

3. Train-Test Split  
   - Split the data into 80% training and 20% testing sets.

4. Model Training  
   - Used Random Forest Classifier due to its high performance and reliability with structured data.

5. Model Evaluation  
   - Evaluated the model using classification report and confusion matrix.

## Results

**Classification Report:**
          precision    recall  f1-score   support

       0       0.96      1.00      0.98        72
       1       1.00      0.94      0.97        42

accuracy                           0.98       114

**Confusion Matrix:**

| Actual \ Predicted | Benign | Malignant |
|--------------------|--------|-----------|
| Benign             | 72     | 0         |
| Malignant          | 2      | 40        |

The model achieved approximately 98% accuracy with only 2 misclassifications on the test data.
