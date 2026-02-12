# Fire Weather Index (FWI) Prediction Web Application

## Overview

This project is a Machine Learning web application built using Flask that predicts the Fire Weather Index (FWI) based on meteorological parameters.

The application integrates a trained Ridge Regression model with a web interface to provide real-time predictions.

---

---

## 🎥 Demo Video

Watch the complete project demonstration below:



https://github.com/user-attachments/assets/5c7e6b59-8b5e-491f-89ca-53f91065459b






## Tech Stack

- Python
- Flask
- Scikit-learn
- NumPy
- Pandas
- HTML

---

## Machine Learning Details

- Algorithm: Ridge Regression
- Feature Scaling: StandardScaler
- Model File: models/ridge.pkl
- Scaler File: models/scaler.pkl
- Framework: Scikit-learn

The model is serialized using pickle and loaded into the Flask application for prediction.

---

## Input Features

The application accepts the following parameters:

- Temperature
- Relative Humidity (RH)
- Wind Speed (Ws)
- Rain
- FFMC
- DMC
- ISI
- Classes
- Region

---

## Project Structure

FWI-Prediction-App/
│
├── app.py
├── models/
│   ├── ridge.pkl
│   └── scaler.pkl
│
├── templates/
│   ├── index.html
│   └── home.html
│
├── requirements.txt
└── README.md

---

## Installation

### Clone Repository

git clone https://github.com/your-username/FWI-Prediction-App.git  
cd FWI-Prediction-App

### Create Virtual Environment (Optional)

python -m venv venv  

Activate (Windows):

venv\Scripts\activate  

### Install Dependencies

pip install -r requirements.txt  

If requirements.txt is not available:

pip install flask numpy pandas scikit-learn  

---

## Run the Application

python app.py  

Application will run at:

http://127.0.0.1:5000/

---

## How It Works

1. User enters environmental data in the form.
2. Flask receives the POST request.
3. Input data is converted to float values.
4. Data is scaled using StandardScaler.
5. Ridge Regression model predicts the FWI value.
6. Result is displayed on the webpage.

---


