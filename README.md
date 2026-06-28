# ❤️ Heart Disease Predictor

## Overview

Heart Disease Predictor is a Machine Learning web application built using Streamlit. It predicts whether a person is at risk of heart disease based on various medical parameters entered by the user.

## Features

* User-friendly web interface
* Predicts heart disease risk instantly
* Uses a trained Logistic Regression model
* Data preprocessing with StandardScaler
* Fast and lightweight application

## Technologies Used

* Python
* Streamlit
* Scikit-learn
* Pandas
* NumPy
* Joblib

## Project Structure

```
Heart_Disease_Predictor/
│── app.py
│── logistic_regression_heart.pkl
│── scaler.pkl
│── columns.pkl
│── requirements.txt
│── README.md
```

## Installation

Clone the repository:

```bash
git clone <repository-url>
cd Heart_Disease_Predictor
```

Install the required packages:

```bash
pip install -r requirements.txt
```

Run the application:

```bash
streamlit run app.py
```

## Model

The prediction model is trained using Logistic Regression. Input data is first standardized using StandardScaler before being passed to the trained model.

## Disclaimer

This application is intended for educational and demonstration purposes only. It should not be used as a substitute for professional medical advice or diagnosis.

## Author

Narendra Kharwal
B.Tech CSE (Artificial Intelligence)
SKIT, Jaipur
