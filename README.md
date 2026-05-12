# Crude Oil Price Prediction
### Using Multiple Linear Regression and Random Forest

---

## Overview
This project predicts daily crude oil closing prices using two 
machine learning models: Multiple Linear Regression (MLR) and 
Random Forest. It was developed as a final project for CSELEC2C 
Machine Learning at the University of Santo Tomas.

---

## Objective
To compare the performance of a parametric model (MLR) against 
a non-parametric ensemble model (Random Forest) in predicting 
crude oil prices using historical market data.

---

## Project Structure
```
Crude-Oil-Price-Prediction/
│
├── data/
│   └── crude_oil_data.csv        ← Dataset (2000–2024)
│
├── notebooks/
│   └── crude_oil_prediction.ipynb ← Main Jupyter notebook
│
├── outputs/
│   ├── oil_price_over_time.png
│   ├── price_distribution.png
│   ├── correlation_heatmap.png
│   ├── mlr_actual_vs_predicted.png
│   ├── rf_actual_vs_predicted.png
│   ├── model_comparison.png
│   └── feature_importance.png
│
├── README.md                      ← You are here
└── requirements.txt               ← Python dependencies
```

---

## Dataset
- **Source:** Kaggle — Crude Oil Stock Dataset 2000–2024
- **Link:** https://www.kaggle.com/datasets/mhassansaboor/crude-oil-stock-dataset-2000-2024
- **Records:** 6,073 daily trading records
- **Features:** Date, Open, High, Low, Close, Adj_Close, Volume
- **Target Variable:** Close Price (USD)

---

## Models Used
| Model | Type | Role |
|---|---|---|
| Multiple Linear Regression | Parametric | Baseline model |
| Random Forest | Ensemble/Non-parametric | Comparison model |

---

## Results
| Model | MAE | RMSE | R² |
|---|---|---|---|
| Multiple Linear Regression | $1.1192 | $1.6248 | 0.9960 |
| Random Forest | $1.2248 | $1.8432 | 0.9948 |

**Key Finding:** MLR outperformed Random Forest, suggesting 
crude oil prices follow a strong linear pattern day-to-day.

---

## How to Reproduce

### Step 1 — Clone the Repository
```bash
git clone https://github.com/YOUR_USERNAME/Crude-Oil-Price-Prediction.git
cd Crude-Oil-Price-Prediction
```

### Step 2 — Install Dependencies
```bash
pip install -r requirements.txt
```

### Step 3 — Add the Dataset
- Download from Kaggle link above
- Place CSV file in the `data/` folder
- Rename to `crude_oil_data.csv`

### Step 4 — Run the Notebook
- Open VS Code
- Navigate to `notebooks/crude_oil_prediction.ipynb`
- Run all cells in order

---

## Tools & Technologies
- **Language:** Python 3.14
- **IDE:** Visual Studio Code
- **Libraries:** pandas, numpy, matplotlib, seaborn, scikit-learn
- **Version Control:** GitHub

---

## AI Use Declaration
Parts of this project used Claude AI (Anthropic) for:
- Brainstorming and topic selection
- Code structure guidance
- Grammar and clarity editing

All models, analysis, and interpretations were reviewed 
and understood by the authors.

---

## Authors 
- Solano, Stephen — University of Santo Tomas, CSELEC2C
- Magcaling, Elijah James — University of Santo Tomas, CSELEC2C
- Pascua, Jerald — University of Santo Tomas, CSELEC2C
