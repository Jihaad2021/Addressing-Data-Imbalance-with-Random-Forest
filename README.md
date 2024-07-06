# Project Summary: Addressing Data Imbalance with Random Forest
## Project Overview
This research aims to identify the best method for addressing data imbalance using the Random Forest model. The study evaluates the effectiveness of various sampling techniques to enhance model performance.

# Objectives
- To determine the optimal method for handling imbalanced datasets in classification tasks.
- To compare the performance of different sampling techniques on the Random Forest model.

## Sampling Techniques Used
- Oversampling
- Undersampling
- Synthetic Minority Over-sampling Technique (SMOTE)
- Edited Nearest Neighbors (ENN)
- SMOTE combined with Edited Nearest Neighbors (SMOTEENN)

## Data Source
The data used in this research is sourced from the Behavioral Risk Factor Surveillance System (BRFSS) database, 
which comprises:
- Entries: 236,378 (0: 197.191 ,1: 5.619 ,2: 33.568) 
- Features: 21 
- Labels: 3 (0: No-diabetic, 1: Pra-Diabetic, 2: Diabetic)

## Methodology
- Data Collection: Extract data from the BRFSS database.
- Data Preprocessing: Apply various sampling techniques to handle data imbalance.
- Model Training: Train the Random Forest model on the preprocessed data.
- Model Evaluation: Assess model performance using metrics such as accuracy, precision, recall, and F1 score.

## Results
| Metode | Accuracy | Precision | Recall | F1-Macro | AUC |
| --- | --- | --- | --- | --- | --- |
| Random Forest (RF) | 0.70 | **0.45** | 0.38 | 0.39 | 0.72 |
| RF + Oversampling | 0.80 | 0.44 | 0.41 | 0.42 | 0.72 |
| RF + Undersampling | 0.56 | 0.43 | 0.47 | 0.39 | 0.71 |
| RF + SMOTE | 0.80 | 0.44 | 0.39 | 0.39 | **0.73** |
| RF + ENN | **0.82** | 0.49 | 0.36 | 0.36 | 0.71 |
| RF + SMOTEEN | 0.71 | 0.43 | **0.48** | **0.43** | **0.73** |

The SMOTEENN technique produced the best results in terms of model performance, effectively addressing data imbalance and enhancing the Random Forest model's Recall, F1-Macro dan AUC and reliability.

## Conclusion
This study successfully identified SMOTEENN as the most effective technique for handling data imbalance in the context of the Random Forest model, leading to improved classification performance on the BRFSS dataset.




