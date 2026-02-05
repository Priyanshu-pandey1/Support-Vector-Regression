# 📈 Support Vector Regression (SVR) Analysis

This repository demonstrates a detailed implementation of **Support Vector Regression (SVR)** using Scikit-Learn. The project focuses on predicting continuous values by comparing various kernels and optimizing hyperparameters to find the best-performing model.

## 🚀 Project Overview

The goal of this project is to implement SVR and analyze how different mathematical kernels and regularization parameters affect the $R^2$ score. By utilizing `GridSearchCV`, I was able to automate the tuning process to achieve a more robust and generalized model.

### Key Highlights:
* **Kernel Comparison:** Evaluated model performance across **RBF**, **Linear**, and **Polynomial** kernels.
* **Hyperparameter Tuning:** Used `GridSearchCV` to optimize:
    * `C` (Regularization parameter)
    * `epsilon` (Margin of tolerance)
    * `kernel` type
* **Advanced SVR:** Implemented `LinearSVR` for optimized linear regression handling in high-dimensional spaces.

## 🛠️ Tech Stack

* **Language:** Python
* **Libraries:** Scikit-Learn, NumPy, Pandas
* **Algorithm:** Support Vector Regression (SVR)

---

## 📊 Performance & Evaluation

### 1. Kernel Benchmarking (Default Parameters)
| Kernel | Train $R^2$ Score | Test $R^2$ Score |
| :--- | :--- | :--- |
| **RBF (Default)** | **0.659** | **0.488** |
| **Linear** | 0.451 | 0.443 |
| **Polynomial** | 0.579 | 0.242 |

### 2. Hyperparameter Optimization Results
Through `GridSearchCV`, the following parameters were identified as the most effective for this dataset:
* **Best Parameters:** `{'C': 10, 'epsilon': 0.1, 'kernel': 'linear'}`

### 3. Final Optimized Model Performance
Using the tuned parameters, the model achieved a more balanced performance between the training and testing sets, reducing the risk of overfitting:
* **Final Train $R^2$ Score:** 0.515
* **Final Test $R^2$ Score:** 0.474

---

## 📂 Repository Structure

* `svr_implementation.ipynb`: The primary Jupyter Notebook containing the SVR model logic, kernel analysis, and hyperparameter tuning.

