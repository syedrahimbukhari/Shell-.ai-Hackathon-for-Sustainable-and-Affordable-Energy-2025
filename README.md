# 🏆 Ultimate Hybrid Model - Shell AI Hackathon 2025

## Overview
This repository contains the implementation of the Ultimate Hybrid Model developed for the Shell AI Hackathon 2025 – Fuel Blend Properties Prediction Challenge. The model predicts 10 final blend properties from complex component fractions and properties using a hybrid approach combining Gradient Boosting and XGBoost.

## Features
- **Hybrid Modeling:** Gradient Boosting for stable targets, XGBoost for complex patterns.  
- **Target-Specific Feature Engineering:** Captures interactions, outlier handling, and statistical robustness.  
- **Prediction Pipeline:** Data preprocessing, feature recreation, smart prediction, and fallback mechanisms.  
- **Production-Ready:** Robust error handling, feature persistence, and reproducible configurations.  
- **Deliverables:** Submission-ready CSV/Numpy predictions, feature sets, and trained model files.  

## Model Details
- **Gradient Boosting:** n_estimators=100-300, learning_rate=0.05-0.15, max_depth=3-4  
- **XGBoost:** n_estimators=100-500, learning_rate=0.01-0.2, max_depth=3-7, regularization alpha=0-1, lambda=1-3  
- **Targets:** 10 blend properties (BlendProperty1 to BlendProperty10)  
- **Feature Engineering:** 56 raw features expanded to 74 with target-specific features  

## Usage
1. Load the test dataset (`test.csv`).  
2. Execute the prediction pipeline (`predict.py` or notebook).  
3. Output: `hybrid_predictions.csv` ready for competition submission.  

## Deliverables
- `hybrid_predictions.csv` - Main competition submission  
- `hybrid_predictions.npy` - Backup predictions  
- `feature_sets.pkl` - Feature configuration  
- `ultimate_hybrid_model.pkl` - Primary trained model  
- `smart_hybrid_model.pkl` & `xgb_hybrid_model.pkl` - Alternative hybrid variants  

## License
This repository is for educational and competition purposes.  

## Conclusion
The Ultimate Hybrid Model leverages advanced machine learning techniques to optimize fuel blend predictions, supporting sustainable and high-performance energy solutions.


