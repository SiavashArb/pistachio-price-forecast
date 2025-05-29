# Pistachio Price Prediction using Machine Learning

📈 This project builds and compares multiple regression models to predict pistachio prices based on features such as kernel percentage, size, shell percentage, and type. It also provides model evaluation, feature importance, and an example of forecasting price for new input data.

---

## 🧾 Dataset

- **Source:** Local file `Book1.csv`
- **Target variable:** `price`
- **Features include:**
  - `kernel perecentage`
  - `size`
  - `close shell percent`
  - `type`
  - `second_type`

---

## 🛠️ Tools & Libraries

- Python (pandas, numpy)
- Data visualization: seaborn, matplotlib
- Machine learning: scikit-learn
  - Models: `LinearRegression`, `RandomForestRegressor`, `GradientBoostingRegressor`, `DecisionTreeRegressor`, `SVR`
  - Metrics: `R²`, `RMSE`, `MAE`, `MAPE`
  - Preprocessing: `MinMaxScaler`, `OneHotEncoder`

---

## 🔄 Workflow

1. **Data Cleaning**
   - Converted price to numeric
   - Removed unnecessary columns
   - Handled categorical variables with one-hot encoding

2. **Feature Engineering**
   - Scaled numerical features using `MinMaxScaler`

3. **Model Training**
   - Trained multiple regression models
   - Evaluated using R², RMSE, MAE, MAPE

4. **Model Comparison**
   - Printed metrics for each model
   - Tracked and selected the best model based on R²

5. **Interpretability**
   - Displayed feature importances (tree models)
   - Displayed coefficients (linear model)

6. **Forecasting Example**
   - Used best model to predict price for a new pistachio entry

---

## 📊 Results Summary

- Best model selected based on highest **R² score** on test data
- Displayed **feature importance** or **coefficients** depending on model type
- Example prediction shows how the model can generalize to unseen inputs

---

## 📦 Sample Prediction

```python
New Input:
{
  "kernel perecentage": 48.0,
  "size": 22.1,
  "close shell precent": 93.0,
  "type": "Fandoghi",
  "second_type": "Closed Shell"
}

💰 Forecasted Price: $X.XX

├── Book1.csv               # Dataset
├── pistachio_price_model.py  # Main model code
├── README.md               # Project description

👤 Author
Siavash Babi
📧 siarbabi@ttu.edu
🎓 Texas Tech University – MS in Data Science (2025)
🔗 LinkedIn (linkedin.com/in/siavash-arbabi)
