# BinarySmoke: Smoking Status Prediction from Bio-Signals

## Overview
This project explores predicting smoking status from non-invasive bio-signal data. The work evaluates multiple machine learning classifiers on clinical measurements to enable automatic identification of smokers, especially when self-reporting is unavailable or unreliable.

## Objectives
- Build a model that predicts smoker status without relying on patient self-reporting.
- Compare multiple machine learning approaches for classification performance.

## Dataset
The dataset contains **38,984 samples** with **23 features** (22 predictors + smoking status target). Features fall into the following groups:
- **Physical characteristics:** age, height, weight, waist circumference, dental caries.
- **Sensory tests:** eyesight and hearing results.
- **Anemia/diabetes indicators:** hemoglobin and blood sugar levels.
- **Heart disease indicators:** triglycerides, HDL, LDL, and total cholesterol.
- **Liver/kidney indicators:** urine protein, serum creatinine, AST, ALT, and GGT levels.

The data is pre-cleaned with no missing values and split into **60% train / 20% validation / 20% test** sets. Ages are grouped into ranges: **20-32, 33-45, 46-58, 59-71, 72-85**.

## Models Evaluated
- Logistic Regression (LR)
- Support Vector Machine (SVM)
- Random Forest (RF)
- Neural Networks (NN)

## Results (from the report)
- **Random Forest** achieved the best performance with **AUC ~87%**.
- **Logistic Regression** and **Neural Networks** performed comparably with **AUC ~80%**.

## Repository Contents
- `BinarySmokePrediction.ipynb` — notebook containing the analysis and model experiments.
- `DS9000_Project_Final_For_Real_This_Time.pdf` — project report summarizing methodology and results.

## Notes
This README is derived from the project report and summarizes the dataset, objectives, and reported results.
