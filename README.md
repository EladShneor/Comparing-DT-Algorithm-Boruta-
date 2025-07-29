#Teen Smartphone Addiction –Comparing DT Models & Feature Selection

This notebook explores a dataset related to teenage smartphone addiction. The main goal is to predict a target variable (e.g., addiction score) using machine learning models with a strong focus on **feature selection** and **boosting algorithms**.

###Key Steps in This Notebook:

1. **Data Exploration**  
   We inspect the structure of the training dataset, including shape, column names, and data types.

2. **Target Encoding**  
   Categorical variables are encoded using methods suitable for tree-based models while avoiding data leakage.

3. **Feature Selection – BorutaPy**  
   We use the Boruta algorithm with a `RandomForestRegressor` as a weak learner to select the most relevant features from the dataset.

4. **Model Training – CatBoost**  
   The CatBoost model is trained twice: once on all features and once on the filtered feature set obtained from Boruta, to compare performance.

5. **Evaluation**  
   Model performance is evaluated using metrics like **R² score**, and we display the number of features used in each model to highlight the efficiency gains.

---

###Requirements

- Python 3.x  
- pandas, numpy  
- scikit-learn  
- catboost
- xgboost
- boruta  

---

###Output

By the end of this notebook, we identify the most important features contributing to smartphone addiction and assess how feature selection impacts the predictive power of tree-based boosting models.

---

> Created by Elad Shenior | 2025
