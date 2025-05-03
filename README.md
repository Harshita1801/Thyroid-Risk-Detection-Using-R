![image](https://github.com/user-attachments/assets/7a3cd0b3-8203-4113-b969-88cefdfbdbf7)# Thyroid Risk Detection Using R

# Problem statement
Thyroid disorders occur when the thyroid gland produces abnormal levels of hormones (T3 & T4), affecting metabolism. Thyroid disorders are of 3 types compensated hypothyroid, primary hypothyroid, secondary hypothyroid. 
Challenges in Early Detection: Symptoms are non-specific (fatigue, weight changes, mood swings) and resemble other common illnesses, Late diagnosis can lead to severe complications like heart disease, infertility, or neurological issues.
Data science enables early and accurate thyroid risk detection through machine learning models that analyze medical data. It helps in predicting high-risk patients, identifying patterns in blood test reports, and automating diagnosis. AI-driven systems improve efficiency and reduce human errors, leading to faster and more reliable thyroid disorder detection.

# Features of the Dataset
Demographic Information: Age, Sex
Medical History: On Thyroxine, Antithyroid Medication, Pregnant, Thyroid Surgery, Goitre, Tumor, etc.
Thyroid Test Results:
      TSH (Thyroid-Stimulating Hormone), T3 (Triiodothyronine), TT4 (Total Thyroxine), T4U (Thyroxine Uptake), FTI (Free Thyroxine Index)
Target Variable: Class (Thyroid Condition: Negative, Compensated Hypothyroid, Primary Hypothyroid, Secondary Hypothyroid)
Dataset Statistics: Total Samples: 3,772   Total Features: 30
Class Distribution:
      Negative (Normal) → 3,481 samples
      Compensated Hypothyroid → 194 samples
      Primary Hypothyroid → 95 samples
      Secondary Hypothyroid → 2 samples

# Data Preprocessing
# Handling Missing Values
Some features (T3, TT4, T4U, FTI, TBG) have missing values, which can affect model performance.
Missing values are not removed to prevent data loss; instead, they are imputed (filled in) using KNN imputation.
# KNN Imputation
K-Nearest Neighbors (KNN) Imputation replaces missing values by using the average of the k-nearest neighbors in the dataset.
It ensures that missing values are replaced with values similar to existing patterns, improving prediction accuracy.
# Splitting into Training & Testing Sets
The dataset is split into training (80%) and testing (20%) to evaluate model performance.
Training Set → Used to train the machine learning model.
Testing Set → Used to measure how well the model generalizes to unseen data.

# Machine Learning Models Used
# Logistic Regression
A simple, interpretable model used for classification problems. Suitable for binary and multi-class classification tasks like thyroid risk detection.
# Random Forest
An ensemble learning method that combines multiple decision trees to improve accuracy and reduce overfitting. More robust and can handle complex patterns in the data.
# Justification for Chosen Models
Logistic Regression was selected for its efficiency and interpretability, making it ideal for understanding how features impact thyroid risk.
Random Forest was used because it provides higher accuracy, handles imbalanced data well, and is less prone to overfitting.

LIME (Local Interpretable Model-Agnostic Explanations) was used to provide individual prediction explanations, ensuring model transparency and interpretability.

![image](https://github.com/user-attachments/assets/13ef5c48-0c03-4c26-928e-1b2ff3dedd15)




