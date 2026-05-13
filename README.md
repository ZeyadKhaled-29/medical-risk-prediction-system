# 🩺 Medical Risk Prediction System

A Machine Learning-powered healthcare application that predicts the risk of multiple chronic diseases based on lifestyle and health-related factors using the BRFSS 2015 dataset.

Built with:

- FastAPI
- Streamlit
- Scikit-learn
- XGBoost

---

# 📌 Project Overview

This project aims to build an intelligent medical risk prediction system that analyzes user lifestyle and health information to estimate the probability of developing:

- Diabetes
- Hypertension
- Heart Disease
- Stroke

The system uses Machine Learning models trained on public health survey data from the BRFSS dataset.

Users enter lifestyle information such as:

- Age
- Height & Weight (BMI calculated automatically)
- Physical activity
- Smoking history
- Fruit & vegetable consumption
- Alcohol habits

The application then predicts disease risk using trained ML models.

---

# 🎥 Demo Video

Add your demo video link here after uploading:

```text
https://youtu.be/3mSPgzuGKpA

````markdown
# 📊 Dataset

Dataset used:

https://www.kaggle.com/datasets/cdc/behavioral-risk-factor-surveillance-system/data?select=2015.csv

⚠️ Important:

The dataset is NOT included in this repository because of its large size.

To run the notebook:

1. Download `2015.csv` from the dataset link above

2. Create a folder named:

```text
dataset/
````

3. Place the CSV file inside it:

```text
dataset/2015.csv
```

---

# 🧠 Notebook Workflow

The notebook contains the complete Machine Learning pipeline.

## 1️⃣ Data Cleaning & Preprocessing

* Selecting relevant medical/lifestyle features
* Handling missing and invalid values
* Feature engineering
* BMI processing
* Lifestyle variable transformation
* Creating binary disease targets

---

## 2️⃣ Exploratory Data Analysis (EDA)

The notebook includes multiple visualizations such as:

* Disease distribution plots
* Correlation heatmaps
* BMI vs disease boxplots
* Smoking & exercise analysis
* ROC curves
* Feature importance charts

These visualizations help understand disease patterns and risk factors.

---

## 3️⃣ Model Training & Selection

Different ML models were tested including:

* Logistic Regression
* Random Forest
* XGBoost

Models were evaluated using:

* Accuracy
* Precision
* Recall
* F1-score
* ROC-AUC

SMOTE was also used to handle class imbalance.

Final models were selected based on:

* Performance
* Interpretability
* Medical explainability

---

# 🏗️ Project Architecture

```text
Streamlit Frontend
        ↓
FastAPI Backend
        ↓
ML Models (.pkl)
        ↓
Prediction Response
```

---

# 📂 Project Structure

```text
DataAnalysisProject/
│
├── backend/
│   ├── app/
│   ├── services/
│   ├── utils/
│   ├── models/
│
├── streamlit_app/
│
├── notebook/
│
├── requirements.txt
│
└── README.md
```

---

# ⚙️ Installation

## 1️⃣ Clone Repository

```bash
git clone <your-repository-link>
cd DataAnalysisProject
```

---

## 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

# 🚀 Running the Application

## ▶️ Run Backend (FastAPI)

```bash
cd backend
python -m uvicorn app.main:app --reload
```

Backend Swagger Documentation:

```text
http://127.0.0.1:8000/docs
```

---

## ▶️ Run Frontend (Streamlit)

Open another terminal:

```bash
python -m streamlit run streamlit_app/app.py
```

Frontend URL:

```text
http://localhost:8501
```

---

# 🧪 Features

✅ Multi-disease prediction system
✅ BMI calculated automatically from height & weight
✅ Interactive Streamlit dashboard
✅ FastAPI REST API backend
✅ Machine Learning model comparison
✅ Data visualization & EDA
✅ Risk probability prediction
✅ Medical dataset preprocessing pipeline

---

# 📈 Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* XGBoost
* FastAPI
* Streamlit

---

# ⚠️ Disclaimer

This project is for educational and research purposes only and should not be considered a medical diagnosis system.

Always consult healthcare professionals for medical advice.

---

# 👨‍💻 Author

Developed by Zeyad Khaled and Mahmoud mansi.

```
```
