# 🫀 Heart Disease Prediction using R

This project builds and evaluates multiple machine learning models to predict the likelihood of heart disease in patients based on clinical and physiological data. It uses a cleaned version of the Cleveland Heart Disease dataset, accessed via Kaggle, and leverages R for comprehensive data analysis, visualization, and model evaluation.

---

## 📁 Dataset

- **Source**: [Kaggle - Heart Disease Predictions by Desalegn Geb](https://www.kaggle.com/code/desalegngeb/heart-disease-predictions/notebook)
- **Based on**: Cleveland Heart Disease dataset from the UCI Machine Learning Repository
- **Records**: 303 patient entries
- **Features**:
  - Age, Sex, Chest Pain Type (`cp`), Resting Blood Pressure (`trestbps`)
  - Cholesterol (`chol`), Fasting Blood Sugar (`fbs`), Resting ECG (`restecg`)
  - Max Heart Rate (`thalach`), Exercise Induced Angina (`exang`)
  - ST Depression (`oldpeak`), Slope of Peak Exercise, Major Vessels (`ca`), Thalassemia (`thal`)
- **Target**: `target` (1 = heart disease, 0 = no heart disease)

---

## 📊 Exploratory Data Analysis

- Correlation heatmap using `corrplot`
- Pairplot of selected numeric features using `GGally::ggpairs`
- Density plots for all numeric features by `target`
- Boxplots and barplots to compare features across target classes
- Summary statistics using R's base functions and `dplyr`

---

## 🤖 Machine Learning Models

- **Random Forest**
- **Support Vector Machine (SVM)**
- **XGBoost**

Each model is evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC Curve + AUC
- Confusion Matrix (visualized as heatmaps)

---

## 🧪 Results Summary

| Model         | Accuracy | Precision | Recall | F1 Score | AUC    |
|---------------|----------|-----------|--------|----------|--------|
| Random Forest | 81.67%   | 83.33%    | 74.07% | 78.43%   | 0.888  |
| SVM           | 81.67%   | 80.77%    | 77.78% | 79.25%   | 0.870  |
| XGBoost       | 75.00%   | 73.08%    | 70.37% | 71.70%   | 0.835  |

> 📌 **SVM** achieved the best F1 Score; **Random Forest** had the highest AUC.

---

## 📦 Tools & Libraries

- **Language**: R
- **Libraries**:
  - `ggplot2`, `dplyr`, `caret`, `randomForest`, `e1071`, `xgboost`, `pROC`, `GGally`, `corrplot`, `gridExtra`
- **Environment**:
  - Jupyter Notebook with IRkernel or RStudio

---

## 📝 How to Run

1. Clone the repository
2. Ensure `heart.csv` is in your working directory
3. Launch `Heart_Disease_Prediction_using_R.ipynb` in Jupyter, or run the `.R` script
4. Install required R packages if needed (see script header)

---

## 📄 License

This project is intended for educational and non-commercial use only.

---

## 🙌 Acknowledgments

- UCI Machine Learning Repository
- Kaggle contributor [Desalegn Geb](https://www.kaggle.com/code/desalegngeb)
- Open-source R community
