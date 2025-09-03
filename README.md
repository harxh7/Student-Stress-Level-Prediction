# Student Stress Level Prediction  

[![Python](https://img.shields.io/badge/Python-3.9%2B-blue)]()  
[![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-orange)]()  
[![License](https://img.shields.io/badge/License-MIT-green)]()  

---

## 📖 Overview  

This project explores the prediction of **student stress levels** using machine learning.  
Stress has become one of the most common challenges for students, affecting both **mental health** and **academic performance**.  
By building models on student lifestyle, academic, and social factors, this project aims to answer:  

- Can we **predict stress levels** accurately?  
- Which **factors contribute most** to student stress?  
- How do different models (Logistic Regression, Decision Tree, Random Forest) compare?  

---

## 🎯 Objectives  

- Perform **exploratory analysis** of the dataset.  
- Establish a **baseline model**.  
- Train and evaluate **Logistic Regression, Decision Tree, and Random Forest**.  
- Compare model performance using **accuracy, F1-score, and confusion matrices**.  
- Extract **feature importances** to identify stress drivers.  

---

## 📂 Dataset  

- Contains ~1100 student records.  
- ~20 features covering **health, academics, and lifestyle factors**.  
- Target variable: `stress_level` (categorical).  
- Balanced dataset, no major missing values.  

*(Dataset not included due to licensing. Please replace `student_stress.csv` with your file.)*  

---

## 🛠️ Tech Stack  

- **Language**: Python 3.9+  
- **Libraries**:  
  - pandas, numpy → data handling  
  - matplotlib, seaborn → visualization  
  - scikit-learn → ML models & evaluation  

---

## 🔬 Methodology  

1. **Data Preprocessing**  
   - Split into train/test sets  
   - Standardization for Logistic Regression  
   - No feature selection (Random Forest handles feature weighting internally)  

2. **Models Trained**  
   - Logistic Regression (baseline)  
   - Decision Tree  
   - Random Forest  

3. **Evaluation**  
   - Accuracy & F1-score (CV + test set)  
   - Confusion Matrices  
   - Feature Importances  

---

## 📊 Results  

| Model                | CV Accuracy | CV F1 | Test Accuracy | Test F1 |
|-----------------------|-------------|-------|---------------|---------|
| Logistic Regression  | ~0.84       | ~0.83 | ~0.84         | ~0.83   |
| Decision Tree        | ~0.86       | ~0.85 | ~0.87         | ~0.86   |
| Random Forest        | ~0.88       | ~0.87 | ~0.89         | ~0.88   |

- 📌 **Random Forest performed best**, confirming ensemble methods generalize better.  
- **Key features:** blood pressure, sleep quality, safety, future career concerns.  

---

## 📈 Visuals  

- **Confusion Matrices** → show where models get confused.  
- **Feature Importance Plot** → highlights top stress predictors.  
- **Model Comparison Bar Chart** → quick performance overview.  

---

## ✅ Key Takeaways  

- Stress prediction is feasible with >85% accuracy using standard ML models.  
- **Health and lifestyle factors** (sleep, blood pressure, peer pressure) matter as much as academics.  
- Ensemble models like Random Forest are the most reliable.  

---

## 🚀 Future Work  

- Collect larger and more diverse student samples.  
- Add **temporal data** to track stress changes over time.  
- Build a **real-time monitoring system** (web/app) for early interventions.  

---

## 📜 License  

This project is released under the **MIT License** – you are free to use, modify, and distribute.  

---

## 🤝 Acknowledgments  

- Dataset source: [Kaggle / academic stress datasets] (replace with actual).  
- Inspired by the importance of **student well-being** in education.  
