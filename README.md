# Mental_Health_Score
 # 🌿 MindPulse — Student Wellness Analytics Dashboard

> An end-to-end Machine Learning web application that analyzes students' lifestyle and digital habits to generate a personalized **Wellness Score (0–10)** through an interactive analytics dashboard.

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)
![FastAPI](https://img.shields.io/badge/FastAPI-Backend-009688?logo=fastapi)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-orange?logo=scikitlearn)
![Render](https://img.shields.io/badge/Deploy-Render-46E3B7?logo=render)
![License](https://img.shields.io/badge/License-MIT-green)

---

## 📖 Overview

**MindPulse** is a Student Wellness Analytics Dashboard built using **Machine Learning** and **FastAPI**. The application evaluates everyday lifestyle factors such as screen time, sleep, study hours, physical activity, stress level, and social media usage to generate a personalized wellness score.

The objective of this project is to promote **wellness awareness** through data-driven insights while providing a modern and responsive user experience.

> **Disclaimer:** MindPulse is designed for educational and informational purposes only. It is **not** a medical or clinical diagnosis tool.

---

## ✨ Features

- 📊 Personalized Wellness Score (0–10)
- 😴 Sleep, Stress, and Study Habit Analysis
- 📱 Digital Habit & Screen Time Insights
- 💪 Physical Activity Evaluation
- 🌐 Responsive and Interactive Dashboard
- ⚡ Real-time Prediction using FastAPI
- 📈 Machine Learning Powered Backend
- 🌿 Educational Wellness Insights with Disclaimer

---

## 🖥️ Live Demo

🔗 **Live Application**

https://mental-health-score-538o.onrender.com

---

## 🏗️ Project Architecture

```text
                 User Input
                      │
                      ▼
         Lifestyle & Digital Habit Form
                      │
                      ▼
              FastAPI Backend API
                      │
                      ▼
      Data Preprocessing & Feature Encoding
                      │
                      ▼
        Trained Machine Learning Model
                      │
                      ▼
      Wellness Score Prediction (0–10)
                      │
                      ▼
      Interactive Analytics Dashboard
```

---

## 🛠️ Tech Stack

### Frontend

- HTML5
- CSS3
- JavaScript
- Responsive UI Design

### Backend

- FastAPI
- Uvicorn

### Machine Learning

- Python
- Scikit-learn
- Pandas
- NumPy
- Joblib

### Deployment

- Render

---

## 🤖 Machine Learning Workflow

1. Data Collection
2. Data Cleaning & Preprocessing
3. Feature Encoding
4. Model Training
5. Model Evaluation
6. Model Serialization (`joblib`)
7. FastAPI Integration
8. Web Deployment

---

## 📊 Input Parameters

The model predicts wellness score using multiple lifestyle attributes.

| Feature | Description |
|---------|-------------|
| Study Hours | Average daily study hours |
| Sleep Hours | Average sleep duration |
| Screen Time | Daily mobile/laptop screen time |
| Stress Level | Self-perceived stress level |
| Physical Activity | Daily exercise/activity duration |
| Social Media Usage | Most-used platform and purpose |
| Daily Phone Unlocks | Approximate unlock frequency |
| Academic & Lifestyle Habits | Additional behavioral inputs |

---

## 🎯 Output

The application generates:

- ✅ Wellness Score (0–10)
- 📈 Personalized Wellness Insight
- 🌿 Visual Wellness Indicator
- 💡 Educational Wellness Recommendation

---

## ⚙️ Installation & Setup

### 1️⃣ Clone Repository

```bash
git clone https://github.com/DG-Modi/MindPulse.git
cd MindPulse
```

### 2️⃣ Create Virtual Environment

```bash
python -m venv venv
```

Activate environment.

**Windows**

```bash
venv\Scripts\activate
```

**Mac/Linux**

```bash
source venv/bin/activate
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 4️⃣ Run FastAPI Server

```bash
uvicorn main:app --reload
```

Backend runs at:

```text
http://127.0.0.1:8000
```

### 5️⃣ Open Frontend

Open `index.html` in your browser or serve it locally.

---

## 📂 Project Structure

```text
MindPulse/
│
├── backend/
│   ├── main.py                 # FastAPI application
│   ├── model.pkl               # Trained ML model
│   ├── encoder.pkl             # Encoders
│   ├── scaler.pkl              # Feature scaler
│   └── requirements.txt
│
├── frontend/
│   ├── index.html
│   ├── style.css
│   ├── script.js
│   └── assets/
│
├── dataset/
│   └── student_wellness_dataset.csv
│
├── notebook/
│   └── model_training.ipynb
│
├── screenshots/
│
├── README.md
└── LICENSE
```

---

## 📊 Dataset

This project uses a student wellness dataset containing behavioral and lifestyle information for machine learning prediction.

The dataset includes features related to:

- Sleep patterns
- Screen time
- Study hours
- Physical activity
- Stress level
- Social media usage
- Digital habits

**Dataset Source:** Kaggle Student Wellness Dataset.

> Please download the dataset separately from Kaggle before training the model.

---

## 🚀 API Endpoint

### Predict Wellness Score

**POST** `/predict`

Example Request

```json
{
  "study_hours": 6,
  "sleep_hours": 7,
  "screen_time": 5,
  "stress_level": 6,
  "physical_activity": 45,
  "daily_unlocks": 80,
  "social_media": "Instagram"
}
```

Example Response

```json
{
  "wellness_score": 8.2,
  "status": "Good Wellness"
}
```

---

## 💡 What I Learned

This project helped me improve my skills in:

- Machine Learning model development.
- Feature engineering and preprocessing.
- REST API development using FastAPI.
- Frontend and backend integration.
- Deploying ML applications on Render.
- Building responsive analytics dashboards.

---

## 🔮 Future Improvements

- User Authentication
- Wellness History Tracking
- Interactive Charts & Trends
- Personalized Habit Recommendations
- AI Chat-based Wellness Assistant
- Multi-language Support

---

## 🤝 Contributing

Contributions, suggestions, and improvements are welcome.

1. Fork the repository.
2. Create a new feature branch.
3. Commit your changes.
4. Open a Pull Request.

---

## 📜 License

This project is licensed under the **MIT License**.

---

## 👨‍💻 Author

**Dev Modi**

Computer Engineering Student | Data Analytics & Machine Learning Enthusiast

- GitHub: https://github.com/DG-Modi
- LinkedIn: www.linkedin.com/in/dev-modi-67a639341/

---
