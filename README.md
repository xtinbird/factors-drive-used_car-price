# What Drives the Price of a Car?

**UC Berkeley Applied Machine Learning**  
**Required Assignment 11.1**  

---

## 📋 Project Overview

This project follows the **CRISP-DM** framework to analyze a large dataset of used cars (~426,000 records) and identify the key factors that drive vehicle prices. The goal is to provide actionable insights to a used car dealership for better inventory optimization and pricing strategy.

## 🛠 Technologies Used

- Python, Pandas, NumPy
- Matplotlib & Seaborn (Visualization)
- Scikit-learn (Modeling & Preprocessing)
- Jupyter Notebook

## 📊 Key Findings

- **Vehicle Age** and **Mileage** are the strongest predictors of price.
- **Luxury brands** (BMW, Mercedes-Benz, Audi, Porsche, Lexus) command significant premiums.
- Cars in **Excellent** or **Like New** condition sell for substantially more.
- **4WD/AWD** vehicles have a strong positive impact on price.
- **Diesel** and certain fuel types tend to hold value better.

## 📈 Modeling Approach

- **Target Variable**: `log_price` (log-transformed to handle skewness)
- **Models Built**: Linear Regression, Ridge Regression, Lasso Regression
- **Techniques Used**: 
  - One-Hot Encoding + StandardScaler
  - Regularization (Ridge & Lasso)
  - GridSearchCV for hyperparameter tuning
  - Cross-validation

## 📁 Repository Structure
```text
What-Drives-the-Price-of-a-Car/
├── README.md
├── prompt_II.ipynb          
├── data.zip/
│   └── vehicles.csv
└── images/
```

## 🚀 How to Run

1. Unzip `vehicles.csv` in data.zip. You may need to change the directry when read CSV file.
2. Place it in the project folder
3. Open `prompt_II.ipynb` in Jupyter Notebook or Google Colab
4. Run all cells

## 🎯 Recommendations for the Dealership

1. **Focus inventory** on 2018+ model years with under 60,000 miles.
2. **Prioritize luxury brands** and 4WD/AWD vehicles for higher margins.
3. **Invest in reconditioning** to bring cars to "Excellent" or "Like New" condition.
4. Be cautious with high-mileage older mainstream vehicles.

## 📌 Future Improvements

- Add interaction terms (e.g., Age × Luxury Brand)
- Incorporate regional pricing analysis
- Explore tree-based models (Random Forest, XGBoost)
- Integrate more recent 2025–2026 data

---

**Submitted as part of UC Berkeley Applied Machine Learning Program**
