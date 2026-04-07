# 🔐 Malicious URL Detection System

**An ML-Powered Cybersecurity System for Detecting Defacement & Malicious URLs**

---

## 📌 Project Overview

The **Malicious URL Detection System** is a machine learning-based cybersecurity application designed to classify URLs as **benign or malicious (defacement attacks)** using structural and lexical features.

The system leverages supervised learning models and efficient feature engineering to enable **fast, real-time detection of suspicious URLs**, helping prevent phishing and web-based attacks.

---

## 💡 What It Does

| Capability              | Description                                       |
| ----------------------- | ------------------------------------------------- |
| URL Classification      | Detects whether a URL is benign or malicious      |
| Feature-Based Detection | Uses structural URL patterns for prediction       |
| Multi-Model Comparison  | Evaluates Logistic Regression, SVM, Decision Tree |
| Data Balancing          | Handles class imbalance for fair training         |
| Real-time Ready         | Can be extended to APIs or web apps               |

---

## 🎯 Project Aims

**"To build a scalable and efficient ML system capable of identifying malicious URLs using lightweight yet powerful feature engineering."**

### Key Objectives:

✅ Achieve strong classification performance
✅ Handle real-world noisy datasets
✅ Ensure fast execution for large datasets
✅ Maintain interpretability of features
✅ Build a production-ready ML pipeline

---

## ✨ Features

### 🧠 ML-Based Detection

* Logistic Regression for baseline performance
* Linear SVM for fast and scalable classification
* Decision Tree for interpretability

### 🔍 Feature Engineering

Extracted key URL-based features:

* URL length
* Number of dots (`.`)
* Number of digits
* Slash count (`/`)
* IP address presence
* Shortened URL detection

### ⚖️ Data Handling

* Robust CSV parsing (handles corrupted rows)
* Automatic label detection and cleaning
* Class balancing using sampling techniques

### 📊 Model Evaluation

* Accuracy Score
* Confusion Matrix
* Classification Report (Precision, Recall, F1-score)

---

## 🏗️ Architecture

```
                MALICIOUS URL DETECTION SYSTEM
-----------------------------------------------------
                     │
         ┌───────────┴───────────┐
         ▼                       ▼
     DATA LOADING          DATA CLEANING
         │                       │
         ▼                       ▼
 FEATURE ENGINEERING      LABEL PROCESSING
         │                       │
         └───────────┬───────────┘
                     ▼
               DATA BALANCING
                     │
                     ▼
              MODEL TRAINING
         (LR | SVM | Decision Tree)
                     │
                     ▼
               MODEL EVALUATION
                     │
                     ▼
               PREDICTION OUTPUT
```

---

## 🤖 ML Models

| Model               | Purpose                         |
| ------------------- | ------------------------------- |
| Logistic Regression | Baseline classification         |
| Linear SVM          | Fast large-scale classification |
| Decision Tree       | Explainable model               |

---

## ⚙️ Workflow

```
Raw URL Data
     │
     ▼
CSV Parsing (error handling)
     │
     ▼
Data Cleaning (labels, nulls)
     │
     ▼
Feature Engineering
     │
     ▼
Class Balancing
     │
     ▼
Train-Test Split
     │
     ▼
Model Training (LR, SVM, DT)
     │
     ▼
Evaluation (Accuracy, Confusion Matrix)
```

---

## 📊 Dataset

* Contains URLs labeled as:

  * **Benign (0)**
  * **Malicious / Defacement (1)**
* Real-world noisy dataset with inconsistent formatting
* Requires preprocessing and cleaning

---

## 🛠️ Tech Stack

### 🧮 Core Technologies

* Python
* Pandas, NumPy

### 🤖 Machine Learning

* Scikit-learn

### 📊 Visualization

* Matplotlib

### 🧪 Development Tools

* Jupyter Notebook
* VS Code

---

## ⚙️ Installation

```bash
# 1. Clone repository
git clone <your-repo-link>
cd malicious-url-detection

# 2. Create virtual environment
python -m venv venv
source venv/bin/activate      # Linux/Mac
venv\Scripts\activate         # Windows

# 3. Install dependencies
pip install -r requirements.txt

# 4. Run the script
python main.py
```

---

## 📁 Project Structure

```
malicious-url-detection/
│
├── main.py                  # Main ML pipeline
├── data/
│   └── benign_vs_defacement_urls.csv
├── models/                  # (optional saved models)
├── requirements.txt
└── README.md
```

---

## 📊 Model Insights

* URL length and digit count strongly influence classification
* Presence of IP address is a strong malicious indicator
* Shortened URLs are often associated with malicious behavior
* Linear SVM provides fast performance with competitive accuracy

---

## 🚀 Future Enhancements

* 🌐 Deploy using FastAPI (real-time API)
* 📊 Build Streamlit dashboard (live URL checker)
* 🧠 Add advanced models (Random Forest, XGBoost)
* 🔍 Integrate NLP-based URL analysis
* 📦 Save/load models for production

---

## 🏁 Conclusion

This project demonstrates a **robust end-to-end ML pipeline** for cybersecurity applications. By combining efficient feature engineering, multiple ML models, and real-world data handling, the system provides a scalable solution for detecting malicious URLs.

It serves as a strong foundation for building **AI-driven security systems** and can be extended into a full production-grade application.

---
