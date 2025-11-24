
# 🛡️ Credit Card Fraud Detection using PyOD AutoEncoder

Author: Samrat Baral

This project implements an **unsupervised fraud detection system** using a **Deep Learning AutoEncoder** from the `PyOD` library, applied to an anonymized **credit card transaction dataset** sourced from Kaggle and loaded via `kagglehub`.

---

## 📌 Project Overview

Credit card fraud detection is challenging due to:

- Highly **imbalanced datasets**
- Constantly evolving fraud patterns
- Need to detect **previously unseen anomalies**

AutoEncoders are well-suited because:

✅ They learn normal transaction patterns  
✅ Fraudulent transactions produce **higher reconstruction error**  
✅ No labels are required for training  

---

## 🧠 Model Details

The notebook includes:

### ✔ Data Loading
- Uses `kagglehub` to fetch dataset automatically:
```
whenamancodes/fraud-detection
```

### ✔ Preprocessing
- Feature selection
- `RobustScaler` normalization
- Stratified train/test split

### ✔ Model Training
- PyOD `AutoEncoder`
- Deep neural architecture
- Contamination threshold based on fraud ratio

### ✔ Evaluation Metrics
The notebook outputs:

✅ ROC-AUC  
✅ Precision  
✅ Recall  
✅ F1-score  
✅ Confusion Matrix  
✅ Classification Report  

### ✔ Visualizations
- anomaly score histogram
- fraud vs normal distribution

---

## 📂 Repository Contents

```
/project-root
│
├── fraud_detection_autoencoder_pyod.ipynb   # Main Colab notebook
├── README.md                                # This file
├── MANIFEST.md                              # Describes included files
├── autoencoder_fraud_pyod.pkl (optional)    # Saved model
```

---

## ▶️ How to Run in Google Colab

### **Option 1 — Upload Notebook**
1. Open Google Colab
2. Upload the `.ipynb` file
3. Run all cells

### **Option 2 — Open with One Click**
(Provide link once uploaded to GitHub)

---

## 🛠️ Installation (Local Environment)

### Install Dependencies
```bash
pip install pyod kagglehub[pandas-datasets] numpy pandas scikit-learn matplotlib joblib
```

---

## 🔗 Dataset Source

Dataset Name: **Credit Card Fraud Detection**  
Provider: Kaggle  
Loader method: `kagglehub`  
File Used: `creditcard.csv`

> Dataset is **not included in the repo** due to licensing – download via KaggleHub in notebook.

---

## 📸 What to Include in Your Assignment Word Report

✅ Screenshot of model training logs  
✅ Screenshot of evaluation metrics (ROC-AUC, Precision, Recall, F1)  
✅ Screenshot of confusion matrix  
✅ Screenshot of anomaly score plot  
✅ GitHub repository URL  

---

## 👨‍💻 Best Practices Followed

✅ Well‑commented code  
✅ Modular cell structure  
✅ Reproducible random state  
✅ No hard‑coded dataset paths  
✅ Academic‑friendly formatting  

---

## ✅ Recommended Enhancements (Optional)

If continuing research:

🔹 Compare with Isolation Forest  
🔹 Add SMOTE + supervised classifier  
🔹 Tune deep network layers  
🔹 Deploy REST API scoring endpoint  

---

## 📬 Support

If you want:
✅ A formatted **Word report**,  
✅ A **PowerPoint presentation**,  
✅ A **GitHub repo setup**,  
✅ A **comparison model**,  

Just ask — I can generate those too.

---

## © Academic Usage

This project may be submitted for coursework as long as:

✅ You run the notebook yourself  
✅ You add your own observations  
✅ You cite Kaggle as dataset source  

---
