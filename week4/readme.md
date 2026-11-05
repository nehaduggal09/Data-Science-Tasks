# Week 4: Machine Learning Model Development and Evaluation

## Project Overview
This project focuses on developing and evaluating a Machine Learning classification model using the publicly available Wine Recognition dataset.

The main objective is to classify wine samples into three different classes based on their chemical properties.

## Dataset
- Dataset: Wine Recognition Dataset
- Source: UCI Machine Learning Repository / Scikit-learn
- Total Records: 178
- Features: 13 numerical features
- Target: Three wine classes

## Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Jupyter Notebook

## Steps Performed
1. Loaded the Wine Recognition dataset.
2. Prepared features and target labels.
3. Split the dataset into training and testing sets.
4. Selected Random Forest Classifier.
5. Applied 5-fold cross-validation.
6. Performed hyperparameter tuning using GridSearchCV.
7. Evaluated the model using accuracy, precision, recall and F1-score.
8. Generated a confusion matrix and feature importance analysis.

## Algorithm Used
Random Forest Classifier was selected because it can handle nonlinear relationships and combine multiple decision trees to improve classification performance.

## Results
- Test Accuracy: 100%
- Macro Precision: 100%
- Macro Recall: 100%
- Macro F1-score: 100%
- Best Cross-validation Accuracy: Approximately 98.52%

## Files Included
- Week4_Model_Development.ipynb
- Week4_Model_Development_Report.docx
- wine_dataset_used.csv

## Conclusion
This project demonstrates the implementation of a complete machine learning classification workflow, including model selection, hyperparameter optimization, cross-validation and performance evaluation.
