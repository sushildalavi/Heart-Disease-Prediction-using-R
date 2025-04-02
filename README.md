# 🫀 Heart Disease Prediction using R

This project builds and evaluates multiple machine learning models to predict the likelihood of heart disease in patients based on clinical data. It uses the Cleveland Heart Disease dataset (accessed via Kaggle) and leverages R for data exploration, visualization, model training, and performance evaluation.

---

## 📁 Dataset

- **Source**: [Kaggle - Heart Disease Dataset](https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction)
- **Records**: 303 patient entries
- **Features**:
  - Age, Sex, Chest Pain Type, Resting Blood Pressure, Cholesterol
  - Fasting Blood Sugar, Resting ECG, Max Heart Rate, Exercise Induced Angina
  - ST Depression, Slope of Peak Exercise, Major Vessels, Thalassemia
- **Target**: `target` (1 = heart disease, 0 = no heart disease)

---

## 📊 Exploratory Data Analysis

- Correlation Matrix and Heatmap
- Density plots for all numerical features
- Boxplots of key health indicators vs. target
- Categorical bar charts by target outcome
- Pairplot of selected variables

---

## 🤖 Models Used

- **Random Forest**
- **Support Vector Machine (SVM)**
- **XGBoost**

Each model is evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- AUC (ROC Curve)
- Confusion Matrix Heatmap

---

## 🧪 Results Summary

| Model         | Accuracy | Precision | Recall | F1 Score | AUC    |
|---------------|----------|-----------|--------|----------|--------|
| Random Forest | 81.67%   | 83.33%    | 74.07% | 78.43%   | 0.888  |
| SVM           | 81.67%   | 80.77%    | 77.78% | 79.25%   | 0.870  |
| XGBoost       | 75.00%   | 73.08%    | 70.37% | 71.70%   | 0.835  |

> 📌 Random Forest had the highest AUC, while SVM achieved the best F1 Score.

---

## 📦 Tools & Libraries

- **R**
  - ggplot2, dplyr, caret, randomForest, e1071, xgboost, pROC, GGally
- **Jupyter Notebook with R Kernel**
- Visualizations using `ggplot2`, `patchwork`, and `GGally`

---

## 📝 How to Run

1. Clone the repo
2. Install required R packages (see script headers)
3. Launch the Jupyter Notebook or run R script
4. Make sure `heart.csv` is in the working directory

---

## 📄 License

This project is for educational and non-commercial use only.

---

## 🙌 Acknowledgments

- UCI Machine Learning Repository
- Kaggle contributors
