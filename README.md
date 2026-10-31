# Diabetes Prediction Using Optimised Machine Learning Models

### A Comparative Study of Support Vector Machine, Random Forest and XGBoost
## Project Overview

This project investigates the application of supervised machine learning to diabetes classification using the Pakistani Diabetes Dataset. Three algorithms—Support Vector Machine (SVM), Random Forest (RF), and Extreme Gradient Boosting (XGBoost)—are implemented and optimised to compare their predictive performance.

The study includes exploratory data analysis, feature preprocessing, hyperparameter optimisation, training and validation, performance comparison, and model interpretation.

## Research Objectives

- Investigate machine learning techniques for diabetes classification.
- Analyse clinical and demographic features associated with the dataset.
- Develop SVM, Random Forest and XGBoost classification models.
- Apply hyperparameter optimisation to improve model selection.
- Evaluate and compare classifiers using multiple performance metrics.
- Investigate model predictions through explainability techniques.

## Dataset

**Dataset:** Pakistani Diabetes Dataset  
**Source:** [Kaggle](https://www.kaggle.com/datasets/mshoaibishaaq/pakistani-diabetes-dataset)

The original dataset contains 912 observations with clinical and demographic attributes. The classification target is diabetes status.

The dataset is not redistributed in this repository. Users should obtain it from the original source and follow its usage terms.

## Methodology

1. Data loading and exploratory analysis.
2. Class distribution analysis and balancing.
3. Missing-value and duplicate checks.
4. Correlation and multicollinearity analysis.
5. Feature preparation and scaling.
6. Training, validation and test splitting.
7. Hyperparameter search and model selection.
8. Evaluation and comparison of the three classifiers.

## Machine Learning Models

### 1. Random Forest

A Random Forest classifier is trained using an explicit hyperparameter search.

Parameters explored include:
- Number of estimators
- Maximum tree depth
- Minimum samples for splitting
- Minimum samples per leaf
- Maximum features
- Bootstrap sampling
- Split criterion
- Class weighting

Model selection considers validation accuracy and the training–validation loss gap.

### 2. Support Vector Machine

SVM classification is explored using different kernel functions.

Parameters explored include:
- Kernel: Linear, RBF and Polynomial
- Regularisation parameter C
- Gamma
- Polynomial degree

The selected model is based on validation accuracy.

### 3. XGBoost

XGBoost is evaluated using a hyperparameter search over:
- Number of estimators
- Maximum tree depth
- Learning rate
- Subsample ratio

Model selection is based on validation accuracy.

## Model Evaluation

The study examines:

- Classification accuracy
- Precision
- Recall
- F1-score
- Confusion matrices
- ROC curves
- Precision–recall curves
- Training and validation performance

Final performance tables and figures will be added after independent verification of the evaluation pipeline.



## Technologies

- Python
- Scikit-learn
- XGBoost
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SHAP
- Statsmodels

## Reproducibility

The experiments were developed using Jupyter Notebook/Google Colab. The original notebook expects a local file named `Pakistani_Diabetes_Dataset.csv`.

A standalone, reproducible notebook and environment requirements are being prepared.

## Limitations

This work is an academic classification experiment, not a clinically validated diagnostic system. The preprocessing and evaluation pipeline requires further review for potential data leakage and correct use of predicted probabilities in ROC and precision–recall analysis. Performance estimates should not be interpreted as clinical diagnostic accuracy.

## Academic Context

This project was completed as part of the Concepts and Technologies of Artificial Intelligence module in the MRes Artificial Intelligence programme at the University of Wolverhampton.

## Author

**Shabana Bashrat**  
MRes Artificial Intelligence | MS Electrical Engineering

**Research Interests:** Machine Learning, Deep Learning, Computer Vision, Model Evaluation, and Responsible AI.
