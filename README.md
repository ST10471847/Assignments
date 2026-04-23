# Project Overview
This project focuses on applying Linear Regression to predict medical insurance charges based on demographic, lifestyle, and geographic factors. The analysis follows a structured data analytics workflow, including data import, exploratory data analysis (EDA), feature selection, model training, and evaluation.
The dataset used is a publicly available medical insurance dataset sourced from Kaggle and is used as a proof‑of‑concept before potential localisation.

Dataset

Source: Kaggle – Medical Insurance Dataset
File: insurance.csv
Observations: 1,338 records (1,337 after duplicate removal)
Target Variable: charges
Features:

age
sex
bmi
children
smoker
region




Tools and Technologies

Python
Google Colab
Libraries Used:

pandas
numpy
matplotlib
seaborn
scikit‑learn




Analysis Workflow
1. Data Import and Setup

Kaggle API was configured in Google Colab to download the dataset.
The dataset was extracted and loaded into a pandas DataFrame.

2. Exploratory Data Analysis (EDA)

Dataset structure and size were examined.
Duplicate records were identified and removed.
Missing values were checked.
Descriptive statistics were generated.
Visualisations were created to explore:

Feature distributions
Categorical variable frequencies
Relationships between predictors and insurance charges



3. Feature Selection

Categorical variables were encoded using one‑hot encoding.
A variance‑based feature screening method was applied.
All features were retained, as sufficient variability was observed.

4. Model Training

The dataset was split into training (80%) and testing (20%) sets.
A Multiple Linear Regression model was trained using Ordinary Least Squares.
Default hyperparameters were used to establish a baseline model.

5. Model Evaluation

Predictions were generated on the test dataset.
Performance was evaluated using:

Mean Squared Error (MSE)
Mean Absolute Error (MAE)
R‑squared (R²)


Regression coefficients were analysed to interpret feature influence.


Key Findings

The model achieved an R² score of 0.807, indicating strong explanatory power.
Smoking status was the most influential predictor of insurance charges.
Age, BMI, and number of children showed positive relationships with cost.
Gender and region had relatively smaller effects.
The model performed well as a baseline, interpretable proof‑of‑concept.


Project Files

PDA8411_Assignment.ipynb – Google Colab notebook containing the full analysis
insurance.csv – Dataset used for modelling
README.md – Project overview and documentation


Conclusion
This project demonstrates the correct application of Linear Regression for predicting medical insurance charges and shows a clear understanding of the end‑to‑end data analytics process. The results align with exploratory insights and meet the requirements of the PDA8411 assessment brief.
