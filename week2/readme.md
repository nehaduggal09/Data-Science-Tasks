# Week 2: Exploratory Data Analysis (EDA)

## 📌 Project Overview
This project performs Exploratory Data Analysis (EDA) on the Wine Recognition dataset. The objective is to understand the dataset's structure, summarize its numerical features, identify potential outliers, discover patterns, and investigate relationships between chemical measurements and wine classes.

The dataset contains 178 wine samples, 13 numerical chemical features, and one target variable representing three wine classes.

## 🎯 Objectives
- Understand the structure and characteristics of the dataset.
- Perform data quality checks for missing values and duplicate records.
- Calculate descriptive statistics.
- Visualize feature distributions and relationships.
- Identify potential outliers using the Interquartile Range (IQR) method.
- Perform hypothesis testing to investigate differences between wine classes.
- Document findings and limitations.

## 📂 Dataset
**Dataset:** Wine Recognition Dataset

**Source:** UCI Machine Learning Repository and scikit-learn.

Dataset link: https://archive.ics.uci.edu/dataset/109/wine

### Dataset Information
- Observations: 178
- Numerical features: 13
- Target classes: 3
- Missing values in the cleaned dataset: 0
- Duplicate records in the cleaned dataset: 0

## 🛠️ Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- SciPy
- Jupyter Notebook

## 🔍 Analysis Performed

### 1. Data Inspection
Examined dataset dimensions, column types, missing values, duplicate records, and class distribution.

### 2. Descriptive Statistics
Calculated measures including:
- Mean
- Median
- Standard deviation
- Variance
- Minimum and maximum
- Quartiles and interquartile range

### 3. Data Visualization
Created the following visualizations:
- Histograms to examine feature distributions.
- Box plots to identify potential outliers.
- Scatter plots to investigate relationships between chemical features.
- Correlation heat maps to explore relationships among numerical variables.

### 4. Outlier Detection
Applied the 1.5 × IQR rule to flag potential outliers. These observations were not automatically removed because unusual measurements are not necessarily errors.

### 5. Hypothesis Testing
Used one-way Analysis of Variance (ANOVA) to investigate whether mean alcohol content differs across the three wine classes.

- **Null hypothesis (H₀):** Mean alcohol content is equal across all three classes.
- **Alternative hypothesis (H₁):** At least one class has a different mean alcohol content.
- **Significance level:** 0.05

## 📊 Key Findings
The analysis examines differences in chemical measurements across wine classes, the distribution and variability of individual features, and correlations between numerical variables.

The ANOVA result is used to evaluate whether the observed differences in mean alcohol content provide statistically significant evidence against the null hypothesis.

## 🚀 How to Run the Project

1. Clone or download this repository.
2. Install the required libraries:

   ```bash
   pip install pandas numpy matplotlib scipy scikit-learn jupyter
   ```

3. Keep `cleaned_wine_dataset.csv` in the same directory as the notebook.
4. Launch Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

5. Open `Week2_EDA_Wine_Dataset.ipynb`.
6. Run the notebook cells sequentially.

## 📁 Project Files
- `Week2_EDA_Wine_Dataset.ipynb` — Jupyter Notebook containing the analysis code.
- `Week2_EDA_Report.docx` — Detailed EDA report.
- `cleaned_wine_dataset.csv` — Cleaned dataset used for analysis.

## ⚠️ Limitations
- The dataset contains a relatively small number of observations.
- Correlation does not establish causation.
- Statistical outliers are not necessarily erroneous measurements.
- ANOVA conclusions depend on its assumptions.
- Findings may not generalize to wine samples outside this dataset.

## 📝 Conclusion
This project demonstrates how exploratory data analysis, descriptive statistics, visualization, and hypothesis testing can be used to understand a structured dataset. The results provide a foundation for subsequent statistical modeling and machine learning.


Data Science Internship — Week 2 Task
