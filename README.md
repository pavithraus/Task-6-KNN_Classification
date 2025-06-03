# Task-6-KNN_Classification

This project implements the **K-Nearest Neighbors (KNN)** algorithm on the classic **Iris dataset** to classify iris flower species. It covers data preprocessing, model training with hyperparameter tuning, evaluation, and decision boundary visualization using PCA.

---

##  Objectives

- Load and preprocess the Iris dataset.
- Train and evaluate KNN models for flower classification.
- Tune the number of neighbors (K) to improve accuracy.
- Visualize confusion matrix and decision boundaries.
- Understand the effect of dimensionality reduction using PCA.

---

##  Dataset Used

- **Dataset**: [Iris.csv]
- **Target Variable**: Species
- **Features**:
  - SepalLengthCm
  - SepalWidthCm
  - PetalLengthC
  - PetalWidthCm

---

##  Key Tasks & Workflow

### 1.  Data Preprocessing
- Drop the Id column.
- Separate features (X) and target (y).
- Normalize features using StandardScaler.

### 2. KNN Classification
- Use train_test_split for 80/20 data division.
- Train KNN models with different k values (1 to 20).
- Plot **K vs Accuracy** to find the optimal value.
- Train the final model with the best K.

### 3. Model Evaluation
- Calculate and print:
  - Accuracy Score
  - Confusion Matrix
  - Classification Report
- Visualize confusion matrix using heatmap.

### 4. PCA + Decision Boundary Visualization
- Reduce features to 2D using PCA.
- Train KNN again on PCA-transformed data.
- Plot the decision boundaries and data distribution.

---

##  Evaluation Summary

| Metric               | Description                         |
|----------------------|-------------------------------------|
| **Accuracy**         | Varies by K, best near ~97%         |
| **Confusion Matrix** | Visualized via heatmap              |
| **Classification Report** | Includes Precision, Recall, F1  |

> *Exact values depend on train/test split and random state.*

---

## Visual Outputs

Line chart of accuracy vs. K

![K Value vs Accuracy](https://github.com/user-attachments/assets/2d2ed27c-693f-44f3-bd7a-8114f6fd1110)
       
Confusion matrix heatmap   

![Confusion Matrix](https://github.com/user-attachments/assets/3f960708-928f-436f-aa47-e75686bdc4bb)

KNN decision boundaries (PCA-based)

![decision_boundary](https://github.com/user-attachments/assets/6ed85efe-1c02-404d-8286-7c6593ba922c)

---

## Libraries Used

- pandas, numpy
- matplotlib, seaborn
- scikit-learn (KNeighborsClassifier, PCA, metrics, etc.)

---

## About

- This project was developed by Pavithra.
- As part of a machine learning learning track.
- Built using Google Colab
- Learning resources: chatgpt, Geek or Geeks,w3school.
- Special Thanks to Elevate Labs
