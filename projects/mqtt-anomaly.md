---
layout: default
permalink: /projects/mqtt-anomaly/
---

# 📡 AI-Based Anomaly Detection in MQTT Data Streams

A deep learning project developed to detect cybersecurity anomalies in IoT-based sensor data using time-series modeling and ensemble methods.

---

## 📄 Project Materials


#### 📘 View or Run Notebooks

- **RNN & FNN Code Notebook**  
  🔗 [View on GitHub](https://github.com/SebasFelipeRA/sebastianriveraportfolio/blob/main/assets/projects/SEP_769_Final_Project_Code_FINAL_Group7_RNNandFNN.ipynb)  
  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/SebasFelipeRA/sebastianriveraportfolio/blob/main/assets/projects/SEP_769_Final_Project_Code_FINAL_Group7_RNNandFNN.ipynb)

---

- **Preprocessing & Visualization Notebook**  
  🔗 [View on GitHub](https://github.com/SebasFelipeRA/sebastianriveraportfolio/blob/main/assets/projects/SEP%20769%20Preprocessing%20Data%20Final%20Project%20Visulization.ipynb)  
  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/SebasFelipeRA/sebastianriveraportfolio/blob/main/assets/projects/SEP%20769%20Preprocessing%20Data%20Final%20Project%20Visulization.ipynb)

---

#### 📄 Additional Project File

- [📄 Anomaly Detection Instructions (TXT)](https://github.com/SebasFelipeRA/sebastianriveraportfolio/blob/main/assets/projects/SEP%20769%20Anomoly%20detection%20instructions.txt)

---

## Overview

This project tackled the detection of **duplication**, **interception**, and **modification** attacks in MQTT data streams — common vulnerabilities in connected industrial systems. Using the DAD (Dataset for Anomaly Detection), we implemented and evaluated multiple anomaly detection models, with a primary focus on **LSTM networks** due to their strength in modeling temporal dependencies.

An ensemble strategy combining **LSTM**, **Random Forest**, and **Isolation Forest** was used to boost classification performance via **majority voting**.

---

## Key Features

- 🧠 LSTM RNN for time-series anomaly prediction  
- 🏗️ Majority voting ensemble of LSTM, Random Forest, and Isolation Forest  
- 📦 Preprocessing includes one-hot encoding, normalization, and SMOTE oversampling  
- 📊 ROC-AUC scores ~0.99 on unseen test data  
- 🛡️ Detected cybersecurity anomalies across 7-day MQTT traffic samples  

---

## 🛠️ Engineering Breakdown

### 🔍 Models & Dataset
- **Dataset**: [DAD - Dataset for Anomaly Detection](https://github.com/dad-repository/dad)  
- **Features used**: `ip.src`, `tcp.srcport`, `mqtt.clientid`, `mqtt.msgid`, and `label`  
- **Models implemented**:
  - LSTM with dropout layers
  - Random Forest (GridSearchCV tuned)
  - Isolation Forest
  - Feedforward Neural Network (FNN)
  - XGBoost

### 🧪 Training Strategy
- Data split: 60% Train / 20% Validation / 20% Test  
- Used **SMOTE** to balance classes  
- Trained for **100 epochs** with **early stopping**  
- Predictions consolidated via **majority voting**

### 📈 Performance Metrics
- **LSTM ROC-AUC**: 0.986 (test)  
- **FNN ROC-AUC**: 0.995 (test)  
- **Ensemble ROC-AUC**: 0.999 (train), 0.995 (validation)  
- Excellent **precision**, **recall**, and **F1-score** observed

---

## 💡 Skills Applied

- Deep Learning: LSTM, FNN, XGBoost  
- Ensemble Learning & Majority Voting  
- Cybersecurity anomaly detection  
- Feature encoding & time-series normalization  
- Python, Keras, scikit-learn, pandas, matplotlib

---

## 🔮 Future Enhancements

- Integrate model into a **real-time system**
- Test in cross-domain settings like healthcare or automotive  
- Improve adversarial robustness  
- Explore hybrid models (e.g., autoencoders + attention mechanisms)

---

### 📍 Project Year: 2024  
---

> _"This project taught me how to design resilient deep learning systems capable of detecting subtle yet critical anomalies in real-world, time-sensitive environments."_
