# Week 3: Statistical Modeling and Hypothesis Testing

## 📌 Project Overview
This project applies statistical hypothesis testing and multinomial logistic regression to the Wine Recognition dataset. The goal is to investigate differences in chemical measurements among wine classes and evaluate whether these measurements can be used to predict class membership.

The dataset contains 178 observations, 13 numerical chemical features, and three target classes.

## 🎯 Objectives
- Formulate a research question and statistical hypotheses.
- Validate and prepare the dataset for modeling.
- Apply one-way ANOVA to test differences in mean alcohol content.
- Develop a multinomial logistic regression classifier.
- Evaluate model performance using classification metrics.
- Apply stratified cross-validation.
- Discuss model assumptions, limitations, and future improvements.

## 📂 Dataset
**Dataset:** Wine Recognition Dataset

**Source:** UCI Machine Learning Repository and scikit-learn.

Dataset link: https://archive.ics.uci.edu/dataset/109/wine

## 🛠️ Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- SciPy
- Scikit-learn
- Jupyter Notebook

## ❓ Research Questions
1. Does mean alcohol content differ significantly among the three wine classes?
2. Can the 13 chemical measurements be used to predict the wine class?

## 🧪 Hypothesis Testing

### One-Way ANOVA

**Null hypothesis (H₀):** The population mean alcohol content is equal across all three wine classes.

**Alternative hypothesis (H₁):** At least one wine class has a different population mean alcohol content.

**Significance level:** α = 0.05

The ANOVA F-statistic and p-value are used to evaluate the null hypothesis. A p-value below 0.05 provides evidence against the null hypothesis, subject to the test's assumptions.

## 🤖 Statistical Modeling

### Multinomial Logistic Regression
Multinomial logistic regression is used to predict one of the three wine classes from the 13 chemical features.

### Data Preparation
- Separate the predictor variables from the target variable.
- Use a stratified 75/25 train-test split.
- Standardize numerical features using `StandardScaler`.
- Fit the scaler and logistic regression model within a pipeline to reduce data leakage.

### Model Evaluation
The classifier is evaluated using:
- Test accuracy
- Macro-averaged F1-score
- Confusion matrix
- Five-fold stratified cross-validation

Cross-validation provides an additional estimate of performance across multiple data splits.

## 📊 Results and Interpretation
The notebook calculates the ANOVA statistic and p-value, fits the logistic regression model, and reports the classification metrics.

The confusion matrix helps identify which wine classes are correctly classified and where misclassifications occur. Cross-validation is used to assess how sensitive model performance is to a particular train-test split.

Actual numerical results should be taken from the executed notebook and accompanying report.

## 🚀 How to Run the Project

1. Clone or download this repository.
2. Install the required libraries:

   ```bash
   pip install pandas numpy matplotlib scipy scikit-learn jupyter
   ```

3. Place `cleaned_wine_dataset.csv` in the same directory as the notebook.
4. Launch Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

5. Open `Week3_Statistical_Modeling_Hypothesis_Testing.ipynb`.
6. Run all cells sequentially.

## 📁 Project Files
- `Week3_Statistical_Modeling_Hypothesis_Testing.ipynb` — Notebook containing hypothesis testing and model evaluation code.
- `Week3_Statistical_Modeling_Report.docx` — Detailed statistical modeling report.
- `cleaned_wine_dataset.csv` — Cleaned dataset used for modeling.

## ⚠️ Assumptions and Limitations
- ANOVA assumes independent observations and has distributional and variance assumptions.
- Logistic regression assumes a suitable relationship between predictors and class log-odds.
- Multicollinearity may affect coefficient stability.
- A small dataset can lead to uncertainty in estimated model performance.
- Cross-validation does not replace external validation on independent data.
- High performance on this benchmark dataset does not guarantee equivalent performance on real-world wine samples.

## 🔮 Future Improvements
- Compare logistic regression with other classification algorithms.
- Investigate multicollinearity using Variance Inflation Factor (VIF).
- Examine residual and model diagnostics.
- Explore post-hoc tests to identify which class pairs differ.
- Evaluate the model on independent external data.

## 📝 Conclusion
This project demonstrates the practical application of statistical hypothesis testing and classification modeling. ANOVA is used to investigate differences in alcohol content, while multinomial logistic regression evaluates the predictive value of chemical measurements for wine classification.


Data Science Internship — Week 3 Task
