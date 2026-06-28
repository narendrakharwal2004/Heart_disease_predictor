# ❤️ Heart Disease Predictor

![Python](https://img.shields.io/badge/Python-3.8+-blue?style=flat&logo=python)
![Streamlit](https://img.shields.io/badge/Streamlit-Deployed-FF4B4B?style=flat&logo=streamlit)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-orange?style=flat&logo=scikit-learn)
![Accuracy](https://img.shields.io/badge/Accuracy-86.14%25-brightgreen?style=flat)
![F1 Score](https://img.shields.io/badge/F1%20Score-87.72%25-brightgreen?style=flat)
![License](https://img.shields.io/badge/License-MIT-yellow?style=flat)

A Machine Learning web application that predicts heart disease risk based on clinical parameters — built with Python, Scikit-learn, and Streamlit.

🔗 **Live Demo:** [heartdiseasepredictor-nk.streamlit.app](https://heartdiseasepredictor-nk.streamlit.app/)

---

## 📸 Screenshots

| High Risk Prediction | Low Risk Prediction |
|---|---|
| ![High Risk](screenshots/high_risk.png) | ![Low Risk](screenshots/low_risk.png) |

> *(Add your screenshots to a `/screenshots` folder in the repo)*

---

## 🧠 About the Project

Heart disease is the **#1 cause of death globally**. Early detection can save lives. This project uses a **Logistic Regression** model trained on the UCI Heart Disease dataset to predict whether a patient is at **High Risk ⚠️** or **Low Risk ✅** of heart disease based on 11 clinical features.

### 🎯 Model Performance

| Metric | Score |
|--------|-------|
| Algorithm | Logistic Regression |
| Accuracy | **86.14%** |
| F1 Score | **87.72%** |

> The model was optimized for **F1 Score** rather than just accuracy — because in medical predictions, minimizing false negatives is critical.

---

## ✨ Features

- ⚡ Real-time heart disease risk prediction
- 🎛️ Interactive UI with sliders and dropdowns for clinical inputs
- 🔄 Automatic feature encoding and scaling pipeline
- 📊 Trained on the UCI Heart Disease dataset
- 🌐 Deployed live on Streamlit Cloud

---

## 🩺 Input Parameters

| Parameter | Description |
|-----------|-------------|
| Age | Patient age (18–100) |
| Sex | Male / Female |
| Chest Pain Type | ATA / NAP / TA / ASY |
| Resting Blood Pressure | mm Hg (80–200) |
| Cholesterol | mg/dL (100–600) |
| Fasting Blood Sugar | > 120 mg/dL (0 or 1) |
| Resting ECG | Normal / ST / LVH |
| Max Heart Rate | bpm (60–220) |
| Exercise-Induced Angina | Yes / No |
| Oldpeak (ST Depression) | 0.0 – 6.0 |
| ST Slope | Up / Flat / Down |

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Language | Python 3.8+ |
| ML Framework | Scikit-learn |
| Web App | Streamlit |
| Data Processing | Pandas, NumPy |
| Model Persistence | Joblib |

---

## 📁 Project Structure

```
Heart_Disease_Predictor/
│── app.py                        # Main Streamlit application
│── logistic_regression.pkl       # Trained Logistic Regression model
│── scaler.pkl                    # Fitted StandardScaler
│── columns.pkl                   # Expected feature columns
│── requirements.txt              # Python dependencies
│── README.md                     # Project documentation
```

---

## ⚙️ How It Works

```
User Input  →  One-Hot Encoding  →  StandardScaler  →  Logistic Regression  →  Risk Prediction
```

1. User fills in 11 clinical parameters via the web UI
2. Categorical features are one-hot encoded to match training format
3. All features are scaled using the saved `StandardScaler`
4. The trained `LogisticRegression` model outputs a binary prediction
5. Result is displayed as **High Risk ⚠️** or **Low Risk ✅**

---

## 🚀 Run Locally

**1. Clone the repository**
```bash
git clone https://github.com/narendrakharwal2004/Heart_disease_predictor.git
cd Heart_disease_predictor
```

**2. Install dependencies**
```bash
pip install -r requirements.txt
```

**3. Run the app**
```bash
streamlit run app.py
```

The app will open at `http://localhost:8501`

---

## 📦 Requirements

```
streamlit
scikit-learn
pandas
numpy
joblib
```

---

## ⚠️ Disclaimer

This application is built for **educational and demonstration purposes only**. It is not a substitute for professional medical advice, diagnosis, or treatment. Always consult a qualified healthcare provider for medical decisions.

---

## 👨‍💻 Author

**Narendra Kharwal**
B.Tech CSE (Artificial Intelligence) — SKIT, Jaipur

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat&logo=linkedin)](https://www.linkedin.com/in/narendrakharwal)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-black?style=flat&logo=github)](https://github.com/narendrakharwal2004)

---

⭐ **If you found this project helpful, please give it a star!** It keeps me motivated to build more. 🚀
