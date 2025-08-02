# 🩺 Medicine Recommendation System

A smart, AI-powered web application that predicts diseases based on user-entered symptoms and provides helpful recommendations like medicines, diet plans, precautions, and workouts. The system uses a machine learning model trained on medical datasets and is served through a Flask-based web interface.

---

## 🚀 Features

- ✅ Enter symptoms to get an AI-predicted disease
- 💊 Get recommended medications for the predicted disease
- 🥗 Get diet suggestions and workout plans
- 📋 See medical precautions and descriptions
- 🧠 ML-powered with text correction and validation
- ⚡ Real-time symptom autocomplete using AJAX
- 🔐 Input sanitization (prevents XSS via `bleach`)

---

## 🛠️ Tech Stack

| Layer       | Tools/Libraries                      |
|-------------|--------------------------------------|
| Language    | Python 3.x                           |
| Backend     | Flask, Scikit-learn, TextBlob        |
| Frontend    | HTML, CSS, Bootstrap, Jinja2         |
| ML Model    | Support Vector Classifier (SVC)      |
| NLP         | TextBlob (spelling correction)       |
| Sanitizer   | bleach (XSS protection)              |
| Data Format | CSV files for training and metadata  |

---
medicine-recommendation-system/
│
├── Datasets/
│ ├── symtoms_df.csv
│ ├── precautions_df.csv
│ ├── workout_df.csv
│ ├── description.csv
│ ├── medications.csv
│ └── diets.csv
│
├── Models/
│ └── svc.pkl
│
├── templates/
│ ├── index.html
│ ├── home.html
│ ├── landing_page.html
│ ├── about.html
│ ├── contact.html
│ └── getstart.html
│
├── static/
│ └── (optional: CSS/JS/images)
│
├── app.py
├── requirements.txt
└── README.md


---

## 📦 Installation

### 🔧 1. Clone the Repository

```bash
git clone https://github.com/Viishhnuvardhunreddy-12/medicine-recommendation-system.git
cd medicine-recommendation-system

▶️ How to Run
python main.py

✅ Sample Symptoms to Test
itching, vomiting, fatigue
headache, cough, chills
skin_rash, nausea, sweating

🧠 Machine Learning
Model: Support Vector Classifier (SVC)
Input: Binary vector for 132 symptoms

Output: Disease name
Trained on a custom symptom-disease dataset
Uses real-time symptom correction (TextBlob)

🔐 Input Sanitization
User inputs are sanitized using bleach to prevent XSS or code injection.
TextBlob is used to auto-correct minor typos in symptoms.

🌐 APIs
/autocomplete?query= – Returns matching symptoms for live search
/predict – Accepts symptoms and returns predictions + recommendations

📋 Requirements.txt
You can create a requirements.txt file with the following content:
Flask==2.2.5
pandas==2.0.3
numpy==1.25.0
scikit-learn==1.3.0
textblob==0.17.1
bleach==6.1.0

To generate it manually from your environment:
pip freeze > requirements.txt
📌 Future Enhancements
🌍 Deploy the app on Render, Railway, or Heroku
🎙️ Add voice-based symptom input
📱 Convert to mobile-friendly PWA
🔗 Connect with real-time drug APIs

👨‍💻 Author
Viishhnuvardhunreddy-12
📧 viishhnureddy@gmail.com
## 📁 Directory Structure

