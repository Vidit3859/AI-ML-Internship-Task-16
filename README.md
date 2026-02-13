# Task 16 — Hyperparameter Tuning using GridSearchCV

## Objective
The goal of this task is to learn how to optimize machine learning models
using hyperparameter tuning with GridSearchCV.

---

## Dataset
Breast Cancer Dataset from sklearn

Samples: 569  
Features: 30  
Target: Binary classification (Malignant / Benign)

---

## Tools Used
- Python
- Pandas
- Scikit-learn
- Jupyter Notebook / Google Colab

---

## Steps Performed

### 1. Data Loading
Loaded the Breast Cancer dataset using sklearn.datasets.

### 2. Train-Test Split
Split the dataset into:
- 80% training data
- 20% testing data

### 3. Default Model
Trained an SVM classifier using default parameters.

### 4. Hyperparameter Grid
Defined tuning parameters:
- C = [0.1, 1, 10, 100]
- kernel = ['linear', 'rbf']
- gamma = ['scale', 'auto']

### 5. GridSearchCV
Applied GridSearchCV with 5-fold cross-validation
to find the best hyperparameters.

### 6. Best Parameters
Extracted the optimal parameter combination.

### 7. Tuned Model Evaluation
Evaluated the tuned model on the test dataset.

### 8. Performance Comparison
Compared default model accuracy with tuned model accuracy.

---

## Results

Default Model Accuracy: 0.9473684210526315  
Tuned Model Accuracy: 0.956140350877193  

Best Parameters:
```
{'C': 100, 'gamma': 'scale', 'kernel': 'linear'}
```

---

## Conclusion
Hyperparameter tuning using GridSearchCV improved the model performance
from 94.73% to 95.61%. This demonstrates how selecting optimal
hyperparameters can enhance model accuracy.

---

## Learning Outcome
- Understanding hyperparameters
- Cross-validation
- GridSearchCV usage
- Model performance optimization

---
