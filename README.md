# 🌍 Life Expectancy Dashboard & Prediction App
### This project explores global health indicators by leveraging data from the World Health Organization (WHO). It includes data cleaning, interactive visual analytics, and machine learning to predict life expectancy based on key socio-economic and health factors. The final model and dashboard are deployed using Streamlit for public access.

## Dataset
We will use the [Life Expectancy Dataset](https://www.kaggle.com/datasets/kumarajarshi/life-expectancy-who) provided by the World Health Organization (WHO), available on Kaggle.
The dataset consists of 2938 rows and 22 columns, featuring 20 predictor variables grouped into several key categories:

- **Immunization Factors**: Hepatitis B, Polio, Diphtheria
- **Mortality Factors**: Adult Mortality, Infant Deaths, Under-5 Deaths
- **Economic Factors**: GDP, Income Composition of Resources
- **Social Factors**: Schooling, Population, Status


 ## Features
📊 **Interactive Dashboard**
Built using Streamlit to explore trends across countries and years. Users can filter data by country, region, or year and visualize factors such as GDP, education, mortality, and healthcare infrastructure.

-----
🧹 **Data Cleaning & Preprocessing**
Handled missing values, normalized continuous features, and encoded categorical data to ensure high model quality.

-----

📈 **Model Overview**

The project utilizes a **Stacked Regressor**, combining the strengths of different machine learning models to achieve more accurate predictions. The model consists of:

- **Base Models**:
  - **Extra Trees Regressor** (n_estimators=300)
  - **Random Forest Regressor** (n_estimators=200)
  - **Gradient Boosting Regressor** (n_estimators=200)
  
- **Meta Model**:
  - **Linear Regression**, which combines the predictions from the base models to provide the final prediction.
-  **Key Features**:
  - Data pre-processing to handle missing values and select relevant features.
  - Stacking Regressor with cross-validation (cv=5) for robust performance.
  - Evaluation using **Mean Absolute Error (MAE)** and **R-squared (R²)** metrics to assess model accuracy.

----

🚀 **Streamlit Deployment**

The model is deployed on Streamlit Cloud, enabling users to input features such as GDP, adult mortality, and immunization rates to predict life expectancy.

You can access the deployed app [here](https://life-expectancy-prediction-app-app-xzwhw45ah9aanatntpjkxp.streamlit.app/).


---- 

## How to Use

 **Clone the repository**:
   ```bash
   git clone https://github.com/Mariam-Ahmed15/life-expectancy-prediction-streamlit-App.git
```

