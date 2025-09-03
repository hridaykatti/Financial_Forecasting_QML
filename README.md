# Financial Forecasting Using Quantum Machine Learning

## 📌 Project Overview
This project explores the use of **Quantum Machine Learning (QML)** for **financial forecasting**, focusing on two applications:  
1. **Stock Price Prediction** using a Quantum Long Short-Term Memory (QLSTM) model.  
2. **Credit Card Fraud Detection** using Variational Quantum Circuits (VQC).  

The aim is to evaluate whether quantum-enhanced models can outperform or complement classical machine learning in terms of **pattern recognition, scalability, and efficiency**.

---

## 🛠️ Technologies Used
- **Languages:** Python 3.9+  
- **Libraries/Frameworks:**   
  - PennyLane  
  - TensorFlow/Keras (for hybrid models)  
  - Pandas, NumPy, Matplotlib  
- **Algorithms:**  
  - QLSTM (Quantum Long Short-Term Memory)  
  - VQC (Variational Quantum Circuits with COBYLA optimizer)  

---

## 📂 Repository Structure
```
Financial_Forecasting_QML/
│── stock-price-prediction/ # QLSTM implementation and notebooks
│── credit-card-fraud-detection/ # VQC implementation and notebooks
│── results/ # Training curves, prediction plots, metrics
│── README.md # Project overview (this file)
```
## 📊 Datasets
- **Stock Dataset:** Apple Inc. (AAPL) daily opening and closing stock prices from 2022.  
- **Fraud Dataset:** Public Kaggle dataset on credit card transactions (284,807 rows, ~0.17% fraud cases).  
  - Data balancing and PCA were applied to handle imbalance and reduce dimensionality.  

---

## ⚙️ Methodology
- **Preprocessing:** Exploratory Data Analysis (EDA), balancing, shuffling, PCA, normalization.  
- **Encoding:** Classical data mapped to quantum states using **amplitude encoding** and **rotation encoding**.  
- **QLSTM:** Combines LSTM’s temporal learning with quantum circuits to forecast stock trends.  
- **VQC:** Parameterized quantum circuits trained with **COBYLA optimizer** for fraud detection.  

---

## 📈 Results
- **Stock Price Prediction (QLSTM):**  
  - Training loss reduced to 0.0002, test loss to 0.0001.  
  - Predicted stock price trends closely followed actual Apple stock movements.  

- **Credit Card Fraud Detection (VQC):**  
  - Achieved ~86% accuracy, F1 = 0.86, AUROC = 0.85.  
  - Compared to Random Forest (95% accuracy, F1 = 0.95, AUROC = 0.95).  
  - Shows potential for scalability but highlights current **quantum hardware limitations**.  
