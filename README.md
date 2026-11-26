# Bangladesh Air Quality Forecasting Using Machine Learning

A BRAC University group project comparing six machine learning regression models for Air Quality Index (AQI) prediction in Bangladesh.

## Dataset

[Bangladesh AQI Dataset (2000–2025), Version 2](https://doi.org/10.17632/9j447cynb9.2). The original dataset contains 1,048,551 records; the report describes 893,517 records after preprocessing.

## Methodology

- Exploratory data analysis and missing-value removal
- Temporal feature extraction and city encoding
- IQR-based outlier handling and standardization
- 80:20 train-test split
- Regression model training and evaluation

## Results

| Model | MAE | RMSE | R² |
|---|---:|---:|---:|
| **Extra Trees** | **6.83** | **10.74** | **0.948** |
| Random Forest | 7.12 | 11.21 | 0.943 |
| Histogram Gradient Boosting | 9.50 | 13.71 | 0.915 |
| Decision Tree | 9.25 | 14.67 | 0.903 |
| Gradient Boosting | 10.90 | 15.62 | 0.890 |
| Linear Regression | 15.43 | 19.91 | 0.821 |

Extra Trees reduced RMSE by 46.06% relative to Linear Regression. PM2.5 and PM10 were the strongest predictors.

## Technologies

Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn and Google Colab.

## Limitations

The reported random train-test split evaluates AQI prediction rather than validated future-time forecasting. Future work includes chronological validation, weather features and hyperparameter tuning.

## Contributors

- Ahnaf Shafique
- Hossain Md Nayeen Zilkar
- Salsabin Haque Simi

BRAC University, Bangladesh.
