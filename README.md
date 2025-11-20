# Ensemble Learning - XGBoost vs CatBoost

## 📋 Project Overview

Comparative analysis of two powerful Gradient Boosting Decision Tree algorithms:
- **XGBoost**: Optimized gradient boosting with regularization and sparsity awareness
- **CatBoost**: Ordered boosting with native categorical feature support

This project implements both algorithms on multiple datasets with hyperparameter tuning using Optuna.

## 🧠 Key Differences

| Aspect | XGBoost | CatBoost |
|--------|---------|----------|
| **Split Finding** | Exact greedy / Histogram-based | Ordered splits |
| **Categorical Features** | Requires One-Hot Encoding | Native support via Target Encoding |
| **Tree Type** | Standard | Symmetric (Balanced) |
| **Training Speed** | Fast (numerical data) | Moderate |
| **Inference Speed** | Moderate | Fast |
| **Robustness** | Sensitive to hyperparameters | More robust defaults |

## 📊 Datasets

- **Breast Cancer Classification**: Binary classification dataset
- **Real Estate**: Regression task for price prediction
- Additional datasets for comprehensive evaluation

## 🔬 Evaluation Metrics

**Classification**: AUC-ROC, LogLoss, F1-Score
**Regression**: RMSE, MAE
**Efficiency**: Training time, Inference time

## 🚀 Quick Start

```bash
# Install dependencies
pip install -r requirements.txt

# Run experiments
python src/main.py --model xgboost
python src/main.py --model catboost
```

## 📁 Project Structure

- `classification/`: Classification notebooks and models
- `assets/`: Dataset files
- `catboost_info/`: Training artifacts and logs

## 📚 Key Findings

- **Categorical Data**: CatBoost excels with high-cardinality features
- **Hyperparameter Tuning**: XGBoost requires careful tuning; CatBoost more stable
- **Trade-offs**: XGBoost faster training vs CatBoost faster inference