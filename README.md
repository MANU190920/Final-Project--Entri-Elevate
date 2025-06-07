# 🛒 Predicting Online Purchase Intent Using User Behavior Features

This project aims to predict whether an online user will make a purchase during a session, based on their browsing behavior. Supervised machine learning models are applied to a publicly available dataset after extensive preprocessing and model tuning.

## 🎯 Objective

To predict **purchase intent** (binary classification: purchase or no purchase) by analyzing **user behavior features** using **supervised machine learning algorithms**.

---

## 📂 Dataset

- **Source**: [UCI Online Shoppers Purchasing Intention Dataset](https://archive.ics.uci.edu/ml/datasets/Online+Shoppers+Purchasing+Intention+Dataset)
- **Instances**: 12,330
- **Features**: 18 numerical and categorical behavior-based variables (e.g., pages visited, duration, bounce rates, etc.)
- **Target Variable**: `Revenue` (True if a purchase occurred, else False)

---

## 🧼 Data Preprocessing

- Handled missing values
- Converted categorical features using Label Encoding
- Applied feature scaling using StandardScaler
- Addressed **class imbalance** using **SMOTE**

---

## 🧠 Models Used

The following models were evaluated:

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- Support Vector Machine (SVM)
- K-Nearest Neighbors (KNN)

---

## 🔍 Hyperparameter Tuning

- Applied **GridSearchCV** to tune the top-performing models
- Models evaluated using **Accuracy, Precision, Recall, and F1-Score**

---

## 📊 Results

### ✅ Final Selected Model Performance (Test Data):
- **Accuracy**: 84.06%
- **F1-Score for Purchase Class (1)**: 0.26

### 📦 Model Performance on Unseen Data:
- **Accuracy**: 74.48%
- **F1-Score**: 0.5091

> These results highlight improved generalization and better performance in identifying minority class (purchase intent) on unseen data.

---

## 🧩 Conclusion

> The final tuned model demonstrated strong overall accuracy and improved capability to detect purchases after addressing class imbalance and hyperparameter optimization. This project shows that **user behavior data can be effectively leveraged** to predict purchase intent in online shopping contexts.

---
