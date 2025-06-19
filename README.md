# 🏥 Medical Recommendation System

A Machine Learning-powered Flask web application that predicts diseases based on user-inputted symptoms and provides detailed medical recommendations including descriptions, medications, precautions, diets, and workouts.

---

## 📌 Project Overview

This Medical Recommendation System helps users identify potential diseases based on their symptoms using a trained Support Vector Classifier (SVC). It then provides:
- Disease Description
- Recommended Medications
- Necessary Precautions
- Dietary Suggestions
- Suggested Workouts

This platform is designed to aid early awareness and provide general health guidance. **It is not a replacement for professional medical consultation.**

---

## ✨ Key Features

- 🧠 **Disease Prediction** using ML models trained on symptoms
- 📋 **Multiple Symptoms Input** through user-friendly UI
- 💊 **Medication Recommendations**
- 🥗 **Diet & Lifestyle Advice**
- 🏃 **Workout Suggestions**
- 📚 **Information-rich pages**: About, Contact, Developer, Blog

---

## 🔍 Sample Models Used for Benchmarking

The following models were tested during development:

| Model             | Accuracy Score |
|------------------|----------------|
| Support Vector Classifier (SVC)   | ✅ Best performing |
| Random Forest Classifier          | Moderate |
| Gradient Boosting Classifier      | Moderate |
| K-Nearest Neighbors (KNN)         | Basic |
| Multinomial Naive Bayes           | Low (Due to numeric input features) |

### 📊 Evaluation Metrics:
- `Accuracy Score`
- `Confusion Matrix`

```python
models = {
    'SVC': SVC(kernel='linear'),
    'RandomForest': RandomForestClassifier(n_estimators=100, random_state=42),
    'GradientBoosting': GradientBoostingClassifier(n_estimators=100, random_state=42),
    'KNeighbors': KNeighborsClassifier(n_neighbors=5),
    'MultinomialNB': MultinomialNB()
}

🧠 Model Used

Algorithm: Support Vector Classifier (SVC)

Input: Binary vector based on 132 symptoms

Output: One of 41 diseases from the predefined list

Training: Symptoms-to-disease mapping dataset

📁 Project Structure

├── app.py                     # Main Flask Application
├── templates/
│   ├── index.html
│   ├── about.html
│   ├── contact.html
│   ├── developer.html
│   └── blog.html
├── models/
│   └── svc.pkl                # Trained SVC model
├── datasets/
│   ├── symptoms_df.csv
│   ├── precautions_df.csv
│   ├── medications.csv
│   ├── diets.csv
│   └── workout_df.csv
├── static/                    # CSS/JS/Assets (optional)
└── README.md

Run the Flask application

python app.py

Open your browser at: http://127.0.0.1:5000

📜 Disclaimer
This project is for educational purposes only. It is not a substitute for professional medical advice, diagnosis, or treatment.

👨‍💻 Developer
Balaji D Bam
B.Sc Artificial Intelligence & Machine Learning