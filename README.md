# 🧠 Scalable Heart Disease Prediction Using R and PySpark

This project builds a scalable machine learning pipeline to predict the likelihood of heart disease in patients using clinical and physiological data. It combines robust statistical modeling and visualization in R with simulated distributed data processing via PySpark and HDFS concepts, creating a hybrid workflow suitable for real-world healthcare analytics.

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

## 🧪 Project Highlights

- Developed a modular ML pipeline in R using Random Forest, SVM, and XGBoost
- Simulated distributed healthcare analytics with PySpark and HDFS for scalable data processing
- Used topic modeling techniques (LDA, NMF) for additional interpretability exploration
- Visualized model performance through ROC curves, correlation heatmaps, and confusion matrix heatmaps

---

## 📊 Exploratory Data Analysis

- Correlation heatmap using `corrplot`
- Pairplot of selected numeric features using `GGally::ggpairs`
- Density plots by `target`
- Boxplots and barplots for feature comparison
- Descriptive stats using `summary()` and `dplyr`

---

## 🤖 Machine Learning Models

- Random Forest (`randomForest`)
- Support Vector Machine (SVM)
- XGBoost (`xgboost`)
- Performance Metrics:
  - Accuracy
  - Precision
  - Recall
  - F1 Score
  - ROC Curve + AUC
  - Confusion Matrix (heatmaps)

---

## 🧪 Results Summary

| Model         | Accuracy | Precision | Recall | F1 Score | AUC    |
|---------------|----------|-----------|--------|----------|--------|
| Random Forest | 81.67%   | 83.33%    | 74.07% | 78.43%   | 0.888  |
| SVM           | 81.67%   | 80.77%    | 77.78% | 79.25%   | 0.870  |
| XGBoost       | 75.00%   | 73.08%    | 70.37% | 71.70%   | 0.835  |

> ✅ SVM achieved the best F1 Score; Random Forest had the highest AUC.

---

## ⚙️ Tools & Libraries

- **Language**: R, PySpark (for simulation)
- **R Packages**:
  - `caret`, `ggplot2`, `dplyr`, `xgboost`, `e1071`, `randomForest`, `pROC`, `GGally`, `corrplot`, `gridExtra`
- **PySpark Components**:
  - Basic use of `RDDs`, DataFrames, and `map-reduce` style operations for healthcare data simulation
- **Topic Modeling**:
  - LDA and NMF (exploratory integration)

---

## 🚀 How to Run

1. Clone the repository
2. Place `heart.csv` in the project root directory
3. Run the R notebook (`.ipynb`) or script using Jupyter/IRkernel or RStudio
4. (Optional) Explore `pyspark_simulation.py` for distributed simulation
5. Install required packages using `install.packages()` and `pyspark` setup

---

## 📄 License

This project is intended for educational and non-commercial use only.

---

## 🙌 Acknowledgments

- UCI Machine Learning Repository  
- Kaggle contributor [Desalegn Geb](https://www.kaggle.com/code/desalegngeb)  
- Apache Spark & Open Source R Community
