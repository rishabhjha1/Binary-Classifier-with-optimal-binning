# Binary-Classifier-with-optimal-binning
# Heart Disease Binary Classification with Optimal Binning and Logistic Regression

## 1. Introduction
This notebook demonstrates a binary classification workflow using the `heart.csv` dataset. The steps include:
1. Loading the dataset.
2. Splitting the data into train and test sets.
3. Performing **Optimal Binning** for features and calculating **Weight of Evidence (WOE)**.
4. Training a **Logistic Regression** classifier.
5. Evaluating the model using the **ROC Curve** and **ROC AUC Score**.
6. Visualizing WOE tables and plots.

---

## 2. Dataset Overview
The `heart.csv` dataset contains medical records used to predict heart disease. The columns are:
- **Age**: Age of the patient.
- **Sex**: Gender of the patient (1 = male, 0 = female).
- **Chest Pain Type**: 4 types of chest pain experienced.
- **Resting Blood Pressure**: Resting blood pressure in mm Hg.
- **Serum Cholesterol**: Cholesterol level in mg/dl.
- **Fasting Blood Sugar**: Whether fasting blood sugar > 120 mg/dl (1 = true, 0 = false).
- **Resting ECG Results**: Results of resting electrocardiographic measurements.
- **Maximum Heart Rate Achieved**: Max heart rate achieved during exercise.
- **Exercise Induced Angina**: Presence of exercise-induced angina (1 = yes, 0 = no).
- **Oldpeak**: ST depression induced by exercise relative to rest.
- **Slope of Peak Exercise**: The slope of the ST segment.
- **Number of Major Vessels**: Colored by fluoroscopy (range 0-3).
- **Thal**: Thalassemia (0 = normal, 1 = fixed defect, 2 = reversible defect).
- **Target**: Binary target variable (1 = presence of heart disease, 0 = absence).

---

## 3. Optimal Binning and Weight of Evidence
We use `optbinning` to:
- Perform optimal binning for numerical features.
- Calculate the Weight of Evidence (WOE) for each bin.

---

## 4. Logistic Regression
A Logistic Regression classifier is trained using the WOE-transformed features.

---

## 5. Performance Evaluation
- **ROC AUC Score** is calculated for both training and testing datasets.
- **ROC Curve** is plotted to visualize model performance.

---

## 6. WOE Tables and Visualizations
- WOE tables summarize binning details, including event rates, WOE values, and IV (Information Value).
- WOE plots provide visual insights into the relationship between features and the target.

---

### Key Results
- **ROC AUC Scores** for training and testing datasets.
- WOE transformation tables and visualizations for each feature.
