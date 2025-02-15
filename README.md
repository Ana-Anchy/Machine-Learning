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
  - **Slutsats:**
    - Den **linjära regressionsmodellen** presterade bra, men **Lasso-regressionen** visade ett marginellt lägre RMSE på valideringsdata.
    - Skillnaden mellan modellerna är dock mycket liten, vilket tyder på att **feature selection** inte var avgörande för detta PoC.
    - Det slutgiltiga testet bekräftade modellens prestanda, men det finns fortfarande **utrymme för förbättringar**.
    - Nästa steg kan vara att testa mer avancerade modeller (såsom **Random Forest** eller **XGBoost**) samt genomföra mer **feature engineering**.





