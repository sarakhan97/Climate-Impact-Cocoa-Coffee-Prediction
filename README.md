# Climate Impact on Coffee and Cocoa Quality Prediction

## Project Overview

This project analyzes how climate-related and crop-specific factors influence coffee and cocoa quality and yield. The goal is to build an end-to-end machine learning workflow that takes raw agricultural datasets, cleans and prepares the data, applies feature engineering, trains multiple models, and compares model performance to identify which techniques work best for crop quality and yield prediction.

The project includes two main workflows:

- Coffee quality prediction
- Cocoa quality and yield prediction

The coffee workflow focuses on cleaning and combining Arabica coffee datasets from multiple years, preparing the data for modeling, and testing different machine learning and deep learning models. The cocoa workflow focuses on predicting cocoa yield and quality using structured crop and climate-related datasets, with additional experiments using advanced models such as TabNet.

## Problem Statement

Climate change can affect agricultural production, crop quality, and yield. Coffee and cocoa are especially sensitive to environmental conditions such as temperature, rainfall, altitude, and regional climate patterns. This project explores how data science and machine learning can be used to understand these relationships and support better prediction of crop outcomes.

The main questions explored in this project were:

- Which climate and crop-related features are useful for predicting coffee and cocoa quality/yield?
- Which machine learning models perform best on the available datasets?
- How can raw agricultural datasets be cleaned, combined, and transformed into a modeling-ready format?
- Can machine learning help identify patterns that may support agricultural planning and crop quality analysis?

## Datasets

The project uses coffee and cocoa datasets containing crop quality, yield, location, and climate-related information. The coffee data includes Arabica coffee datasets from different years, while the cocoa data includes cocoa quality and yield-related datasets.

The data required preprocessing steps such as:

- Removing unnecessary or inconsistent columns
- Handling missing values
- Cleaning numerical and categorical fields
- Combining datasets from different years
- Encoding categorical variables
- Preparing final modeling datasets
- Splitting data into training and testing sets

## Technologies Used

- Python
- Jupyter Notebook
- pandas
- NumPy
- scikit-learn
- XGBoost
- TensorFlow / Keras
- PyTorch / TabNet
- Matplotlib
- Seaborn
- Git
- GitHub

## Machine Learning Models Used

The project experiments with multiple machine learning and deep learning models, including:

- Random Forest
- XGBoost
- LSTM
- ResNet
- TabNet
- Neural Network models
- Wrapper-based modeling approaches

These models were used to compare traditional machine learning methods with deep learning techniques for structured agricultural data.

## Methodology

The project followed an end-to-end data science workflow:

1. **Data Collection**  
   Coffee and cocoa datasets were gathered from available crop quality, yield, and climate-related sources.

2. **Data Cleaning**  
   Raw datasets were cleaned by handling missing values, removing unnecessary fields, fixing inconsistent formats, and preparing clean versions of the data.

3. **Data Preprocessing**  
   Numerical and categorical variables were transformed into a modeling-ready format using encoding, scaling, and feature selection techniques.

4. **Feature Engineering**  
   New useful features were created or refined to improve model performance and make the data more suitable for prediction.

5. **Model Training**  
   Multiple models were trained on the prepared datasets to predict coffee and cocoa quality/yield outcomes.

6. **Model Evaluation**  
   Models were evaluated using regression metrics such as R², MAE, and RMSE where applicable.

7. **Model Comparison**  
   The results from different models were compared to identify which algorithms performed better for the available data.

## Results and Findings

The project showed that tree-based machine learning models such as Random Forest and XGBoost performed strongly on structured crop and climate datasets. These models were effective because they can handle nonlinear relationships and mixed feature types better than some deep learning models on smaller tabular datasets.

For cocoa prediction, preprocessing, feature engineering, and proper handling of categorical variables had a major impact on model performance. Advanced models such as TabNet were also tested to explore whether deep learning approaches could improve prediction quality on structured data.

For coffee prediction, multiple models were tested, including Random Forest, XGBoost, LSTM, ResNet, and wrapper-based approaches. The coffee workflow helped compare traditional machine learning models with neural network-based methods for quality prediction.

Overall, the project demonstrated that machine learning can be used to analyze agricultural datasets and identify patterns between climate-related factors and crop outcomes.

## Key Skills Demonstrated

- Data cleaning and preprocessing
- Exploratory data analysis
- Feature engineering
- Machine learning model development
- Regression modeling
- Model evaluation and comparison
- Jupyter Notebook workflow
- Git and GitHub project organization
- Data science documentation
- Climate and agriculture analytics

## Repository Structure

```text
Climate-Impact-Cocoa-Coffee-Prediction/
│
├── README.md
├── RUN_ORDER.md
├── requirements.txt
├── .gitignore
│
├── coffee/
│   ├── clean_coffee_2008.ipynb
│   ├── clean_coffee_data_2023.ipynb
│   ├── clean_coffee_data_2025.ipynb
│   ├── coffee_combined_clean.ipynb
│   ├── random_forest.ipynb
│   ├── xgboost.ipynb
│   ├── LSTM.ipynb
│   ├── resnet.ipynb
│   ├── Wrapper.ipynb
│   └── coffee CSV data files
│
├── cocoa/
│   ├── 01_cocoa_yield_prediction.ipynb
│   ├── 02_cocoa_quality_prediction.ipynb
│   ├── 03_cocoa_tabnet_quality_experiments.ipynb
│   ├── archive_cocoa_first_experiments.ipynb
│   └── cocoa CSV data files
