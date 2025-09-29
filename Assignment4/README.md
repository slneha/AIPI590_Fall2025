# Assignment 4: Explainable Techniques II

## Dataset
The dataset used is the PRSA Beijing PM2.5 Dataset (UCI Repository), which records hourly air quality and meteorological data from 2010 to 2014. The target variable is PM2.5 concentration.

## Preprocessing
- Standardized column names and parsed datetime
- Removed sentinel missing values and imputed missing data
- Engineered temporal features including month, hour, day of week, and weekend indicator

## Model
A Random Forest Regressor is trained within a scikit-learn pipeline.  
- Numeric features: median imputation and scaling  
- Categorical features: most frequent imputation and one-hot encoding  

The model is then explained using PDP, ICE, and ALE plots.
