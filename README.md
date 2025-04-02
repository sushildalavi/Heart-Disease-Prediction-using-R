# HeartFlow: Scalable ML-Driven Cardiovascular Risk Detection

This project presents a hybrid machine learning workflow to predict the likelihood of heart disease using clinical and physiological data. The solution combines robust modeling and visualization in R with simulated distributed data processing using PySpark and HDFS concepts to demonstrate scalable healthcare analytics.

---

## Dataset

- **Source**: [Kaggle - Heart Disease Predictions by Desalegn Geb](https://www.kaggle.com/code/desalegngeb/heart-disease-predictions/notebook)
- **Based on**: Cleveland Heart Disease dataset from the UCI Machine Learning Repository
- **Samples**: 303 patient records
- **Features**:
  - Age, Sex, Chest Pain Type (`cp`), Resting Blood Pressure (`trestbps`)
  - Cholesterol (`chol`), Fasting Blood Sugar (`fbs`), Resting ECG (`restecg`)
  - Max Heart Rate (`thalach`), Exercise Induced Angina (`exang`)
  - ST Depression (`oldpeak`), Slope of Peak Exercise, Major Vessels (`ca`), Thalassemia (`thal`)
- **Label**: `target` (1 = presence of heart disease, 0 = absence)

---

## Project Highlights

- Built an end-to-end ML pipeline in R with Random Forest, SVM, and XGBoost models.
- Simulated distributed healthcare data ingestion and transformation using PySpark DataFrames and HDFS workflows.
- Applied topic modeling (LDA, NMF) to explore interpretability and textual insights (conceptual integration).
- Evaluated model performance with confusion matrix heatmaps, ROC curves, and correlation visualizations.

---

## Exploratory Data Analysis

- Correlation matrix visualized using `corrplot`
- Pairplots using `GGally::ggpairs` for multivariate relationships
- Density plots, boxplots, and barplots for feature-target comparisons
- Summary statistics with `summary()` and `dplyr`

---

## Machine Learning Models

- Random Forest (`randomForest`)
- Support Vector Machine (`e1071`)
- XGBoost (`xgboost`)

Evaluation metrics include:

- Accuracy
- Precision
- Recall
- F1 Score
- AUC and ROC curves
- Confusion matrices (visualized)

---

## Results Summary

| Model         | Accuracy | Precision | Recall | F1 Score | AUC    |
|---------------|----------|-----------|--------|----------|--------|
| Random Forest | 81.67%   | 83.33%    | 74.07% | 78.43%   | 0.888  |
| SVM           | 81.67%   | 80.77%    | 77.78% | 79.25%   | 0.870  |
| XGBoost       | 75.00%   | 73.08%    | 70.37% | 71.70%   | 0.835  |

---

## Tools and Technologies

- **R Packages**:
  - `caret`, `ggplot2`, `dplyr`, `xgboost`, `e1071`, `randomForest`, `pROC`, `GGally`, `corrplot`, `gridExtra`
- **Big Data Simulation**:
  - PySpark: DataFrames, RDDs, basic transformations
  - HDFS-style file I/O (simulated)
- **Topic Modeling**:
  - LDA and NMF (conceptual integration)

---

## How to Run

1. Clone the repository
2. Ensure `heart.csv` is placed in the project root
3. Run the R Notebook or script in Jupyter (IRkernel) or RStudio
4. Optionally, execute `pyspark_simulation.py` for Big Data simulation
5. Install dependencies in R using `install.packages()` and configure PySpark if needed

---

## License

This repository is intended for educational and research purposes only.

---

## Acknowledgments

- UCI Machine Learning Repository  
- Kaggle contributor Desalegn Geb  
- Apache Spark and the open-source R community
