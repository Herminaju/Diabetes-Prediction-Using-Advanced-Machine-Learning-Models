# Diabetes-Prediction-Using-Advanced-Machine-Learning-Models
Developed an end-to-end diabetes prediction system with data cleaning, encoding, scaling, and biomarker correlation analysis. Benchmarked multiple ML models and validated the best performer with cross-validation and a multi-class confusion matrix for accurate risk assessment.

This project builds a complete machine-learning pipeline to predict diabetes status using a clinical dataset containing demographic information and several medical biomarkers. The workflow begins by loading the dataset and performing an initial assessment of data quality, identifying issues such as inconsistent class labels and irregular gender formatting. These values are then standardized to ensure reliability in downstream analysis.

To better understand the population, age values are grouped into defined age brackets, making trends across age ranges easier to analyze. A gender distribution chart and class distribution summary help illustrate dataset composition and highlight potential imbalances among the diagnostic categories.

Next, a detailed correlation analysis is performed across all clinical measurements—such as HbA1c, Urea, Creatinine, Cholesterol, triglycerides, HDL, LDL, VLDL, and BMI—to show how these biomarkers relate to each other and to diabetes outcomes. This step helps identify which features carry the strongest predictive signals.

The data is then prepared for machine learning by removing irrelevant fields, converting categorical values (gender, age range, diabetes class) into numerical form, and scaling all clinical measurements. Scaling ensures that all biomarkers contribute equally to model training rather than being dominated by features with larger numeric ranges.

After preprocessing, several machine-learning models are tested and compared using cross-validation, including Logistic Regression, K-Nearest Neighbors, Naive Bayes, Support Vector Machine, Random Forest, Decision Tree, and XGBoost. Each model’s performance is evaluated across multiple folds of the dataset to ensure fairness and robustness. XGBoost emerges as the strongest performer due to its ability to capture complex relationships within clinical data.

Finally, the chosen model is validated on a separate test set using a multi-class confusion matrix. This provides a clear visual representation of the model’s ability to correctly classify patients as non-diabetic, prediabetic, or diabetic, and highlights where misclassifications occur.

Overall, the project showcases a full data-science workflow—from raw medical data to an interpretable, high-accuracy predictive model—demonstrating strong capabilities in data preprocessing, feature engineering, model evaluation, and healthcare-focused analytics.

