# Predicting Heart Disease Risk Using Machine Learning

## Overview

Heart disease remains the leading cause of death worldwide, making early detection critical for improving patient outcomes. This project develops and evaluates multiple supervised machine learning models to predict heart disease risk using demographic and clinical patient data.

The project demonstrates an end-to-end healthcare data science workflow—from exploratory data analysis and data preprocessing to model development, hyperparameter tuning, threshold optimization, and model interpretation. The goal is to identify patients at elevated risk and support clinical decision-making through data-driven insights.

---

## Business Problem

Healthcare professionals need reliable methods to identify patients who are at high risk for heart disease using routinely collected clinical information. Traditional screening methods may overlook high-risk individuals or delay intervention.

This project explores how machine learning can improve early risk detection, reduce missed diagnoses, and assist healthcare providers in prioritizing preventive care.

---

## Project Objectives

- Predict whether a patient is at risk for heart disease
- Compare multiple supervised machine learning algorithms
- Optimize model performance through hyperparameter tuning
- Improve prediction performance using decision threshold optimization
- Interpret model predictions using feature importance
- Demonstrate how machine learning can support healthcare decision-making

---

## Dataset

The dataset contains demographic and clinical information commonly collected during routine patient evaluations.

### Features include:

- Age
- Sex
- Blood Pressure
- Cholesterol
- Chest Pain
- ECG/EKG Results
- Shortness of Breath
- Fatigue
- Additional cardiovascular indicators

**Target Variable**

- Presence or absence of heart disease

---

## Exploratory Data Analysis (EDA)

EDA included:

- Dataset structure inspection
- Missing value analysis
- Distribution plots
- Histograms
- Boxplots
- Correlation heatmaps
- Feature relationship analysis
- Class distribution visualization

These analyses provided insights that guided preprocessing and model selection.

---

## Data Preprocessing

A machine learning pipeline was created to ensure reproducible preprocessing and eliminate data leakage.

### Preprocessing Steps

- Median imputation for missing numerical values
- Most frequent imputation for categorical variables
- One-Hot Encoding for categorical features
- Standardization of numerical variables
- Train/Test split
- Stratified Cross Validation

---

## Machine Learning Models

Several supervised learning algorithms were evaluated and compared:

- Logistic Regression
- Support Vector Classifier (RBF Kernel)
- K-Nearest Neighbors (KNN)
- Random Forest
- Gradient Boosting
- Histogram Gradient Boosting

Model performance was evaluated using Stratified Cross Validation.

---

## Evaluation Metrics

The following performance metrics were used:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC

Because detecting heart disease is a medical classification problem where distinguishing between positive and negative cases is essential, **ROC-AUC** was selected as the primary model comparison metric.

---

## Model Optimization

Performance improvements included:

- RandomizedSearchCV hyperparameter tuning
- ROC-AUC guided optimization
- Decision threshold optimization
- Precision vs Recall tradeoff analysis
- Youden's J Statistic
- Minimum Recall constraints
- F1-score optimization

These techniques helped improve sensitivity while maintaining acceptable precision for healthcare applications.

---

## Best Performing Model

Among all evaluated algorithms, the **Support Vector Classifier (RBF Kernel)** achieved the strongest overall performance.

Key strengths included:

- Highest ROC-AUC
- Strong balance of precision and recall
- High F1-score
- Excellent discrimination between patients with and without heart disease

---

## Model Interpretation

To improve model transparency, feature importance analysis was performed using **Permutation Importance**.

This allowed identification of the clinical and demographic variables that contributed most to heart disease prediction while improving model interpretability.

---

## Business Impact

This model demonstrates how predictive analytics can support healthcare organizations by:

- Identifying high-risk patients earlier
- Supporting preventive interventions
- Improving clinical decision-making
- Optimizing healthcare resource allocation
- Reducing missed diagnoses
- Improving patient outcomes

---

## Ethical Considerations

Healthcare AI requires responsible deployment.

This project considers:

- Patient privacy
- HIPAA-aware data handling
- Fairness in predictive modeling
- Model transparency
- Responsible AI practices
- Bias mitigation
- Clinical interpretability

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Pipelines
- ColumnTransformer
- RandomizedSearchCV
- Permutation Importance
- Jupyter Notebook

---

## Skills Demonstrated

- Healthcare Data Analytics
- Predictive Modeling
- Machine Learning
- Data Cleaning
- Feature Engineering
- Exploratory Data Analysis
- Classification Modeling
- Hyperparameter Tuning
- Cross Validation
- Model Evaluation
- Threshold Optimization
- Model Interpretation
- Healthcare Decision Support
- Data Visualization

---

## Future Improvements

Future enhancements may include:

- External validation using additional healthcare datasets
- Integration with Electronic Health Record (EHR) systems
- Explainable AI methods such as SHAP values
- Ensemble learning techniques
- Real-time clinical decision support dashboards
- Deep learning approaches for larger healthcare datasets

---

## Author

**Ruth Maddux**

Certified Occupational Therapy Assistant transitioning into Healthcare Data Analytics, leveraging data-driven solutions to solve complex real-world problems.

