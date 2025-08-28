# Insurance-Charges-Analysis
This project builds a comprehensive end-to-end pipeline to analyze and model a medical insurance dataset. By leveraging personal attributes such as age, BMI, smoking status, and more, the goal is to predict an individual's insurance costs accurately.

---

## 🎯 Objective

To perform detailed exploration, data preprocessing, feature transformation, and statistical testing on a medical insurance dataset, and ultimately develop a regression model capable of accurately estimating insurance charges.

---

## 🧰 Tools & Technologies

| Category             | Libraries / Tools Used                               |
| -------------------- | ---------------------------------------------------- |
| Programming Language | Python                                               |
| Data Manipulation    | `pandas`, `numpy`                                    |
| Data Visualization   | `matplotlib`, `seaborn`                              |
| Statistical Analysis | `scipy` (Pearson correlation, Chi-square tests)      |
| Machine Learning     | `scikit-learn` (Linear Regression, train/test split) |
| Data Preprocessing   | `StandardScaler`, `OneHotEncoding` (via `pandas`)    |

---

## 📂 Dataset Overview

* **File:** `insurance.csv`
* **Records:** 1,338
* **Features:** 7 input variables + 1 target

### Variables:

* `age`: Age of the individual
* `sex`: Gender (`male` / `female`)
* `bmi`: Body Mass Index
* `children`: Number of dependents
* `smoker`: Smoking status (`yes` / `no`)
* `region`: Geographic region of residence
* `charges`: Annual insurance charges *(target)*

---

## 🔄 Workflow Summary

### 1. **Exploratory Data Analysis**

* Analyzed distributions, relationships, and trends
* Visualized data through histograms, scatter plots, and heatmaps
* Identified outliers with boxplots

### 2. **Data Cleaning**

* Checked and removed duplicate rows
* Ensured no missing values were present
* Encoded categorical features numerically

### 3. **Feature Engineering**

* Created a `bmi_category` feature (Underweight → Obese)
* Applied one-hot encoding to `sex`, `smoker`, and `region`
* Standardized continuous variables: `age`, `bmi`, `children`

### 4. **Statistical Testing**

* Used Pearson correlation to examine relationships with `charges`
* Applied Chi-square tests to assess categorical variable significance

### 5. **Model Development**

* Trained a **Linear Regression** model using `scikit-learn`
* Split data into 80% training and 20% testing sets
* Evaluated model performance using R² and Adjusted R² metrics

### 6. **Final Feature Set**

* `age`, `is_female`, `bmi`, `children`, `is_smoker`, `region_southeast`, `bmi_category_Obese`

---

## 📌 Conclusion

This project showcases a full data science workflow — from raw data analysis to feature selection and predictive modeling. The steps and techniques used here can serve as a solid foundation for solving similar regression-based problems in real-world healthcare analytics.

---

