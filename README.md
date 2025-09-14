# CICIDS2017 Random Forest Model

*This project was developed with guidance from ChatGPT during the model training and evaluation process.*

## Project Overview
This project implements a **Random Forest classifier** on the **CICIDS2017 network traffic dataset** to detect normal and attack traffic.

## Dataset
- **Name:** CICIDS2017  
- **Description:** Network traffic data collected over several days, including normal and attack traffic.  
- **Target:** `Label` column (Normal = 0, Attack = 1)  

## Model
- **Algorithm:** Random Forest  
- **Goal:** Predict whether traffic is normal or an attack.  
- **Why Random Forest:** Combines multiple decision trees for better accuracy and handles large datasets well.

## Preprocessing
- Dropped unnecessary columns: `Src IP dec`, `Dst IP dec`, `Timestamp`  
- Encoded target labels  
- Split data: 70% training, 30% testing  

## Evaluation
- **Metrics:** Accuracy, Precision, Recall, F1-score  
- **Result:** Accuracy ~ 0.9985  

## Files
- `CICIDS2017_RandomForest.ipynb` – notebook with preprocessing, training, evaluation, and feature importance  

## References
- [CICIDS2017 Dataset](https://www.unb.ca/cic/datasets/ids-2017.html)  
- [Scikit-learn Random Forest](https://scikit-learn.org/stable/modules/ensemble.html#forest)
