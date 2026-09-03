# 🫀 Framingham Heart Disease Classification Assignment

## 📌 Project Overview

This project is a Machine Learning Classification Assignment based on the **Framingham Heart Study Dataset**.

The main purpose of this project is to predict **TenYearCHD** by applying different Machine Learning Classification Models.

The complete workflow includes data preprocessing, missing value handling, feature scaling, dataset balancing, model comparison, evaluation, Hyperparameter Tuning, and final model optimization.

---

# 🎯 Project Objective

The objectives of this project are:

- Analyze the dataset properly.
- Check and handle missing values.
- Check whether encoding is required.
- Apply Feature Scaling.
- Check whether the dataset is balanced or imbalanced.
- Balance the training data using SMOTE.
- Apply different Classification Models.
- Compare model performance.
- Calculate Accuracy, Precision, Recall, and F1-Score.
- Generate Classification Reports.
- Generate Confusion Matrices.
- Select the best-performing model.
- Perform Hyperparameter Tuning.
- Compare performance before and after tuning.

---

# 📂 Dataset Information

### Dataset File

`framingham.csv`

### Target Variable

`TenYearCHD`

The target variable is used for the classification prediction.

---

# 🔍 Project Workflow

## 1️⃣ Dataset Analysis

The dataset is analyzed by checking:

- Number of rows and columns.
- Column names.
- Data types.
- Dataset information.
- Statistical summary.

---

## 2️⃣ Missing Values Handling

The dataset is checked for missing values.

Missing numerical values are filled using the **median** of each column.

This allows the dataset to be used for Machine Learning without removing a large number of records.

---

## 3️⃣ Duplicate Values Check

Duplicate rows are checked before model training.

---

## 4️⃣ Encoding Check

The data types of the columns are checked.

The dataset contains numerical values, so additional text encoding is not required.

---

## 5️⃣ Feature Scaling

Feature Scaling is performed using:

`StandardScaler()`

Scaling helps bring feature values to a similar range.

It is useful for models such as:

- Logistic Regression
- KNN
- SVM

---

## 6️⃣ Dataset Balancing

The target variable is checked for class imbalance.

SMOTE is used to balance the training dataset.

### What is SMOTE?

SMOTE creates additional examples of the minority class.

This helps the model learn from both classes more fairly.

The testing data is kept unchanged for fair evaluation.

---

# 🤖 Classification Models Used

The following models are used:

### 1. Logistic Regression

A basic model used for classification problems.

### 2. K-Nearest Neighbors (KNN)

KNN predicts a class by checking nearby data points.

### 3. Decision Tree

A Decision Tree makes predictions using a tree-like structure.

### 4. Random Forest

Random Forest combines multiple Decision Trees.

### 5. Support Vector Machine (SVM)

SVM finds a boundary between different classes.

### 6. Naive Bayes

Naive Bayes is a probability-based classification algorithm.

---

# 📊 Evaluation Metrics

The models are evaluated using:

## Accuracy

Shows the percentage of correct predictions.

## Precision

Shows how many positive predictions were correct.

## Recall

Shows how many actual positive cases were correctly identified.

## F1-Score

Provides a balance between Precision and Recall.

---

# 📄 Classification Report

The Classification Report provides:

- Precision
- Recall
- F1-Score
- Support

---

# 🔢 Confusion Matrix

The Confusion Matrix shows:

- Correct predictions.
- Incorrect predictions.

It helps us understand how the model performed for each class.

---

# 🏆 Best Model Selection

All models are compared using their performance results.

The model with the highest Accuracy is selected as the best-performing model.

---

# ⚙️ Hyperparameter Tuning

After selecting the best model, Hyperparameter Tuning is performed.

The project uses:

`GridSearchCV`

GridSearchCV tests different model settings and selects the combination with the best performance.

---

# 📈 Before and After Tuning

The best model's Accuracy is compared:

- Before Hyperparameter Tuning
- After Hyperparameter Tuning

This helps determine whether tuning improved the model.

---

# 📁 Project Files

Your repository should contain:

```text
Framingham-Classification-Assignment/
│
├── Framingham_Classification_Assignment.ipynb
│
├── framingham.csv
│
└── README.md
```

---

# 📚 Libraries Used

- Pandas
- NumPy
- Scikit-learn
- Imbalanced-learn

---

# 💻 Installation

Install the required libraries:

```bash
pip install pandas numpy scikit-learn imbalanced-learn
```

---

# 🚀 How to Run the Project

### Step 1

Download or clone the project.

### Step 2

Keep `framingham.csv` and the Jupyter Notebook in the same folder.

### Step 3

Install the required Python libraries.

### Step 4

Open the `.ipynb` file using Jupyter Notebook or Google Colab.

### Step 5

Run all cells from top to bottom.

---

# ✅ Assignment Requirements Covered

| Requirement | Status |
|---|---|
| Dataset Analysis | ✅ Completed |
| Missing Values Handling | ✅ Completed |
| Encoding Check | ✅ Completed |
| Feature Scaling | ✅ Completed |
| Dataset Balancing | ✅ SMOTE Used |
| Different Classification Models | ✅ 6 Models Used |
| Model Comparison | ✅ Completed |
| Accuracy | ✅ Completed |
| Precision | ✅ Completed |
| Recall | ✅ Completed |
| F1-Score | ✅ Completed |
| Classification Report | ✅ Completed |
| Confusion Matrix | ✅ Completed |
| Best Model Selection | ✅ Completed |
| Hyperparameter Tuning | ✅ Completed |
| Model Optimization | ✅ Completed |
| Code Comments | ✅ Included |
| Simple Explanations | ✅ Included |

---

# 📝 Conclusion

In this project, the Framingham Heart Study dataset was analyzed and prepared for Machine Learning Classification.

Missing values were handled, features were scaled, and the training dataset was balanced using SMOTE.

Six different Classification Models were applied and compared using Accuracy, Precision, Recall, and F1-Score.

The best-performing model was selected and Hyperparameter Tuning was performed using GridSearchCV.

Finally, the performance of the model before and after tuning was compared.
