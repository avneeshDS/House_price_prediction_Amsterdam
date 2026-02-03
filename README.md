# House Price Prediction

## Overview
This project aims to predict house prices using different machine learning models and evaluate their performance based on various metrics.

## Steps

1. **Database Setup**  
   The first step involved importing the PostgreSQL database and establishing a connection to the server using Python. PgAdmin was utilized to import the data and create the database tables, which were then used to execute structured queries.

2. **Data Import and Exploration**  
   The 'pandas' library was used to import the tables from the database and perform an initial data exploration to understand the dataset.  
   The 'seaborn' library was employed to visualize the data and examine relationships between features.

3. **Feature Definition and Analysis**  
   Features were defined, and data analysis was performed to study their distributions and correlations. Important libraries were imported to prepare the data for machine learning, including 'train_test_split'. Feature scaling and engineering were performed using 'StandardScaler'.

4. **Outlier Detection and Handling**  
   Outliers were identified using boxplots and heatmaps. They were subsequently addressed using the Interquartile Range (IQR) method.

5. **Linear Regression Modeling**  
   A Linear Regression model was trained on the dataset to predict house prices. Cross-validation was performed to assess model stability.  
   Model performance was evaluated using R², Mean Squared Error (MSE), and Mean Absolute Error (MAE) for both test and cross-validation data.  
   Predicted vs actual values were plotted, and residuals were calculated and visualized.

6. **Target Transformation**  
   To improve predictions, a log1p transformation was applied to the target variable. The model was retrained on the transformed data, and performance was evaluated and compared to the non-transformed model.

7. **Additional Machine Learning Models**  
   In addition to Linear Regression, Support Vector Regression (SVR), Random Forest, and XGBoost models were trained on both transformed and non-transformed data. Results were visualized using matplotlib` and seaborn libraries.

8. **Model Evaluation and Comparison**  
   Finally, all models were compared based on R², MSE, and MAE to determine the best-performing model for this dataset.
