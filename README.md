
# Heart Disease Prediction using KNN

## 📌 Overview

This project implements a machine learning pipeline to predict the presence of heart disease using clinical data. The model is built using the **K-Nearest Neighbors (KNN)** algorithm and evaluated with standard classification metrics.

The goal is to create a **reliable baseline model** for healthcare risk prediction, where early detection is critical.

---

## 📊 Dataset

The dataset (`heart.csv`) contains patient-level medical attributes such as:

* 🧓 Age
* ⚧️ Sex
* 💔 Chest pain type
* 🩺 Resting blood pressure
* 🧪 Cholesterol levels
* ❤️ Maximum heart rate

### 🎯 Target Variable

* `1` → Heart disease present
* `0` → No heart disease

---

## ⚙️ Project Workflow

### 1️⃣ Data Preprocessing

* Load dataset using **Pandas**
* Split into features (`X`) and target (`y`)
* Train-test split (80/20)

### 2️⃣ Feature Scaling

* Applied **StandardScaler**
* Prevented data leakage by fitting only on training data

### 3️⃣ Model Training

* Algorithm: **K-Nearest Neighbors (KNN)**
* Parameter: `k = 5`

### 4️⃣ Model Evaluation

The model is evaluated using:

* ✅ Accuracy
* 🎯 Precision
* 🔍 Recall
* 📉 Confusion Matrix
* ⚖️ F1 Score

---

## 📈 Evaluation Metrics

* **Accuracy** → Overall correctness
* **Precision** → Quality of positive predictions
* **Recall** → Ability to detect actual cases
* **F1 Score** → Balance between precision and recall

> ⚠️ In healthcare applications, **Recall is prioritized** to reduce missed diagnoses.

---

## 📊 Sample Performance

Typical results for this model:

* 📌 Accuracy: ~80–85%
* 📌 Precision: ~78–85%
* 📌 Recall: ~80–90%
* 📌 F1 Score: ~0.78–0.85

---

## 🧠 Key Insights

* 📏 Feature scaling is critical for distance-based models like KNN
* 🔢 Model performance depends heavily on the value of `k`
* ⚠️ F1 Score alone is not sufficient for medical decisions
* 🏥 Minimizing false negatives is essential in healthcare

---

## ⚠️ Limitations

* No hyperparameter tuning (fixed `k=5`)
* No cross-validation
* No comparison with other models
* KNN may not scale well for large datasets

---

## 🚀 Future Improvements

* 🔍 Hyperparameter tuning using GridSearchCV
* 🔁 Cross-validation for robust evaluation
* 🤖 Model comparison (Logistic Regression, Random Forest, XGBoost)
* 📊 ROC-AUC analysis
* ⚖️ Class imbalance handling

---

## 💻 Installation

```bash
pip install pandas scikit-learn
```

---

## ▶️ Usage

```bash
python KNN.py
```

---

## 📁 Project Structure

```
├── heart.csv
├── KNN.py
└── README.md
```

---

## 📌 Conclusion

This project demonstrates a structured approach to building a machine learning model for heart disease prediction. While effective as a baseline, further optimization is required for real-world deployment.

-
