# Predicting Safe Nicotine Intake Using Biomedical and Behavioral Health Profiles

## 1. Overview

This project aims to develop a regression model that can estimate how much nicotine (in milligrams per month) an individual can safely consume based on their biomedical health data, smoking behaviour, and serum cotinine levels. This is particularly relevant in light of Australia’s updated national laws that require pharmacist approval for vape products.

Since no detailed Australian dataset was available with nicotine biomarkers, this project uses the US-based NHANES dataset (2007–2020), which contains clinically relevant features including serum cotinine as a measure of nicotine exposure. A custom dataset was created by merging six NHANES cycles and carefully selecting and engineering 40 features, later refined to 38 after cleaning.

The final goal of this project is to support pharmacists or public health practitioners with a model that can generate personalised nicotine intake recommendations or warnings.

## 2. Setup

This project is implemented in Python using a Jupyter Notebook. You can either:

- **Run the notebook in Google Colab** (recommended, no setup needed), or  
- **Run locally using Anaconda**, with required packages installed (e.g. pandas, matplotlib, seaborn, scikit-learn)

The Jupyter notebook contains all steps: data import, preprocessing, exploratory data analysis, and preparation for modelling.

## 3. How to Run This Project

You can follow the steps below to reproduce or review the project:

1. Open the file `Nicotine_Intake_Prediction.ipynb` in Jupyter or Google Colab
2. Make sure the dataset `NHANES_Cleaned_Ready.csv` is in the same directory or mounted in Colab
3. Run the notebook cell-by-cell to see:
   - Dataset import and overview
   - Data cleaning and missing value handling
   - Feature engineering (e.g., blood pressure averaging)
   - Exploratory data analysis and visualisations
   - Project summary and future directions

## 4. Files in This Repository

- `Nicotine_Intake_Prediction.ipynb`: Jupyter notebook with full analysis
- `NHANES_Cleaned_Ready.csv`: Final merged and cleaned dataset (2007–2020 NHANES data)
- `README.md`: This file

## 5. Notes for the Reviewer 

- Please run the notebook in order — all cells have been executed and cleaned.
- EDA has been completed through multiple visualisations: heatmaps, boxplots, scatter plots, and histograms.
- All research justifications and report writing are included in the notebook comments and markdown cells.
- Feature justification and explanation are provided in table format.
- We have taken care to ensure all code is well-commented and output matches expectations.
- If needed, additional NHANES cycles can be merged later to improve the model (discussed in Part 4 of the report).

## 6. Author

Pritthika Dhar  
Master of Artificial Intelligence and Machine Learning  
The University of Adelaide  
July 2025
