## 🦠 Cholera Outbreak Predictor

This project uses a machine learning approach to predict cholera outbreaks in Nigeria based on historical data. It supports early public health response and improves decision-making for outbreak prevention and control.

---

## 📌 Project Overview

Cholera remains a recurring public health threat in Nigeria. Using supervised learning techniques, this project classifies weekly state-level reports as either an outbreak or no outbreak, based on reported suspected cases and deaths.

The project includes:

Data preprocessing

Exploratory Data Analysis (EDA)

Model training and evaluation

Threshold tuning to improve recall

saving the final model for future reuse

---

## 📁 Project Structure
-cholera-outbreak-predictor/
+cholera-outbreak-predictor/

 │
 
 ├── data/
 
 │   └── cholera_dataset.csv  # Raw dataset
 
 │
 
 ├── models/
 
 │   └── cholera_model.pkl    # Trained ML model
 
 │
 
 ├── notebooks/
 
 │   └── Cholera_Prediction_Model.ipynb  # Full code and analysis
 
 │
 
 └── README.md  # Project documentation


## 📊 Dataset

The dataset contains cholera surveillance reports with:
- State
- Week
- Number of suspected cases
- Number of deaths
- Label (0 = No Outbreak, 1 = Outbreak)

**Note:** The dataset is small and imbalanced, which influenced model performance and required threshold adjustments.

---

## 🧠 Model Summary

A classification model was trained to identify outbreak patterns.
Key steps include:
- Handling class imbalance
- Performance evaluation using precision, recall, F1-score
- Custom threshold tuning to improve recall without sacrificing precision

### ✅ Final Performance:

| Metric        | Value |
|---------------|--------|
| Accuracy      | 93%    |
| Precision (1) | 1.00   |
| Recall (1)    | 0.50   |
| F1-score (1)  | 0.67   |

The model is highly accurate for 'No Outbreak' cases and demonstrates high precision when it predicts an outbreak.

---

## 🚀 How to Run

1. **Clone the repository:**
```bash
git clone https://github.com/Ukayria/cholera-outbreak-predictor.git
Open the notebook:

2. Navigate to notebooks/Cholera_Prediction_Model.ipynb

Run it in Jupyter Notebook or Google Colab

3. Load the model:

import joblib
model = joblib.load('models/cholera_model.pkl')

🛠 Requirements

Install dependencies with:
```bash
pip install pandas scikit-learn matplotlib seaborn imbalanced-learn


📌 Notes
The model performs well but was trained on a small dataset, so further validation is needed for production use.

More data and feature engineering would improve generalizability and detection accuracy.

🤝 Contributions
Want to improve the model, try other ML algorithms, or automate weekly predictions?
Fork the repo and submit a pull request.




