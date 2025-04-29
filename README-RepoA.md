<<<<<<< HEAD

# Life Expectancy Prediction Project

This project leverages data from the World Health Organization (WHO) and the United Nations to predict life expectancy for 193 countries between the years 2000 and 2015. Using a stacked regression model, the project aims to identify the key health, economic, and social factors affecting life expectancy. The model is deployed on Streamlit Cloud, allowing users to interactively input data and obtain life expectancy predictions.

## About the Dataset

The dataset consists of 2938 rows and 22 columns, featuring 20 predictor variables grouped into several key categories:

- **Immunization Factors**: Hepatitis B, Polio, Diphtheria
- **Mortality Factors**: Adult Mortality, Infant Deaths, Under-5 Deaths
- **Economic Factors**: GDP, Income Composition of Resources
- **Social Factors**: Schooling, Population, Status

The data was sourced from WHO's Global Health Observatory (GHO) and the United Nations. Missing data for variables like GDP and Hepatitis B for less known countries (e.g., Vanuatu, Tonga, Togo) led to their exclusion from the final dataset.

## Problem Statement

Previous studies on life expectancy often omitted the effects of immunization and the Human Development Index. This project addresses these gaps by focusing on critical health-related, social, and economic factors. By analyzing data from 2000 to 2015, the project helps identify which factors most significantly influence life expectancy, providing insights for countries looking to improve the health of their populations.

## Model Overview

The project utilizes a **Stacked Regressor**, combining the strengths of different machine learning models to achieve more accurate predictions. The model consists of:

- **Base Models**:
  - **Extra Trees Regressor** (n_estimators=300)
  - **Random Forest Regressor** (n_estimators=200)
  - **Gradient Boosting Regressor** (n_estimators=200)
  
- **Meta Model**:
  - **Linear Regression**, which combines the predictions from the base models to provide the final prediction.

### Key Features:
- Data pre-processing to handle missing values and select relevant features.
- Stacking Regressor with cross-validation (cv=5) for robust performance.
- Evaluation using **Mean Absolute Error (MAE)** and **R-squared (R²)** metrics to assess model accuracy.

## Streamlit Deployment

The model is deployed on Streamlit Cloud, enabling users to input features such as GDP, adult mortality, and immunization rates to predict life expectancy.

You can access the deployed app [here](https://life-expectancy-app.streamlit.app/).

## How to Use

1. **Clone the repository**:
   ```bash
   git clone https://github.com/Mariam-Ahmed15/life-expectancy-prediction-streamlit-App.git
=======
# DEPI-Project-Life-Chart-
## Life Expectancy Data Analysis
## Project Overview
Life expectancy is a key indicator of a country's overall health and well-being. Understanding the factors that influence life expectancy can provide invaluable insights for policymakers, public health officials, and researchers. This project aims to analyze life expectancy data to identify significant predictors of low life expectancy and provide actionable recommendations for improvement. By leveraging data-driven insights, countries can prioritize areas that will most effectively raise their population's life expectancy.
## Objectives
Identify Predicting Factors: Analyze various factors such as immunizations, mortality rates, financial indicators, social determinants, and health-related issues to determine their impact on life expectancy.
Country-wise Analysis: Highlight the major predictors for each country and provide tailored recommendations.
Data Visualization: Use advanced visualization techniques to present the data in an accessible and actionable manner.
Recommendations: Develop a comprehensive strategy to guide countries in addressing areas of concern for improving life expectancy.
## Dataset
We will use the [Life Expectancy Dataset](https://www.kaggle.com/datasets/kumarajarshi/life-expectancy-who) provided by the World Health Organization (WHO), available on Kaggle.
>>>>>>> repob/main
