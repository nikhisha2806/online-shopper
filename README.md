# 🛒 Online Shoppers Intention Prediction

## 📌 Project Overview

This project focuses on analyzing online shopping session data and predicting whether a visitor will generate revenue from an online shopping session.

The project uses machine learning classification algorithms to identify patterns in customer browsing behavior and predict the **Revenue** outcome.

## 📊 Dataset

The project uses the **Online Shoppers Intention Dataset**.

- Number of Rows: **12,330**
- Number of Columns: **18**
- Target Variable: **Revenue**
- Problem Type: **Binary Classification**

The dataset contains information about visitors' browsing activities, page visits, duration, traffic information, and other session-related details.

### 📋 Main Features

- Administrative
- Administrative Duration
- Informational
- Informational Duration
- Product Related
- Product Related Duration
- Bounce Rates
- Exit Rates
- Page Values
- Special Day
- Month
- Operating Systems
- Browser
- Region
- Traffic Type
- Visitor Type
- Weekend
- Revenue

## 🎯 Objective

The main objective of this project is to develop a machine learning model that can predict whether an online shopping session will result in revenue.

The project also aims to compare different classification algorithms and identify their performance using suitable evaluation metrics.

## 🛠️ Technologies Used

- **Python**
- **NumPy**
- **Pandas**
- **Matplotlib**
- **Seaborn**
- **Scikit-learn**
- **Imbalanced-learn**

## 🔄 Project Workflow

The project follows these major steps:

1. Data Loading
2. Data Exploration
3. Exploratory Data Analysis
4. Outlier Treatment
5. Categorical Encoding
6. Handling Class Imbalance
7. Feature Selection
8. Feature Transformation
9. Feature Scaling
10. Train-Test Split
11. Model Training
12. Model Evaluation
13. Model Comparison

## 📥 Data Loading

The dataset is loaded using the Pandas library.

The dataset used in this project is:

`online_shoppers_intention.csv`

After loading the dataset, its shape, columns, data types, and other basic information are examined.

## 🔍 Data Exploration

Data exploration is performed to understand the structure and characteristics of the dataset.

The following operations are performed:

- Checking the number of rows and columns
- Viewing the dataset
- Checking column names
- Checking data types
- Identifying missing values
- Examining statistical information
- Understanding the target variable

## 📈 Exploratory Data Analysis

Exploratory Data Analysis (EDA) is performed to understand relationships and patterns in the data.

Visualizations are used to analyze:

- Numerical variables
- Categorical variables
- Revenue distribution
- Customer browsing behavior
- Relationships between important features

Matplotlib and Seaborn are used for data visualization.

## 🚨 Outlier Treatment

Outliers are identified and treated using an **IQR-based approach**.

The Interquartile Range (IQR) method is used to identify values that fall outside the expected range.

This step helps reduce the effect of extreme values on the machine learning models.

## 🔤 Categorical Encoding

Categorical variables need to be converted into numerical form before applying machine learning algorithms.

Encoding techniques are applied to categorical features so that they can be processed by machine learning models.

The project uses encoding methods including:

- Label Encoding
- One-Hot Encoding / Get Dummies

## ⚖️ Handling Class Imbalance

The target variable may contain an unequal number of samples between the classes.

To handle class imbalance, the project uses **SMOTE (Synthetic Minority Over-sampling Technique)**.

SMOTE generates synthetic samples for the minority class and helps create a more balanced training dataset.

## 🎯 Feature Selection

Feature selection is performed to identify the most important features for prediction.

The project uses:

**SelectKBest with f_classif**

The **10 best features** are selected for building the machine learning models.

Feature selection helps reduce unnecessary features and can improve model performance.

## 📐 Feature Transformation and Scaling

Numerical features are transformed and scaled before model training.

The project explores **Yeo-Johnson Power Transformation** for numerical variables.

After transformation, **StandardScaler** is used to standardize the features.

Scaling ensures that numerical features are represented on a comparable scale.

## ✂️ Train-Test Split

The dataset is divided into training and testing sets.

- **Training data: 80%**
- **Testing data: 20%**
- **Random State: 40**

The training data is used to train the machine learning models, while the testing data is used to evaluate their performance.

## 🤖 Machine Learning Models

The project trains and compares multiple classification algorithms.

### 1. Logistic Regression

Logistic Regression is a classification algorithm used to predict the probability of a binary outcome.

### 2. Decision Tree Classifier

Decision Tree Classifier uses a tree-like structure to make classification decisions based on feature values.

### 3. Random Forest Classifier

Random Forest combines multiple decision trees to produce a stronger classification model.

### 4. AdaBoost Classifier

AdaBoost is an ensemble learning algorithm that combines multiple weak learners to improve classification performance.

### 5. Gradient Boosting Classifier

Gradient Boosting builds models sequentially and improves the prediction by focusing on errors made by previous models.

## 📏 Model Evaluation

The trained models are evaluated using different classification metrics.

The project uses:

- **Accuracy**
- **Precision**
- **Recall**
- **F1 Score**

These metrics help compare the performance of the different machine learning models.

## 🏆 Model Comparison

The performance of the classification models is compared using the evaluation metrics.

The comparison helps determine which model performs better for predicting whether an online shopping session will generate revenue.

The final model should be selected based on the evaluation results obtained from the notebook.

## 💡 Conclusion

This project demonstrates how machine learning can be applied to online shopping data to predict customer purchasing behavior.

The project includes data exploration, visualization, preprocessing, outlier treatment, categorical encoding, class imbalance handling, feature selection, transformation, scaling, model training, and evaluation.

Multiple classification algorithms are compared to understand their performance in predicting the **Revenue** variable.

## 📁 Project Structure

```text
Online-Shoppers-Intention-Prediction/
│
├── online_shoppers_intention.csv
├── online_shoppers_intention.ipynb
└── README.md
