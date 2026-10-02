# California Housing Price Prediction

## Project Overview
This project predicts the median house value in California districts using Machine Learning.  
I compared **Linear Regression** and **Random Forest Regressor** and analyzed feature importance.

## Dataset
- Source: Scikit-learn California Housing dataset
- Samples: 20,640
- Features: 8 (MedInc, HouseAge, AveRooms, AveBedrms, Population, AveOccup, Latitude, Longitude)
- Target: MedHouseVal (Median house value in units of $100,000)

## Approach
1. Data exploration with Pandas
2. Train-Test split (80/20)
3. Trained two models:
   - Linear Regression (baseline)
   - Random Forest Regressor
4. Evaluated using MAE, RMSE, and R²
5. Analyzed Feature Importance

## Results

| Model               | MAE   | RMSE  | R²    |
|---------------------|-------|-------|-------|
| Linear Regression   | 0.530 | 0.736 | 0.591 |
| Random Forest       | 0.329 | 0.504 | 0.808 |

**Random Forest** performed significantly better.

### Top Important Features
1. MedInc (Median Income) – 52.2%
2. AveOccup (Average Occupancy) – 13.9%
3. Latitude / Longitude – ~8.9% each

## How to Run
```python
# Clone the repository
git clone https://github.com/YourUsername/California-Housing-Price-Prediction.git

# Install requirements
pip install scikit-learn pandas numpy matplotlib

# Run the notebook or script

What I Learned
- Comparing regression models
- Interpreting MAE, RMSE, and R²
- Feature importance analysis
- Building a clean end-to-end ML workflow

Future Improvements
- Hyperparameter tuning
- Feature engineering
- Trying Gradient Boosting models (XGBoost / LightGBM)
