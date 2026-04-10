Intelligent Fraud Detection & KYC Verification System

This project is based on a real-world problem in banking and financial systems — detecting fraud while also verifying user identity.
The main idea was to build a complete pipeline that not only detects suspicious transactions but also ensures that the user behind the transaction is genuine.

Project Overview

In this project, I have combined multiple machine learning techniques to create a system that can:
 Detect fraudulent transactions 
 Identify unusual behaviour using anomaly detection
 Segment customers based on their risk level
 Verify identity using OCR-based KYC

Instead of relying on a single model, the system uses a combination of approaches to make better decisions.

How the System Works
The system follows a step-by-step pipeline:

1. KYC Verification
   The user uploads an ID document, and OCR is used to extract details like name and ID number.
2. Fraud Detection (Supervised ML)
   Models like Logistic Regression, Random Forest, and XGBoost are used to predict fraud probability.
3. Anomaly Detection
   Isolation Forest is used to detect unusual or unseen fraud patterns.
4. Customer Segmentation
   K-Means clustering is used to group customers based on risk.
5. Final Decision System
   All outputs are combined into a single risk score, and the system decides whether to approve, monitor, or flag the transaction.

Models Used
Logistic Regression (baseline)
Random Forest
XGBoost (final model)
Isolation Forest (for anomaly detection)
K-Means (for segmentation)

Key Features
Handles highly imbalanced data using SMOTE
Detects both known and unknown fraud patterns
Combines multiple models for better accuracy
Includes KYC verification using OCR
Provides a final risk score for decision making

 Results
Achieved high accuracy and strong AUC score (~0.98)
Successfully detected most fraud cases
Reduced unnecessary alerts
System can be extended for real-time use

Tech Stack -Python, Pandas, NumPy ,Scikit-learn ,XGBoost ,Imbalanced-learn ,OpenCV, Tesseract OCR

How to Run
1. Install required libraries:pip install -r requirements.txt
2. Open the notebook:jupyter notebook
3. Run all cells step by step

Future Improvements
Real-time deployment using APIs
Deep learning models like LSTM
Face verification for stronger KYC
Continuous model training

About Me
This project was developed as part of my MSc Data Science work.
It reflects my interest in solving real-world problems using machine learning and building practical systems.
⭐ If you found this useful, feel free to star the repo!
