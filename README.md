Support Vector Machines (SVM) - Breast Cancer Classification

📌 Objective:

The goal of this task is to use Support Vector Machines (SVM) for binary classification of breast cancer cases (Malignant vs Benign) using the Breast Cancer Wisconsin dataset. The task includes training linear and RBF kernel SVMs, tuning hyperparameters, and visualizing decision boundaries.

📂 Dataset:

File: breast-cancer.csv
Source: Breast Cancer Wisconsin Diagnostic Dataset
Features:

30 numeric features describing cell nucleus measurements (e.g., radius, texture, smoothness).

diagnosis column: M (Malignant) / B (Benign).

id column: Patient ID (removed during preprocessing).

🛠 Tools & Libraries:

Python

Pandas – Data handling

NumPy – Numerical operations

Scikit-learn – SVM models, scaling, encoding, evaluation, PCA

Matplotlib – Visualization

📋 Steps Implemented:
1. Load & Inspect Data

Removed unnecessary id column.

Encoded diagnosis column: M → 1, B → 0.

2. Train-Test Split

80% training data, 20% testing data.

3. Feature Scaling

Used StandardScaler to normalize features for SVM performance.

4. Model Training

Linear SVM (kernel='linear', C=1)

RBF SVM (kernel='rbf', C=1, gamma='scale')

5. Evaluation

Confusion Matrix

Classification Report (Precision, Recall, F1-score)

Accuracy Score

6. Hyperparameter Tuning

Used GridSearchCV with cross-validation to find best C and gamma for RBF SVM.

7. Visualization

Reduced dataset to 2D using PCA for plotting decision boundaries of RBF SVM.

📊 Results (Example):

(Actual values will vary depending on tuning results)

Linear SVM Accuracy: ~97%

RBF SVM Accuracy: ~98%

Best Parameters: C=10, gamma=0.01

▶ How to Run:

Install dependencies:

pip install pandas numpy scikit-learn matplotlib


Run the Python script or Jupyter Notebook:

python task7_svm.py
or
Open TASK7.ipynb in Jupyter Notebook and run all cells.

View:

Printed model performance metrics in console/notebook output.

Decision boundary plot for visual understanding.

📌 Notes:

Feature scaling is mandatory for SVM models.

PCA is used only for visualization, not for training the final model.

The dataset is balanced enough for direct accuracy comparison.
