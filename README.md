# MediTrak-ML-Project
# MediTrak — Expiry Risk Prediction & Drug Wastage Minimization

## Problem Statement
Pharmacies and hospitals lose significant money due to medicines 
expiring before they are sold. This project predicts which medicines 
are at high risk of expiring using machine learning, so staff can 
take action early (discounts, returns, redistribution).

## Dataset
- 10,000 rows × 20 columns (expiry_dirty.csv)
- Contains medicine inventory, sales velocity, stock quantity, 
  expiry dates, storage conditions

## Technologies Used
- Python, Pandas, NumPy
- Scikit-learn (Logistic Regression, Random Forest, 
  Gradient Boosting)
- Matplotlib, Seaborn
- Google Colab / Jupyter Notebook

## How to Run
1. Clone this repository
2. Open Meditrack.ipynb in Google Colab or Jupyter
3. Upload expiry_dirty.csv when prompted
4. Run all cells in order

## Project Workflow
1. Data cleaning — handled missing values, fixed negative stock, 
   standardised messy labels
2. Feature engineering — created DaysToExpiry, TurnoverRatio, 
   IsSlowMoving, ValueAtRisk
3. Model training — compared 3 ML models
4. Alert report — generated CSV of at-risk medicines

## Best Model
Gradient Boosting Classifier
- Top features: Sales Velocity, Unit Price, Stock Age, 
  Days To Expiry
