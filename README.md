
# 🏠 Real Estate Price Prediction and Analysis

This project performs **data cleaning**, **feature engineering**, **exploratory data analysis (EDA)**, and **machine learning** to predict real estate prices. It uses property listing data and builds regression models to estimate property values based on key features.

---

## 📌 Overview

- Cleans and preprocesses real estate data
- Handles missing values and outliers
- Encodes categorical features
- Performs univariate and bivariate visualizations
- Trains and compares multiple regression models
- Exports cleaned dataset and saves the best-performing model

---

## 🛠 Technologies Used

- **Python**
- **Pandas** – for data manipulation
- **NumPy** – for numerical operations
- **Matplotlib** & **Seaborn** – for data visualization
- **Scikit-learn** – for machine learning models
- **Joblib** – for saving the model and scaler

---

## 📁 File Descriptions

| File Name | Description |
|-----------|-------------|
| `code.py` | The complete script for preprocessing, EDA, model training, evaluation, and saving outputs |
| `Property_with_Feature_Engineering.csv` | Original dataset containing real estate listings (ensure it's present in your directory) |
| `cleaned_dataset.csv` | Cleaned and transformed dataset after preprocessing |
| `house_price_model.pkl` | Trained Random Forest model saved for future predictions |
| `scaler.pkl` | StandardScaler object saved for consistent feature scaling |

---

## 🚀 How to Run the Project

1. **Clone the Repository**
   ```bash
   git clone https://github.com/Suhaibahmad19/House-Price-Prediction-Project.git
   cd House-Price-Prediction-Project
   ```

2. **Install Dependencies**
   Make sure Python 3.x is installed, then run:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn joblib
   ```

3. **Add Dataset**
   Place `Property_with_Feature_Engineering.csv` in the root directory.

4. **Run the Script**
   ```bash
   python code.py
   ```

---

## 📊 Model Evaluation Results

| Model                | R² Score | MAE    | MSE    | RMSE   |
|---------------------|----------|--------|--------|--------|
| Linear Regression    | 0.2000   | 0.6708 | 0.8166 | 0.9036 |
| Decision Tree        | 0.4664   | 0.3683 | 0.5446 | 0.7380 |
| Random Forest        | 0.5796   | 0.3493 | 0.4291 | 0.6551 |

✅ **Best Model**: Random Forest Regressor

---

## 📈 Key Features Engineered

- `price_per_sqft`: Derived by dividing price by area
- `location_encoded`: Location mapped to average prices
- `year`, `month`, `day`: Extracted from date
- Standardized continuous variables (e.g., price, area_sqft)

---

## 📉 Visual Insights

- Distribution plots and boxplots for numeric features
- Count plots for categorical values
- Scatter plots and correlation heatmaps
- Line charts showing yearly/monthly price and area trends

---

## 📦 Outputs

- `cleaned_dataset.csv`: Final cleaned and engineered dataset
- `house_price_model.pkl`: Trained Random Forest model
- `scaler.pkl`: Feature scaler for deployment

---

## 📬 Contact

For questions, feedback, or collaboration:

**Your Name**  
Email: [suhaibraza42@gmail.com]  

---

## 📄 License

This project is licensed under the **MIT License** – feel free to use and modify it.
