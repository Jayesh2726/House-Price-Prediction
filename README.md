# 🏠 House Price Prediction — Linear Regression & Random Forest

## 📌 Project Overview

This project focuses on predicting house prices using supervised machine learning techniques.
We start with **Linear Regression** as the baseline model and later improve the model performance using **RandomForestRegressor** and **Grid Search CV** for hyperparameter tuning.

---

## 📊 Dataset

The dataset contains features such as:

* **SqFt** – Total square feet
* **Bedrooms**
* **Bathrooms**
* **Offers**
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

### 2️⃣ **RandomForestRegressor (Improved Model)**

* Handles non-linear relationships
* Reduces overfitting
* Performs feature bagging
* Achieved up to **~79–80% R²**

### 3️⃣ **Grid Search CV (Hyperparameter Tuning)**

Grid Search was applied on Random Forest to optimize parameters such as:

* `n_estimators`
* `max_depth`
* `min_samples_split`
* `min_samples_leaf`

This further improved performance with:
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
model.predict([[SqFt, Bedrooms, Bathrooms, Offers]])
```

---

## 🏁 Conclusion

* **Linear Regression** gave a good baseline performance.
* **RandomForestRegressor** significantly improved accuracy.
* **Grid Search CV** helped fine-tune the model for optimal performance.
* Final model achieved strong prediction accuracy with an R² close to **80%**.
