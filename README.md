## Overview
Respiratory distress syndrome (RDS) remains a leading cause of morbidity and mortality in premature infants, often requiring timely exogenous surfactant therapy. Current clinical decision-making for surfactant administration and dosing is challenging due to the integration of heterogeneous clinical, imaging, and laboratory data.

PreSurf-XAI is an explainable machine learning framework designed to support early, personalized decisions regarding surfactant therapy in preterm neonates (≤34 weeks' gestation). The framework addresses two sequential clinical questions:

Will the infant require surfactant therapy? (binary prediction)

How many surfactant doses will be needed? (multiclass prediction: 0, 1, or 2 doses)

## Key Features: 
Two-stage explainable architecture combining CatBoost (binary) and Random Forest with SMOTE (multiclass)

High predictive performance with built-in interpretability via SHAP analysis and feature importance

Clinically actionable outputs designed for NICU decision support

Handles class imbalance using synthetic oversampling techniques

## Key Predictive Features
Surfactant Requirement Prediction
FiO₂ at admission
Gestational age
Head circumference
Respiratory distress at birth
Base excess

## Dose Number Prediction
FiO₂ at admission
5-minute Apgar score
Base excess
Gravidity
Multiple birth (twin/triplet)
