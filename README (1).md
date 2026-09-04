# 🫀 Heart Failure Classification Assignment

## 📌 Project Overview

This project is a **Machine Learning Classification Assignment** based on the **Heart Failure Clinical Records Dataset**.

The main goal of this project is to build different Machine Learning models and predict whether a patient experienced a **DEATH_EVENT**.

The project follows a complete Machine Learning workflow, starting from dataset analysis and preprocessing and ending with model evaluation and Hyperparameter Tuning.

---

# 🎯 Project Objective

The objective of this assignment is to:

- Analyze the dataset properly.
- Check and handle missing values.
- Check whether encoding is required.
- Apply Feature Scaling where required.
- Check whether the dataset is balanced or imbalanced.
- Balance the training dataset using SMOTE.
- Apply different Classification Models.
- Compare the performance of all models.
- Calculate Accuracy, Precision, Recall, and F1-Score.
- Generate Classification Reports.
- Generate Confusion Matrices.
- Select the best-performing model.
- Perform Hyperparameter Tuning.
- Compare model performance before and after tuning.

---

# 📂 Dataset Information

### Dataset Name

`heart_failure_clinical_records_dataset.csv`

### Target Variable

`DEATH_EVENT`

The target variable is used to predict the final classification outcome.

The dataset contains different medical and clinical features that are used as input variables for Machine Learning models.

---

# 🔍 Project Workflow

## 1️⃣ Dataset Analysis

The dataset is first loaded using the Pandas library.

The following information is checked:

- Number of rows and columns.
- Column names.
- Data types.
- Basic statistical information.
- Overall dataset structure.

This step helps us understand the dataset before applying Machine Learning.

---

## 2️⃣ Missing Values Check

Missing values are checked using:

```python
df.isnull().sum()
```

If missing values are present, they should be handled before training the model.

For this dataset, the missing values are checked before moving to the next step.

---

## 3️⃣ Duplicate Values Check

Duplicate records are checked using:

```python
df.duplicated().sum()
```

This helps identify whether the dataset contains repeated rows.

---

## 4️⃣ Encoding Check

Encoding is required when a dataset contains categorical or text values.

The data types of all columns are checked.

Since the dataset contains numerical values, encoding is not required.

---

## 5️⃣ Feature and Target Selection

The dataset is divided into:

### Features (X)

Features are the input variables used by the Machine Learning model.

```python
X = df.drop("DEATH_EVENT", axis=1)
```

### Target (y)

The target variable is the value we want to predict.

```python
y = df["DEATH_EVENT"]
```

---

## 6️⃣ Train-Test Split

The dataset is divided into:

- **80% Training Data**
- **20% Testing Data**

The training data is used to train the models.

The testing data is used to check the final performance of the models.

---

## 7️⃣ Feature Scaling

Feature Scaling is applied using:

```python
StandardScaler()
```

Feature Scaling helps bring the values of different features to a similar scale.

It is especially useful for models such as:

- Logistic Regression
- KNN
- SVM

---

## 8️⃣ Dataset Balancing Using SMOTE

The target variable is checked to determine whether the dataset is balanced.

SMOTE is used to balance the training dataset.

### What is SMOTE?

SMOTE creates additional examples of the minority class.

This helps Machine Learning models learn from both classes more fairly.

**Important:** SMOTE is applied only to the training data. The testing data remains unchanged.

---

# 🤖 Classification Models Used

The following Machine Learning Classification Models are used in this project:

### 1. Logistic Regression

A simple classification model used for predicting two possible classes.

### 2. K-Nearest Neighbors (KNN)

This model predicts a class by checking nearby data points.

### 3. Decision Tree

This model makes decisions using a tree-like structure.

### 4. Random Forest

Random Forest uses multiple Decision Trees to make predictions.

### 5. Support Vector Machine (SVM)

SVM tries to find the best boundary between different classes.

### 6. Naive Bayes

Naive Bayes is a probability-based classification algorithm.

---

# 📊 Model Evaluation

Each model is evaluated using the following metrics:

## ✅ Accuracy

Accuracy shows the percentage of correct predictions made by the model.

## ✅ Precision

Precision shows how many positive predictions were actually correct.

## ✅ Recall

Recall shows how many actual positive cases were correctly identified.

## ✅ F1-Score

The F1-Score provides a balance between Precision and Recall.

---

# 📄 Classification Report

The Classification Report provides detailed information about:

- Precision
- Recall
- F1-Score
- Support

This helps us understand the performance of every classification model.

---

# 🔢 Confusion Matrix

A Confusion Matrix shows the number of:

- Correct predictions.
- Incorrect predictions.

Example:

```text
[[36  5]
 [ 6 13]]
```

This means:

| Actual Value | Predicted 0 | Predicted 1 |
|-------------|------------:|------------:|
| Actual 0 | 36 | 5 |
| Actual 1 | 6 | 13 |

In this example:

- **36** predictions of class 0 were correct.
- **5** predictions were incorrectly predicted as class 1.
- **6** predictions were incorrectly predicted as class 0.
- **13** predictions of class 1 were correct.

---

# 🏆 Model Comparison

All Classification Models are compared using:

- Accuracy
- Precision
- Recall
- F1-Score

The results are stored in a comparison table.

The model with the highest performance is selected as the best-performing model.

---

# ⚙️ Hyperparameter Tuning

After selecting the best model, Hyperparameter Tuning is performed.

### What is Hyperparameter Tuning?

Hyperparameters are settings that can affect the performance of a Machine Learning model.

Different values are tested to find the best combination.

---

## GridSearchCV

This project uses:

```python
GridSearchCV
```

GridSearchCV automatically tests different parameter combinations.

The combination that gives the best accuracy is selected.

---

# 📈 Before and After Hyperparameter Tuning

The model's performance is compared:

### Before Tuning

The original best model performance is recorded.

### After Tuning

The model is tested again using the best parameters found by GridSearchCV.

This helps determine whether Hyperparameter Tuning improved the model's performance.

---

# 📁 Project Files

Your GitHub repository should contain the following files:

```text
Heart-Failure-Classification/
│
├── FINAL_Heart_Failure_Classification_Assignment.ipynb
│
├── heart_failure_clinical_records_dataset.csv
│
└── README.md
```

---

# 📚 Libraries Used

The following Python libraries are required:

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn

---

# 💻 Installation

Install the required libraries using:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn
```

---

# 🚀 How to Run the Project

### Step 1

Download or clone the GitHub repository.

### Step 2

Make sure the dataset file and Jupyter Notebook are in the same folder.

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
| Missing Values Check | ✅ Completed |
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
| Step-by-Step Explanation | ✅ Included |

---

# 📝 Conclusion

In this project, the Heart Failure Clinical Records Dataset was analyzed and prepared for Machine Learning Classification.

Different Classification Models were applied and evaluated using Accuracy, Precision, Recall, and F1-Score.

The dataset was balanced using SMOTE to handle class imbalance.

The performance of all models was compared, and the best-performing model was selected.

Hyperparameter Tuning was then performed using GridSearchCV to find better model settings.

Finally, the model performance was evaluated again to determine whether the tuning process improved the results.

---
