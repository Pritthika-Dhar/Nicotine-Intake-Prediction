# Predicting Safe Nicotine Intake Using Biomedical and Behavioral Health Profiles

## 1. Overview

This project develops and evaluates multiple supervised regression models to predict safe monthly nicotine intake based on individuals’ biomedical indicators, behavioural patterns, and log-transformed serum cotinine levels. The analysis is grounded in public health policy relevance, particularly in response to Australia's pharmacist-only vape regulations.

Since no detailed Australian dataset was available, the project utilises data from the US-based NHANES (2007–2020). A clean and feature-rich dataset was created by merging six NHANES cycles, carefully selecting and engineering variables across biomedical, behavioural, and demographic domains. The final model aims to assist pharmacists and public health professionals in estimating nicotine exposure risks.

## 2. Setup

This project is implemented in Python using a Jupyter Notebook. You can:

- **Run the notebook in Google Colab** (recommended — no setup needed), or  
- **Run locally via Anaconda**, with required packages such as pandas, matplotlib, seaborn, scikit-learn, and xgboost.

The notebook includes all steps: from data import and preprocessing to model selection and performance evaluation.

## 3. How to Run This Project

1. Open the notebook `Nicotine_Intake_Prediction.ipynb` in Jupyter or Colab  
2. Ensure `NHANES_Cleaned_Ready.csv` is in the working directory or uploaded to Colab  
3. Run all cells to explore:

   - Data merging, cleaning, and log transformation
   - Exploratory visualisations (e.g. histograms, scatter plots, correlation matrices)
   - PCA transformation and comparison with original feature set
   - Model training (Linear, Ridge, Random Forest, XGBoost, MLP)
   - Performance evaluation using five metrics
   - Final model selection based on predictive accuracy and robustness

## 4. Files in This Repository

- `Nicotine_Intake_Prediction.ipynb`: Full project notebook with modelling and analysis
- `NHANES_Cleaned_Ready.csv`: Final cleaned and standardised dataset (2007–2020)
- `Model_Comparison_Table_Bordered.png`: Summary table comparing best model results
- `README.md`: Project summary and run instructions

## 5. Notes for the Reviewer (Teacher / Marker)

- All models were trained and evaluated on the original feature set after PCA was found to degrade performance.
- Five models were tested: Linear Regression, Ridge Regression, Random Forest, XGBoost, and MLP.
- Model refinement included hyperparameter tuning for Random Forest and XGBoost (e.g. tree depth, estimators, learning rate).
- Evaluation metrics included R² score, MAE, RMSE, Median AE, and Explained Variance.
- The tuned XGBoost model achieved the best overall performance and was selected as the final model.
- Visual results are included throughout the notebook, and final comparison figures are exported as PNG files.

## 6. Author

Pritthika Dhar  
Master of Artificial Intelligence and Machine Learning  
University of Adelaide  
July 2025
