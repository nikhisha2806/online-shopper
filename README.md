Online Shoppers Intention Prediction
Project Overview
This project analyzes online shopping session data and builds machine learning classification models to predict whether an online shopping session will generate revenue.
The target variable is Revenue, which indicates whether the session resulted in a purchase.
Dataset
The project uses the online_shoppers_intention.csv dataset.
- Rows: 12,330
- Columns: 18
- Target variable: Revenue
- Problem type: Binary Classification
Main Features
The dataset contains information about:
- Administrative page visits and duration
- Informational page visits and duration
- Product-related page visits and duration
- Bounce Rate
- Exit Rate
- Page Values
- Special Day
- Month
- Operating System
- Browser
- Region
- Traffic Type
- Visitor Type
- Weekend
Objective
To build and compare machine learning classification models that can predict whether an online shopping session results in revenue.
Technologies Used
- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn (SMOTE)
Project Workflow
1. Data Loading
The dataset is loaded using Pandas from:
online_shoppers_intention.csv
2. Data Exploration
The notebook performs:
- Dataset inspection
- Column identification
- Shape checking
- Statistical description
- Data type checking
- Missing-value checking
- Duplicate-value checking
- Revenue distribution analysis
3. Exploratory Data Analysis
A correlation matrix and heatmap are created to study relationships between numerical features.
Box plots are also used to inspect the distribution of numerical variables and identify outliers.
4. Outlier Treatment
An IQR-based function is used to detect and replace values outside the lower and upper bounds.
5. Categorical Encoding
Categorical data is converted into numerical form using:
- Label Encoding
- One-Hot Encoding / get_dummies
6. Handling Class Imbalance
The dataset is balanced using SMOTE (Synthetic Minority Over-sampling Technique).
This creates a more balanced distribution of the Revenue target classes.
7. Feature Selection
SelectKBest with the f_classif scoring function is used to select the 10 best features for classification.
8. Feature Transformation and Scaling
A Yeo-Johnson Power Transformation is explored for numerical variables.
The selected features are then standardized using StandardScaler.
9. Train-Test Split
The processed data is divided into:
- 80% training data
- 20% testing data
random_state=40 is used for the train-test split.
10. Machine Learning Models
The following classification models are trained and compared:
1. Logistic Regression
2. Decision Tree Classifier
3. Random Forest Classifier
4. AdaBoost Classifier
5. Gradient Boosting Classifier
11. Model Evaluation
The models are evaluated using:
- Accuracy
- Precision
- Recall
- F1 Score
A comparison table is created to identify the performance of the different models.
Model Comparison
The notebook generates a results table containing:
Model	Accuracy	Precision	Recall	F1 Score
Logistic Regression	Generated in notebook	Generated in notebook	Generated in notebook	Generated in notebook
Decision Tree	Generated in notebook	Generated in notebook	Generated in notebook	Generated in notebook
Random Forest	Generated in notebook	Generated in notebook	Generated in notebook	Generated in notebook
AdaBoost	Generated in notebook	Generated in notebook	Generated in notebook	Generated in notebook
Gradient Boosting	Generated in notebook	Generated in notebook	Generated in notebook	Generated in notebook


Conclusion
The project demonstrates a complete machine learning classification workflow for online shopping intention data. It includes data exploration, outlier handling, categorical encoding, class balancing using SMOTE, feature selection, scaling, model training, and performance comparison.
The final model can be selected based on the evaluation metrics generated in the notebook, with particular attention to accuracy, precision, recall, and F1 score.
Project Structure
Online-Shoppers-Intention/
│
├── online(1).ipynb
├── online_shoppers_intention.csv
└── README.md

