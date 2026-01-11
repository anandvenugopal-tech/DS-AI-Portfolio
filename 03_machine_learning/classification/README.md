# Classification 

This directory contains implementations of supervised learning algorithms designed to predict discrete categories or class labels. From fundamental probabilistic models to advanced ensemble methods, these notebooks explore how to draw decision boundaries between different types of data.



---

## Included Models

| Model | Core Concept | Key Advantage |
| :--- | :--- | :--- |
| **Logistic Regression** | Linear probability modeling via Sigmoid function. | Highly interpretable, fast, and a great baseline. |
| **K-Nearest Neighbors** | Instance-based learning using distance metrics. | Simple to understand; makes no assumptions about data distribution. |
| **Support Vector Machines** | Maximizing the margin between classes using hyperplanes. | Effective in high-dimensional spaces; robust to outliers. |
| **Decision Trees** | Hierarchical rule-based splitting. | Captures non-linear relationships and is easy to visualize. |
| **Random Forest** | Ensemble of Decision Trees using Bagging. | Reduces overfitting and provides feature importance rankings. |
| **Naive Bayes** | Probabilistic classification based on Bayes' Theorem. | Extremely fast; works well with high-dimensional text data. |

---

## The Classification Workflow

Each implementation follows a standardized pipeline:
1. **Data Ingestion**: Loading standard Scikit-Learn datasets (Iris, Breast Cancer, Wine, Digits).
2. **Preprocessing**: Handling feature scaling (essential for KNN and SVM).
3. **Model Selection**: Initializing the algorithm with specific hyperparameters.
4. **Evaluation**: Using metrics beyond simple accuracy to judge performance.



---

## Evaluation Metrics Explained

To truly understand how a classifier is performing, we use:

* **Accuracy**: The percentage of total correct predictions.
* **Precision**: The ability of the classifier not to label a negative sample as positive.
* **Recall (Sensitivity)**: The ability of the classifier to find all the positive samples.
* **F1-Score**: The harmonic mean of Precision and Recall (best for imbalanced data).
* **Confusion Matrix**: A table layout that allows visualization of the performance of an algorithm.

---

## Key Takeaways
* **Scaling Matters**: Algorithms like KNN and SVM rely on distance calculations; without **StandardScaler**, features with larger scales will dominate the model.
* **Bias-Variance Tradeoff**: A simple Logistic Regression might **underfit** (High Bias), while a deep Decision Tree might **overfit** (High Variance).
* **Linear vs Non-Linear**: SVM with an RBF kernel or Random Forests are better suited for datasets where classes cannot be separated by a straight line.

---
