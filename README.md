# 🛡️ Intelligent Intrusion Detection System (IDS) using XGBoost and Flask

## 📚 Description

This project aims to develop an **Intelligent Intrusion Detection System (IDS)** using **machine learning** to monitor network traffic and detect malicious activities **in real time**. It uses the **XGBoost** algorithm for fast and accurate classification and integrates a **Flask API** for real-time detection and response.

---

## 🎯 Objectives

- Detect the following attack types:
  - ✅ Denial-of-Service (DoS)
  - ✅ Distributed Denial-of-Service (DDoS)
  - ✅ Brute Force Attacks
  - ✅ Port Scanning
  - ✅ Zero-Day Exploits

- Improve model effectiveness by:
  - 📈 Increasing detection accuracy
  - ❌ Reducing false positives
  - ⚙️ Deploying with minimal computation

---

## ✅ Why This Approach?

| Criteria                | Justification                                                       |
|-------------------------|----------------------------------------------------------------------|
| 🔧 Easy to Implement     | XGBoost is lightweight and powerful with minimal tuning             |
| ⚡ Real-Time Detection   | Flask handles real-time predictions with low latency                |
| 🖥️ Low Hardware Cost     | No GPU required; runs smoothly on personal laptops                  |
| 🧪 Strong Evaluation     | High accuracy, F1-score, and low false-positive rate                |
| 🚀 Resume-Ready Project | Demonstrates end-to-end ML deployment with backend API integration  |

---

## 🛠️ Tools & Technologies

| Purpose              | Tools / Libraries                   |
|----------------------|--------------------------------------|
| Machine Learning     | Python, XGBoost, Scikit-learn        |
| Data Handling        | Pandas, NumPy                        |
| API Development      | Flask                                |
| Visualization        | Matplotlib, Seaborn                  |
| Dataset              | CICIDS 2017 (filtered subset)        |

---

## 🧠 Methodology

1. **Data Preprocessing**
   - Load and filter CICIDS 2017 dataset
   - Encode attack labels (e.g., `DoS`=1, `Normal`=0)
   - Drop duplicates and nulls
   - Feature selection

2. **Model Training**
   - Train-test split (70/30)
   - Train `XGBClassifier`
   - Save model using `joblib`

3. **Flask API for Real-Time Prediction**
   - Load `.pkl` model
   - Accept POST requests with packet features
   - Return prediction (malicious or not)

4. **Simulated Real-Time Input**
   - Script to send rows to the API every few seconds
   - Mimics streaming behavior

5. **Performance Evaluation**
   - Accuracy, precision, recall, F1-score
   - Confusion matrix, classification report


