# 🎓 Student Performance Prediction

A Machine Learning project that predicts student exam scores using academic, personal, and school-related factors.

## 📌 Project Overview

This project demonstrates a complete Machine Learning workflow, from data exploration and preprocessing to model training, evaluation, and prediction.

The goal is to estimate student exam scores using the `StudentPerformanceFactors.csv` dataset.

## 🎯 Objectives

* Explore and understand the dataset.
* Handle missing values.
* Prepare numerical and categorical features.
* Train a Linear Regression model.
* Compare Linear Regression with Random Forest.
* Evaluate model performance.
* Predict exam scores for new student data.

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook
* Joblib

## 📂 Project Structure

```text
Student_Performance_Prediction/
│
├── models/
├── Student_Performance_Prediction.ipynb
├── StudentPerformanceFactors.csv
└── README.md
```

## 📊 Dataset

**Dataset file:** `StudentPerformanceFactors.csv`

**Target variable:** `Exam_Score`

The dataset contains student-related factors that can be used to explore patterns associated with exam performance.

Place the dataset in the location expected by the notebook before running the cells.


## 🤖 Models Used

### Linear Regression

Used to predict numerical exam scores.

### Random Forest Regressor

Used as a second model to compare prediction performance.

## 📈 Model Evaluation

The following results were obtained on the test dataset:

| Metric   | Linear Regression | Random Forest |
| -------- | ----------------: | ------------: |
| MAE      |            0.4524 |        1.0841 |
| RMSE     |            1.8044 |        2.1657 |
| R² Score |            0.7696 |        0.6682 |

Linear Regression performed better than Random Forest on these test results.

* **MAE:** Measures average absolute prediction error.
* **RMSE:** Penalizes larger prediction errors more strongly.
* **R² Score:** Measures how much variation in the target is explained by the model.

## 🔮 Making Predictions

The notebook includes a reusable prediction function that accepts student information and returns an estimated exam score.

The saved model and preprocessing pipeline can be loaded with Joblib.

## ⚠️ Limitations

* Predictions are estimates, not guaranteed exam results.
* Model performance depends on the dataset and its quality.
* Relationships in the data do not necessarily prove cause and effect.
* Results on this test dataset may not generalize to other student populations.


## 👨‍💻 Author

Muhammad Hamza Khan

