# 🩺 Diabetes Prediction

This project is a **machine learning model** that predicts whether a person has diabetes based on health-related features such as glucose levels, blood pressure, BMI, age, etc. It explores multiple algorithms and compares their performance, with **Logistic Regression** performing best overall.

---

## 📂 Project Structure

* `diabetes.csv` → Dataset containing patient health records.
* `diabetes_prediction.ipynb` → Jupyter notebook with preprocessing, training, and evaluation.
* `model.pkl` → Trained Logistic Regression model (saved for deployment).
* `app.py` → Flask backend to serve predictions.
* `index.html` → Frontend interface for entering patient data.

---

## 📊 Workflow

1. **Data Preprocessing**

   * Handled missing/zero values.
   * Applied feature scaling.
   * Checked correlations among features.

2. **Model Training**
   * Algorithms tested:
     * Logistic Regression ✅ (Best Accuracy \~76%)
     * Support Vector Classifier (SVC)
     * K-Nearest Neighbors (KNN)
     * Decision Tree
     * Random Forest
   * Train-test split: 80% training, 20% testing.

3. **Model Evaluation**

   * Accuracy Score
   * Confusion Matrix
   * Precision, Recall, F1-score

---

## 📈 Visual Insights

### 🔍 Correlation Heatmap

```
[ Feature correlation heatmap between glucose, BMI, age, etc. ]
```

### 📊 Class Distribution

```
[ Bar chart showing number of diabetic vs non-diabetic patients ]
```

### 🧪 Model Comparison

```
[ Bar chart comparing accuracy of Logistic Regression, SVC, KNN, Decision Tree, Random Forest ]
```

---

## 🚀 Deployment

1. Run Flask App:

```bash
python app.py
```

2. Open `http://127.0.0.1:5000/` in browser.

3. Enter patient details (glucose, BMI, age, etc.) → Get prediction instantly.

---

## ✅ Example Prediction

| Glucose | BMI  | Age | Prediction     |
| ------- | ---- | --- | -------------- |
| 148     | 33.6 | 50  | Diabetic ⚠️    |
| 95      | 26.1 | 29  | Non-Diabetic ✅ |

---

## 🔮 Future Improvements

* Test advanced models (XGBoost, Neural Networks).
* Add feature importance visualization.
* Deploy on **Heroku / Render / AWS**.
* Build a mobile-friendly interface.

## 📌 Conclusion

This project demonstrates how **machine learning** can be applied in the medical domain to assist with early diabetes prediction. With proper deployment, it can be used as a **decision-support tool** for healthcare professionals and patients.
