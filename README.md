# Customer Churn Risk Prediction – PowerCo Case Study

This repository contains an end-to-end machine learning workflow for **predicting customer churn** in the energy sector. Using **PowerCo’s electricity consumption, contract, and pricing data**, the project explores churn patterns, engineers predictive features, and trains a machine learning model to identify at-risk customers.

---

## Repository Structure

```
.
├── PowerCo_EDA.ipynb          # Exploratory Data Analysis of client consumption & churn
├── feature_engineering.ipynb  # Feature engineering & preprocessing pipeline
├── RandomForest.ipynb         # Random Forest model training & evaluation
├── client_data.csv            # Raw client contract & consumption data
├── price_data.csv             # Pricing data (peak, off-peak, mid-peak tariffs)
├── clean_data_after_eda.csv   # Processed dataset after EDA
├── data_for_predictions.csv   # Final dataset used for churn predictions
├── Data Description.pdf       # Field descriptions for client & price data
└── README.md
```

---

## Project Workflow

1. **Exploratory Data Analysis (EDA)**
   - Examined churn distribution across tariff types, contract durations, and customer segments.
   - Visualized electricity & gas consumption patterns to uncover churn drivers.

2. **Feature Engineering**
   - Derived temporal, contract-based, and margin-related features.
   - Cleaned missing values and encoded categorical variables.
   - Prepared datasets for model training.

3. **Modeling with Random Forest**
   - Built and optimized a Random Forest classifier to predict churn.
   - Evaluated using precision, recall, accuracy, and feature importance.
   - Identified key features influencing attrition, supporting targeted retention strategies.

---

## Data Sources

- **client_data.csv**: Contract info, consumption history, forecasts, margins, and churn label.  
- **price_data.csv**: Energy and power prices across peak, off-peak, and mid-peak periods.  
- **Data Description.pdf**: Documentation of all fields and business context.  

---

## Key Results

- Strong predictive accuracy using Random Forest.  
- Top churn drivers identified: contract duration, energy margins, tariff types, and consumption forecasts.  
- Framework enables **actionable retention strategies** for high-risk customers.  

---

## Tech Stack

- Python 3.8+  
- pandas, numpy, matplotlib, seaborn  
- scikit-learn  

---

## Usage

Clone the repository and install dependencies:

```bash
git clone https://github.com/<your-username>/customer-churn-prediction.git
cd customer-churn-prediction
pip install -r requirements.txt
```

Run notebooks sequentially for full workflow:
1. `PowerCo_EDA.ipynb`  
2. `feature_engineering.ipynb`  
3. `RandomForest.ipynb`  

---

## Future Work

- Benchmark against **XGBoost/LightGBM** for potential performance gains.  
- Deploy as an API (Flask/FastAPI) for real-time churn scoring.  
- Integrate external market/demographic data for feature enrichment.  

