# Diabetes_Prediction_machine_learning_project

Abstract

Diabetes is a chronic condition that affects millions of people and often remains undiagnosed until complications
appear. Early prediction can support timely medical intervention. In this project, a machine learning system was
developed to predict whether an individual is diabetic based on clinical measurements. The work includes data
preprocessing, feature engineering, model training, and evaluation. Six algorithms were tested: Logistic Regression,
Decision Tree, Random Forest, Support Vector Machine (SVM), K-Nearest Neighbors (KNN), and a simple neural
network. Across the evaluated classical models, the SVM achieved the highest test accuracy (90.79%), closely
followed by Logistic Regression and Random Forest (89.47% each). The report discusses model behaviour,
limitations, and possible improvements, and includes annotated screenshots of the underlying implementation for
each key stage of the pipeline.

1. Motivation and Rationale

Diabetes is one of the most common metabolic disorders worldwide. Many people remain unaware of their
condition until serious symptoms appear. Predictive models can help identify individuals at risk and support
preventive healthcare.
Machine learning is well suited for this task because it can learn patterns from clinical data and provide fast, noninvasive predictions. This project explores how different algorithms behave on a real dataset and evaluates their
reliability for early diabetes detection.

2. State of the Art (SOTA)

Machine learning has been widely applied to diabetes prediction. Common approaches include:
● Logistic Regression for baseline medical classification tasks.
● Decision Trees and Random Forests for handling mixed numerical and categorical data.
● SVM for high-dimensional clinical features.
● Neural networks for learning non-linear relationships.
Most studies report that ensemble methods (Random Forest, Gradient Boosting) and SVM often outperform simpler
models. However, performance depends heavily on preprocessing, scaling, and the quality of the dataset. This
project follows similar techniques and compares them on a publicly available dataset.

3. Problem Statement

The goal is to build a model that predicts whether a person has diabetes based on clinical measurements such as
glucose level, BMI, age, and insulin level. The task is a binary classification problem.

4. Objectives

The project aims to:
● Build a machine learning model that predicts diabetes accurately.
● Compare multiple algorithms to understand their strengths and weaknesses.
● Apply preprocessing, feature engineering, and scaling to improve performance.
● Evaluate models using standard metrics and discuss failure cases.
● Identify the most reliable model for this dataset.
5. Dataset Description
The dataset was obtained from Kaggle and contains medical measurements for individuals with and without
diabetes. Key characteristics:
● Binary target variable: diabetic (1) or non-diabetic (0)
● Features: Glucose, Insulin, BMI, Age, Pregnancies, Blood Pressure, Skin Thickness, Diabetes Pedigree

6. Methodology

7. Experiments and Results
Evaluation Metrics
Models were evaluated using:
● Accuracy
● Precision
● Recall
● F1-score
● Confusion matrix
● ROC curve (recommended for future presentation — not yet implemented in the current notebook)
Model Performance
Note: the table below reflects the actual accuracy values produced by the notebook's saved run (see Figures 8–12),
which differ from an earlier draft of this report. SVM was the strongest performer in this run, narrowly ahead of
Logistic Regression and Random Forest.
Model Test Accuracy (%)
Support Vector Machine (SVM) 90.79
Logistic Regression 89.47
Random Forest 89.47
Decision Tree 88.16
K-Nearest Neighbors (KNN) 88.16

8. Conclusions

This project demonstrates how different machine learning algorithms behave on a diabetes prediction task. In the
current notebook run, SVM achieved the highest accuracy, with Logistic Regression and Random Forest close
behind. Feature engineering and scaling meaningfully shaped these results. Future improvements could include:
● Using larger datasets
● Applying more advanced ensemble methods (e.g. Gradient Boosting, XGBoost)
● Adding ROC curves and AUC scores for each model
● Performing deeper hyperparameter tuning
● Adding k-fold cross-validation for more reliable evaluation
Machine learning shows strong potential for supporting early diabetes detection.
