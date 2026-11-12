# Global Supply Chain Disruption Prediction

## Project Overview

This project focuses on predicting shipment delivery delays using Machine Learning. It uses a Random Forest Classification model to identify whether a shipment will arrive **On Time** or **Late** based on various supply chain factors.

The project explores how transportation mode, product category, scheduled lead time, weather severity, geopolitical risk, shipping cost, and order weight relate to shipment delivery performance.

## Problem Statement

Late deliveries can affect supply chain efficiency, increase operational costs, and impact customer satisfaction.

The objective of this project is to analyze shipment data, identify factors associated with delivery delays, and develop a machine learning classification model to predict shipment delivery status.

## Dataset

- **Dataset:** Global Supply Chain Disruption Dataset
- **Records:** 10,000
- **Features:** 19 columns
- **Target Variable:** Delivery Status (On Time / Late)

The dataset contains information related to shipment routes, transportation modes, product categories, lead times, weather conditions, geopolitical risks, shipping costs, and order weights.

## Tools & Technologies

- Python
- Pandas & NumPy
- Matplotlib & Seaborn
- Scikit-learn
- Imbalanced-learn (SMOTE)
- Jupyter Notebook

## Project Workflow

1. Data loading and initial inspection.
2. Data cleaning and preprocessing.
3. Exploratory Data Analysis (EDA).
4. Analysis of shipment delays across different supply chain factors.
5. Categorical variable encoding.
6. Train-test split (80:20).
7. Random Forest classification model development.
8. Handling class imbalance using class weights and SMOTE.
9. Model evaluation using classification report and confusion matrix.
10. Feature importance analysis.

## Model Performance

The class-weighted Random Forest model achieved the following results:

| Evaluation Metric | Result |
|---|---:|
| Accuracy | 90.50% |
| Late Shipment Precision | 0.77 |
| Late Shipment Recall | 0.37 |
| Late Shipment F1-Score | 0.50 |

The project also compares the class-weighted Random Forest model with SMOTE-based resampling to evaluate its impact on identifying late shipments.

## Key Observations

- The model achieved 90.50% overall accuracy.
- The class-weighted Random Forest model performed better than the SMOTE-based model in terms of Late-class recall and F1-score.
- Identifying late shipments remains a challenge, with a recall of 37%.
- The results highlight the importance of evaluating precision and recall alongside accuracy when working with imbalanced classification problems.

## Repository Structure

```text
supply-chain-disruption-prediction/
│
├── SupplyChain_RandomForest_.ipynb
├── global_supply_chain_disruption_v1.csv
└── README.md
```

## How to Run the Project

1. Clone this repository:

   ```bash
   git clone https://github.com/Paawankumar11/supply-chain-disruption-prediction.git
   ```

2. Navigate to the project directory.

3. Install the required libraries:

   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn jupyter
   ```

4. Open the Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

5. Open `SupplyChain_RandomForest_.ipynb` and run the cells.

## Future Improvements

- Improve recall for late shipment predictions.
- Perform hyperparameter tuning to optimize model performance.
- Experiment with different classification algorithms.
- Optimize the classification threshold based on business requirements.
