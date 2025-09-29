# Elevate Labs AI/ML Internship - Task 5: K-Nearest Neighbors (KNN)

## 📝 Objective

This repository contains the solution for **Task 5: K-Nearest Neighbors (KNN)** of the Elevate Labs AI & ML Internship. The objective of this task is to implement the KNN algorithm to build a classification model that predicts the presence of heart disease based on a set of patient medical attributes.

---

## ❤️ Dataset

The project uses the **Heart Disease UCI** dataset (`heart.csv`). This dataset contains 14 columns, where the `target` column is the label indicating the presence (1) or absence (0) of heart disease.

---

## 🛠️ Workflow & Methodology

The project follows a standard machine learning workflow for building and evaluating a KNN classifier.

* **1. Data Preprocessing & Scaling**: The dataset was loaded and checked for integrity. A critical preprocessing step, **Feature Scaling**, was performed using `StandardScaler`. This is essential for distance-based algorithms like KNN to ensure that all features contribute equally to the model's predictions.
* **2. Train-Test Split**: The scaled data was split into a training set (80%) and a testing set (20%) for unbiased model evaluation.
* **3. Finding the Optimal 'k'**: The choice of 'k' (the number of neighbors) is a crucial hyperparameter. The "Elbow Method" was used to find the optimal 'k' by training and evaluating the model on a range of 'k' values and selecting the one that resulted in the lowest error rate.
* **4. Model Training**: A `KNeighborsClassifier` model was trained using the optimal 'k' value found in the previous step.
* **5. Model Evaluation**: The final model's performance was evaluated on the test set using an **accuracy score** and a detailed **classification report**, which includes precision, recall, and F1-score for each class.

---

## 📈 Evaluation Results

* The model achieved an **Accuracy Score** of **`[Insert your accuracy score, e.g., 0.89]`** on the test data.
* The **Classification Report** showed a high **recall** for class 1 (patients with heart disease), indicating the model is very effective at identifying individuals who have the condition.

---

## 💻 Tools and Libraries Used

* Python
* Pandas
* Scikit-learn
* Matplotlib & Seaborn

---

## 🚀 How to Run

1.  Clone this repository to your local machine.
2.  Ensure you have Python and the required libraries installed.
3.  Open and run the Jupyter Notebook (`.ipynb`) file to see the complete implementation and results.
