# Predictive_maintanance# 🔧 Predictive Maintenance Using Machine Learning

This project demonstrates how machine learning can be applied to **predict machine failure** and classify the **type of failure** using sensor data from industrial machines. It combines real-world-like datasets, feature engineering, model training (Random Forest & XGBoost), and evaluation — all inside a clean, reproducible Jupyter Notebook.

---

##  Objectives

-  Predict **whether a machine will fail or not** (binary classification)
-  Predict the **type of failure** (multi-class classification)
-  Analyze and visualize sensor data to understand failure behavior
-  Evaluate model performance using accuracy, precision, recall, and confusion matrix

---

##  Dataset Overview

The dataset contains machine sensor readings such as:

| Feature                    | Description                                |
|---------------------------|--------------------------------------------|
| `Air temperature [K]`     | Ambient temperature                        |
| `Process temperature [K]` | Internal machine temperature               |
| `Torque [Nm]`             | Rotational force applied                   |
| `Rotational speed [rpm]`  | Shaft rotation speed                       |
| `Tool wear [min]`         | Duration of tool use                       |
| `Type`                    | Machine type (`L`, `M`, `H`)               |
| `Target`                  | Machine failure (0 = No, 1 = Yes)          |
| `Failure Type`            | Specific failure type (TWF, HDF, etc.)     |

---

##  Technologies Used

- Python (Pandas, NumPy, Matplotlib, Seaborn)
- Scikit-learn (`RandomForestClassifier`, `MultiOutputClassifier`, `StandardScaler`)
- XGBoost (`XGBClassifier`)
- Plotly (for interactive visualizations)
- Jupyter Notebook

---

##  Machine Learning Models

###  Random Forest (MultiOutputClassifier)
- Predicts both `Target` and `Failure Type`
- Robust to outliers and non-linearities
- Feature importance extraction supported

###  XGBoost (MultiOutputClassifier)
- Gradient boosting model with high accuracy
- Handles imbalanced data well
- Highly tunable and fast

---

##  Evaluation Metrics

- **Accuracy**
- **Precision**
- **Recall**
- **Confusion Matrix**
- **Classification Report**

---

##  Visualizations

- Histogram and box plots of features
- Correlation heatmap
- Failure distribution (pie chart & bar plots)
- Confusion matrices for both targets

