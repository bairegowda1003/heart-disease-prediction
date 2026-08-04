# 🫀 Heart Disease Prediction Web App

A machine learning web application that predicts the likelihood of heart disease in a person based on health parameters such as age, gender, blood pressure, cholesterol level, and more

Built with **Python**, **Flask**, and **KNN (K-Nearest Neighbors)** algorithm — developed as a BCA final project by **Bairegowda**.

---

## 📌 About the Project

This is an end-to-end machine learning project that takes health inputs from the user through a web form and predicts whether the person is at risk of heart disease or not.

The goal was to not just build a model, but to **deploy** it as a real web application that anyone can use — without needing to open a Jupyter notebook.

---

## 🚀 Features

- Predicts heart disease risk based on 13 medical input parameters
- Simple and clean web interface built with HTML/CSS and Flask
- Handles range inputs (e.g., blood pressure entered as `120-130`)
- KNN model trained on the Cleveland Heart Disease dataset

---

## 🧠 How It Works

1. User fills in health details on the web form
2. Flask backend collects the inputs
3. Data is passed to the pre-trained KNN model (`.pkl` file)
4. Model returns a prediction: **Heart Disease Detected** or **No Heart Disease**
5. Result is displayed on the result page

---

## 📁 Project Structure

```
Heart-Disease-Prediction/
│
├── app.py                              # Main Flask application
├── prediction.py                       # Model training script
├── heart-disease-prediction-knn-model.pkl  # Saved KNN model
├── heart_cleveland_upload.csv          # Dataset used for training
├── requirements.txt                    # Python dependencies
├── Procfile                            # For deployment
│
├── templates/
│   ├── main.html                       # Input form page
│   └── result.html                     # Prediction result page
│
└── static/
    └── style.css                       # Styling for the web app
```

---

## 🔢 Input Parameters

| Parameter | Description |
|-----------|-------------|
| Age | Age of the patient |
| Sex | Gender (1 = Male, 0 = Female) |
| CP | Chest pain type (0–3) |
| Trestbps | Resting blood pressure (mm Hg) |
| Chol | Serum cholesterol (mg/dl) |
| FBS | Fasting blood sugar > 120 mg/dl (1 = True, 0 = False) |
| Restecg | Resting ECG results (0–2) |
| Thalach | Maximum heart rate achieved |
| Exang | Exercise induced angina (1 = Yes, 0 = No) |
| Oldpeak | ST depression induced by exercise |
| Slope | Slope of peak exercise ST segment |
| CA | Number of major vessels (0–3) |
| Thal | Thalassemia type (1–3) |

---

## 🛠️ Tech Stack

- **Language:** Python 3.8
- **Framework:** Flask
- **ML Library:** Scikit-learn
- **Algorithm:** K-Nearest Neighbors (KNN)
- **Frontend:** HTML, CSS
- **Dataset:** Cleveland Heart Disease Dataset

---

## ⚙️ Installation & Setup

### 1. Clone the repository

```bash
git clone https://github.com/bairegowda1003/heart-disease-prediction.git
cd heart-disease-prediction
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Run the application

```bash
python app.py
```

Then open your browser and go to: `http://127.0.0.1:5000`

---

## 📊 Dataset

The model is trained on the **Cleveland Heart Disease Dataset** from the UCI Machine Learning Repository.  
It contains 303 records with 13 features and a target variable indicating heart disease presence.

---

## 👨‍💻 Author

**Baire Gowda**  
BCA Graduate  
GitHub: [@bairegowda1003](https://github.com/bairegowda1003)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
