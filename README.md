# Machine Learning Course-End Project: Healthcare

## Project Objective
The primary objective of this machine learning course-end project is to address the critical issue of cardiovascular diseases, which are the leading cause of death worldwide. To tackle this problem effectively, the project aims to develop a predictive model that can identify the causes and predict heart attacks with a high degree of accuracy. The project utilizes a comprehensive dataset containing information about various factors that might impact cardiovascular health.

## Dataset Description
The dataset used for this project is provided in an Excel file named **"CEP 1_ Dataset.xlsx."** It contains the following variables:

* Age: Age in years
* Sex: 1 = male; 0 = female
* cp: Chest pain type
* trestbps: Resting blood pressure (in mm Hg on admission to the hospital)
* chol: Serum cholesterol in mg/dl
* fbs: Fasting blood sugar > 120 mg/dl (1 = true; 0 = false)
* restecg: Resting electrocardiographic results
* thalach: Maximum heart rate achieved
* exang: Exercise induced angina (1 = yes; 0 = no)
* oldpeak: ST depression induced by exercise relative to rest
* slope: Slope of the peak exercise ST segment
* ca: Number of major vessels (0-3) colored by fluoroscopy
* thal: 3 = normal; 6 = fixed defect; 7 = reversible defect
* Target: 1 or 0 (indicating the presence or absence of cardiovascular disease)
***
### Task 1: Preliminary Analysis
#### Data Inspection
The initial data inspection involved loading the dataset and identifying any missing values, duplicates, or anomalies. The dataset was loaded successfully, and we found that it required preprocessing steps to handle missing data and duplicates.

##### Data Cleaning
Handling Missing Values: We observed missing values in some columns, and we employed appropriate strategies such as mean imputation for numerical columns to ensure that missing values were properly handled.

**Removing Duplicates**: Duplicate rows were identified and removed from the dataset to maintain data integrity.
***
### Task 2: Data Exploration and Reporting
**Preliminary Statistical Summary**
We calculated measures of central tendencies (mean, median) and spread (standard deviation) for numerical features like age, trestbps, chol, thalach, oldpeak, etc. This summary provided an initial understanding of the data distribution.

**Exploring Categorical Variables**
We identified categorical variables such as sex, cp, fbs, restecg, exang, slope, ca, thal, and target. For each of these variables, we created count plots to visualize the frequency of each category, gaining insights into their distributions.

**CVD Occurrence Across Age Category**
We analyzed the occurrence of Cardiovascular Disease (CVD) across different age categories. This allowed us to identify age-related trends in CVD prevalence.

**Composition by Sex Category**
We examined the composition of all patients with respect to the sex category, providing insights into the gender distribution within the dataset.

**Resting Blood Pressure Analysis**
We investigated if heart attacks could be detected based on anomalies in resting blood pressure (trestbps) of patients. This analysis involved plotting trestbps against the target variable.

**Cholesterol Levels and Target Variable**
We described the relationship between cholesterol levels (chol) and the target variable (CVD). Visualization helped us understand how cholesterol impacts CVD risk.

**Peak Exercise and Heart Attack Occurrence**
We explored the relationship between peak exercising (slope) and the occurrence of a heart attack (target). This analysis helped identify if certain types of exercise were associated with CVD.

**Thalassemia and CVD**
We checked if thalassemia (thal) is a major cause of CVD by examining the distribution of thalassemia categories with respect to CVD.

**Other Factors and CVD Occurrence**
We listed how other factors, including chest pain type (cp), fasting blood sugar (fbs), exercise-induced angina (exang), ST depression (oldpeak), and the number of major vessels (ca), determine the occurrence of CVD.

**Pair Plot**
We used a pair plot to understand the relationships between all given variables, aiding in the identification of potential correlations and patterns in the data.
***
### Task 3: Building Baseline Models
We built baseline models to predict the risk of a heart attack using logistic regression and random forest algorithms. Feature selection was performed using correlation analysis, and logistic regression leveraging standard error and p-values from statsmodels.

**Logistic Regression Model**
We employed logistic regression to build a predictive model. The model was trained on a subset of the data and evaluated for its predictive performance using accuracy metrics.

**Random Forest Model**
A random forest classifier was trained and evaluated to predict the risk of a heart attack. This ensemble learning approach provided insights into the feature importance for prediction.

**Feature Selection**
Feature selection was performed using correlation analysis to identify relationships between features and the target variable. Additionally, logistic regression with p-values and standard errors from statsmodels was utilized for further feature selection.
***
### Conclusion
This comprehensive project aimed to address the critical issue of cardiovascular diseases through effective data analysis and predictive modeling. The tasks included data inspection and cleaning, in-depth data exploration, and the development of baseline predictive models. The findings and insights gained from this project provide a foundation for further advanced machine learning techniques and models to predict heart attacks with higher accuracy, ultimately contributing to better healthcare outcomes.
