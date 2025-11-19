# 🏠 House Price Prediction — Linear Regression

## 📌 Project Overview

This project focuses on predicting house prices using supervised machine learning techniques.
We use  **Linear Regression** as the baseline model.

---

## 📊 Dataset

The dataset contains features such as:

* **SqFt** – Total square feet
* **Bedrooms**
* **Bathrooms**
* **Offers**
* **Neighborhood**
* **Price** — *target variable*

Basic preprocessing steps include:

* Handling missing values
* Removing outliers using IQR
* Feature scaling (optional)
* Train–test splitting

---

## 🔧 Models Used

### 1️⃣ **Linear Regression (Baseline Model)**

* Simple and interpretable model
* Achieved ~**70–79% R²** depending on outlier treatment
* Evaluation metrics used:

  * **MSE**
  * **RMSE**
  * **MAE**
  * **R² Score**


Performance with:
✔ Lower MSE
✔ Lower RMSE
✔ Slightly better MAE
✔ Higher R² Score

---

## 📈 Model Evaluation

Metrics used:

* **Mean Squared Error (MSE)**
* **Root Mean Square Error (RMSE)**
* **Mean Absolute Error (MAE)**
* **R-squared (R² Score)**

These metrics helped compare both models and confirm improvement.

---

## 🧪 Prediction

After training the best model, predictions are generated for new input values such as:

```python
model.predict([[SqFt, Bedrooms, Bathrooms, Offers,Neighborhood]])
```

---

## 🏁 Conclusion

* **Linear Regression** gave a good baseline performance.
* Final model achieved strong prediction accuracy with an R² close to **80%**.
