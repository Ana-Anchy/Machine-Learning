# 🧠 Machine Learning Project - Housing Price Prediction

## 📌 Overview
This project involves a **Machine Learning workflow** for **housing price prediction**, covering data preprocessing, exploratory data analysis (EDA), model training, evaluation, and conclusions.

The dataset used includes various housing features such as **location, number of rooms, population density, and median income**.

---

## 🚀 Project Workflow

### **1️⃣ Exploratory Data Analysis (EDA)**
- **Checked for missing values** and visualized them using a heatmap.
- **Descriptive statistics** were generated for better understanding of the dataset.
- **Visualizations** for insights:
  - Distribution of features
  - Correlations between variables
  - Identified important predictive features

### **2️⃣ Data Preprocessing**
- **Handled missing values** using `SimpleImputer(strategy='median')`.
- **Feature selection & transformation**:
  - Removed or encoded non-numeric categorical features (e.g., `ocean_proximity`).
  - Normalized numeric values for better model performance (optional).
- **Data Splitting**:
  - **Training:** 70%
  - **Validation:** 15%
  - **Testing:** 15%

### **3️⃣ Machine Learning Models**
- Implemented and compared:
  - **Linear Regression**
  - **Lasso Regression** (with `GridSearchCV` for hyperparameter tuning)

### **4️⃣ Model Evaluation**
- **Metric Used:**  
  - **Root Mean Squared Error (RMSE)** to measure predictive accuracy.
- **Results (example figures):**
  - Linear Regression RMSE: **~71,495**
  - Lasso Regression RMSE: **~71,944**
  - Final RMSE on Test Set: **~67,135**
- **Conclusions:**
The linear regression model performed well, but Lasso regression showed a marginally lower RMSE on the validation data.
However, the difference between the models is very small, suggesting that feature selection was not critical for this PoC.
The final test confirmed the model's performance, but there is still room for improvement.
The next step could be to try more advanced models (such as Random Forest or XGBoost) and to perform more feature engineering.





