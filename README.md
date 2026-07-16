# 🛡️ LinkSus – Cloud-Based Machine Learning Phishing Detection System

> **An intelligent phishing detection platform powered by Machine Learning, Explainable AI (SHAP), Google Gemini AI, QR Code (Quishing) Detection, and Cloud Deployment.**

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)
![Flask](https://img.shields.io/badge/Flask-Backend-black?logo=flask)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-orange?logo=scikitlearn)
![Render](https://img.shields.io/badge/Hosted%20on-Render-46E3B7?logo=render)
![License](https://img.shields.io/badge/License-MIT-green)

---

## 📖 Overview

LinkSus is a **Machine Learning-based phishing website detection system** designed to identify malicious URLs in real time.

The application combines **TF-IDF text vectorization**, **custom URL feature engineering**, and a **Linear Support Vector Classifier (LinearSVC)** to accurately classify URLs as **Safe** or **Phishing**.

Unlike traditional phishing detectors, LinkSus enhances user trust by providing:

- 🧠 Explainable AI using SHAP
- 🤖 Human-readable explanations using Google Gemini AI
- 📱 QR Code (Quishing) Detection
- 🌐 Chrome Extension for real-time URL analysis
- ☁️ Cloud deployment using Render

---

# 🚀 Features

- 🔍 Real-time phishing URL detection
- 🤖 Machine Learning classification using LinearSVC
- 📊 Explainable AI (SHAP)
- 💬 AI-generated security explanations using Google Gemini
- 📱 QR Code (Quishing) Scanner
- 🌍 Chrome Browser Extension
- 🎯 TF-IDF based URL analysis
- 🔐 Custom URL feature engineering
- ☁️ Hosted on Render Cloud
- 📈 Fast prediction with high accuracy

---

# 🏗️ System Architecture

```
            +----------------+
            |     User       |
            +-------+--------+
                    |
                Enter URL /
                Scan QR Code
                    |
                    v
          +----------------------+
          |   Flask Web App      |
          +----------+-----------+
                     |
        URL Cleaning & Preprocessing
                     |
                     v
        Feature Extraction Module
    (TF-IDF + 19 URL Features)
                     |
                     v
      LinearSVC ML Model
                     |
         +-----------+-----------+
         |                       |
         v                       v
 SHAP Explanation         Gemini AI Explanation
         |                       |
         +-----------+-----------+
                     |
                     v
        Safe / Phishing Prediction
                     |
                     v
                  User


```

---

# 🧠 Machine Learning Pipeline

Dataset
↓
Cleaning URLs
↓
TF-IDF Vectorization
↓
Custom URL Feature Extraction
↓
Feature Scaling
↓
Feature Combination
↓
LinearSVC Training
↓
Prediction
↓
SHAP Explanation
↓
Gemini AI Explanation

---

# ⚙️ Technologies Used

## Programming Languages

- Python
- HTML5
- CSS3
- JavaScript

## Backend

- Flask

## Machine Learning

- Scikit-Learn
- LinearSVC
- TF-IDF Vectorizer
- StandardScaler

## Libraries

- NumPy
- Pandas
- SciPy
- SHAP
- Google GenAI
- Python Dotenv

## Cloud

- Render

## Version Control

- Git
- GitHub

---

# 📊 Dataset

- Balanced Dataset
- 60,000 URLs
- 30,000 Safe URLs
- 30,000 Phishing URLs

Source:
Kaggle Phishing Website Dataset

---

# 🔬 Feature Engineering

The model combines:

## TF-IDF Features

- 3000 text-based features

## Custom URL Features (19)

Examples include:

- URL Length
- Number of Dots
- Number of Hyphens
- Number of Digits
- Login Keyword
- Verify Keyword
- Secure Keyword
- Account Keyword
- Update Keyword
- Suspicious TLD Detection
- Look-alike Domain Detection
- Scam Keyword Count
- Semantic Phishing Phrase Detection

---

# 📈 Model Performance

| Metric | Score |
|---------|-------|
| Algorithm | LinearSVC |
| Accuracy | ~92% |
| Features | TF-IDF + 19 URL Features |

---

# 💡 Explainable AI

The project integrates **SHAP (SHapley Additive Explanations)** to explain why a URL is classified as phishing or safe.

This increases transparency by highlighting which URL features contributed most to the prediction.

---

# 🤖 Google Gemini AI

After prediction, Google Gemini generates a human-readable explanation describing why the URL is considered safe or suspicious.

This helps users better understand phishing threats instead of receiving only a binary prediction.

---

# 📱 QR Code (Quishing) Detection

Users can upload or scan QR codes.

The system extracts the embedded URL and automatically performs phishing analysis using the trained machine learning model.

---

# 🌍 Chrome Extension

The project includes a browser extension that:

- Detects phishing URLs
- Connects to the Flask backend
- Displays prediction results instantly

---

# ☁️ Cloud Deployment

The application is deployed on **Render Cloud Platform**, enabling secure HTTPS access and automatic deployments through GitHub integration.

---

# 📂 Project Structure

```
LinkSus
│
├── app.py
├── requirements.txt
├── phishing_modelnew.pkl
├── vectorizernew.pkl
├── scalernew.pkl
│
├── templates/
│     └── index.html
│
├── extension/
│
├── dataset/
│
└── README.md
```

---

# ▶️ Installation

Clone the repository

```bash
git clone https://github.com/yourusername/LinkSus.git
```

Move into the project

```bash
cd LinkSus
```

Install dependencies

```bash
pip install -r requirements.txt
```

Run the application

```bash
python app.py
```

Open

```
http://127.0.0.1:5000
```

---

# 🎯 Future Enhancements

- Deep Learning (LSTM / Transformers)
- DNS Reputation Analysis
- SSL Certificate Verification
- Browser Sandboxing
- Crowdsourced Threat Intelligence
- Mobile Application
- Continuous Model Retraining

---

# 👨‍💻 Developed By

**Jayanth S**

Bachelor of Computer Applications (BCA)

---

# ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub!
