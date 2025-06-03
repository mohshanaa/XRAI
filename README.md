# XRAI: A Hybrid Anomaly Detection Framework for Credit Card Fraud Detection

## 🔍 Overview

**XRAI** (short for **XGBoost, Random Forest, Autoencoder, and Isolation Forest**) is a hybrid machine learning framework designed to detect fraudulent credit card transactions with high accuracy and robustness. By combining **supervised** and **unsupervised** learning techniques, XRAI tackles the challenges of class imbalance, adversarial behavior, and model explainability in real-world financial environments.

This repository contains a single self-contained Jupyter Notebook that includes all code, from data preprocessing to model training, ensemble, and evaluation.

> **Research Title:** *A Hybrid Anomaly Detection Framework Combining Supervised and Unsupervised Learning for Credit Card Fraud Detection*

---

## 🧠 Model Architecture

XRAI integrates the following components:

* **X** - `XGBoost` (Supervised)
* **R** - `Random Forest` (Supervised)
* **A** - `Autoencoder` (Unsupervised)
* **I** - `Isolation Forest` (Unsupervised)

These are combined in a hybrid ensemble using majority voting for robust fraud prediction.

Additional techniques used:

* `MinMaxScaler` for feature normalization
* `PCA` for dimensionality reduction
* `Train/Test Split` for supervised learning
* `Thresholding` for anomaly detection via reconstruction error

---

## 📈 Performance Summary

| Metric       | Value  |
| ------------ | ------ |
| Accuracy     | 99.98% |
| Precision    | 95.69% |
| Recall (TPR) | 92.50% |
| F1-Score     | 94.07% |
| MCC          | 94.07% |
| AUC          | 0.9885 |

---

## 📁 Repository Structure

```
XRAI-Fraud-Detection/
├── data/
│   └── creditcard.csv              # Dataset (must be added manually)
├── XRAI_fraud_detection.ipynb      # Full end-to-end notebook (main file)
├── requirements.txt
└── README.md
```

---

## 📊 Dataset

This project uses the **Credit Card Fraud Detection Dataset** available on Kaggle:
🔗 [https://www.kaggle.com/mlg-ulb/creditcardfraud](https://www.kaggle.com/mlg-ulb/creditcardfraud)

Download the CSV file and place it inside the `/data` folder.

---

## ▶️ How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/XRAI-Fraud-Detection.git
   cd XRAI-Fraud-Detection
   ```

2. Install required packages:

   ```bash
   pip install -r requirements.txt
   ```

3. Open the notebook:

   ```bash
   jupyter notebook XRAI_fraud_detection.ipynb
   ```

---

## 🧪 Features Covered in Notebook

* Data loading and exploration
* Preprocessing (scaling, PCA, outlier removal)
* Model training:
  * XGBoost
  * Random Forest
  * Autoencoder
  * Isolation Forest
* Ensemble learning
* Evaluation: Confusion Matrix, Classification Report, AUC, Precision/Recall

---

## 🔬 Future Work

* Add temporal modeling (LSTM, Transformers)
* Improve explainability using SHAP and LIME
* Explore dynamic ensembles
* Test across multiple real-world datasets
* Improve robustness against adversarial attacks

---

## 📜 Citation

If you use this framework in your work, please cite:

> Shanaa, M., Abdallah, S. (2025). *A Hybrid Anomaly Detection Framework Combining Supervised and Unsupervised Learning for Credit Card Fraud Detection*. F1000Research (submitted).

---

## 📧 Contact

For questions or feedback:
📩 `mohammadsshanaa@gmail.com`

