# Customer Churn Risk Prediction – PowerCo Case Study

This repository contains an end-to-end workflow for predicting customer churn in the energy sector. Using **electricity consumption and contract data from PowerCo**, we perform exploratory analysis, feature engineering, and machine learning modeling to uncover churn drivers and build predictive insights that support actionable retention strategies.

---

## Repository Structure

```
.
├── PowerCo_EDA.ipynb         # Exploratory data analysis of customer contracts and churn
├── feature_engineering.ipynb # Feature creation and preprocessing pipeline
├── RandomForest.ipynb        # Model training & evaluation (Random Forest)
└── README.md
```

---

## Project Workflow

1. **Exploratory Data Analysis (EDA)**
   - Analyzed churn distribution across:
     - Tariff types  
     - Contract durations  
     - Customer segments  
   - Identified consumption and behavioral patterns driving attrition.  

2. **Feature Engineering**
   - Created temporal and categorical features to capture seasonal demand and contract behaviors.  
   - Applied preprocessing: handling missing data, encoding categorical variables, scaling numerical values.  

3. **Modeling with Random Forest**
   - Built and optimized a Random Forest classifier for churn prediction.  
   - Evaluated model with accuracy, precision/recall, and feature importance.  
   - Results highlight key factors influencing customer retention.  

---

## Key Results

- **Strong predictive performance** with Random Forest, enabling identification of at-risk customers.  
- **Business insights** from feature importances that guide retention strategies.  

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

- Experiment with **XGBoost/LightGBM** for improved performance.  
- Deploy model via **Flask/FastAPI** for real-time churn scoring.  
- Extend feature set with external consumption or demographic data.  

