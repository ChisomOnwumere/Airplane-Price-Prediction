# Airplane-Price-Prediction
Prediction using Xgboost Model and Random Forest
# Airplane Price Prediction

This project involves predicting the prices of airplanes based on various features such as model, production year, engine type, capacity, range, fuel consumption, maintenance cost, and region of sale. The dataset used for this analysis is `airplane_price_dataset.csv`.

## Technologies Used

- Python 3.x
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost

## Dataset Overview

The dataset includes the following columns:
- **Model**: The model of the airplane.
- **Üretim Yılı**: Year of production.
- **Motor Sayısı**: Number of engines.
- **Motor Türü**: Type of engine (e.g., Turbofan, Piston).
- **Kapasite**: Seating capacity.
- **Menzil (km)**: Range in kilometers.
- **Yakıt Tüketimi (L/saat)**: Fuel consumption in liters per hour.
- **Saatlik Bakım Maliyeti ($)**: Hourly maintenance cost in dollars.
- **Yaş**: Age of the airplane.
- **Satış Bölgesi**: Sales region.
- **Fiyat ($)**: Price in dollars (target variable).

## Analysis Steps

1. **Data Preprocessing**: 
   - Loaded and explored the dataset.
   - Handled missing values and converted categorical variables into numerical format.

2. **Model Training**: 
   - Split the dataset into training and testing sets.
   - Trained two models:
     - Random Forest Regressor
     - XGBoost Regressor

3. **Model Evaluation**: 
   - Evaluated the models using Mean Squared Error (MSE) and R-squared (R²) metrics.
   - Visualized the predictions against actual prices for both models.

## Results

- **Random Forest Model**:
  - MSE: 1,093,123,967,779,579.00
  - R²: 0.98

- **XGBoost Model**:
  - MSE: 1,149,079,395,085,718.00
  - R²: 0.98
  - Analysis of Results
  - 
- **MSE Comparison**:
  The MSE for the Random Forest model is lower than that of the XGBoost model.
  Lower MSE indicates better predictive performance, suggesting that the Random Forest model      is performing better in this case.
  
- **R² Comparison**:
  Both models have the same R² value of 0.98.
  This indicates that both models explain 98% of the variance in the target variable,         
  suggesting they each provide similar levels of explanatory power.
- **Conclusion** 
  XGBoost does not have a significantly lower MSE than the Random Forest model; in fact, its      MSE is higher.
  Both models have the same R² value, indicating similar explanatory power.
  Overall, the Random Forest model performs better based on MSE, as a lower MSE is preferable.
  Thus, you can conclude that the Random Forest model is the better-performing model for this     dataset.

## Conclusion

  After comparing the performance of both models based on the MSE and R² metrics, the **XGBoost 
  model performed better** than the Random Forest model. This conclusion is based on the lower 
  MSE and higher R² value observed for the XGBoost model, indicating more accurate predictions.

## Future Work

- Hyperparameter tuning for both models to improve accuracy.
- Explore additional features or use ensemble methods to further enhance predictive performance.
- Consider using advanced techniques like Neural Networks for comparison.

