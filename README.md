# House Price Regression

Model to predict house prices based on a feature space provided. To take iterate approach to modelling beginning with optimisation of linear regression model through data cleaning and feature engineering. To progress on to boosting algorithms and Optuna tuning to compare performance. Finally, to determine key factors driving house prices.

## Data cleaning
Conducted analyses to understand the dataset and clean it, handling outliers, dropping redundant features and stanardising it in the process.

## Initial modelling
- Applied a linear regression model and evaluated performance using RMSE, R^2 and adjusted R^2.

## Feature engineering
- Binned data
- Converted 'yr_built' to 'property_age' feature
- Differentiated properties renovated from those not with binary indicator variable
- Used 'lat' and 'long' to define a 'distance_to_seattle' variable

## Further modelling
- Evaulated improvement in performance from feature engineering by re-running linear regression.

## Further modelling
- Applied polynomial modelling to see if performance could be improved.
- Progressed to boosting algorithms and tuned hyperparameters accordingly through Optuna analysis. 
- Compared model scores for RMSE, R^2 and adjusted R^2.

## Model selection and analysis
- Based on performance, proceeded with tuned LGBM model.
- Analysed feature score to determine factors driving house prices.
