# Bulldozer Price Prediction Project

 Project Goal

To build a regression model that can accurately predict the sale price of bulldozers based on:
- Equipment usage (like hours)
- Type & configuration of the machine
- Sale date (seasonal trends)
   Approach

1. **Explored the Data**  
   → Understood the dataset using pandas and the data dictionary  
   → Looked for missing values, datatypes, and outliers  

2. **Cleaned & Prepared the Data**  
   → Filled in missing values  
   → Converted saledate into new time-based features (like year, month, weekday, etc.)  
   → Encoded categorical variables using `LabelEncoder`

3. **Trained the Model**  
   → Used `XGBoost`  
   → Split the training set into train/validation to check model performance  
   → Evaluated using **RMSLE** since it penalizes big errors (especially underestimates)

4. **Made Final Predictions**  
   → Applied model on the test data  
   → Saved predictions in the required format (`SalesID`, `SalePrice`)

 Evaluation Metric

using **Root Mean Squared Logarithmic Error (RMSLE)** 
got test prediction.csv which is uploded in the repository


