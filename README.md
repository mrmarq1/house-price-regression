# House Price Regression

Model to predict house prices based on a feature space provided. To take iterative approach to modelling beginning with optimisation of linear regression model through data cleaning and feature engineering. To progress on to boosting algorithms and Optuna tuning to compare performance. Finally, to determine key factors driving house prices.

## Project Motivation
- To source tabular data that presents sufficient challenge to practice an array of data cleaning and feature engineering techniques.
- To work with a relatable, real-world context to help the feature engineering and model analysis process.

## Learning Points

- The impact of feature engineering on model performance (the linear regression model's adj. R^2 went from 0.7114 at baseline to 0.7905). 
- How to calculate distances based on latitude and longitude with Python's 'vincenty' package.
- Relative merits of different model performance metrics.
- Practical implementation of Optuna hyperparameter tuning.
- Use of 'model.feature_importances_' to gain insight into feature weighting of models using boosting algorithms. 

## Project Breakdown

### Data cleaning
Conducted analyses to understand the dataset and clean it, handling outliers, dropping redundant features and stanardising it in the process.

### Initial modelling
- Applied a linear regression model and evaluated performance using RMSE, R^2 and adjusted R^2.

### Feature engineering
- Binned data
- Converted 'yr_built' to 'property_age' feature
- Differentiated properties renovated from those not with binary indicator variable
- Used 'lat' and 'long' to define a 'distance_to_seattle' variable

### Further modelling
- Evaulated improvement in performance from feature engineering by re-running linear regression.

### Further modelling
- Applied polynomial modelling to see if performance could be improved.
- Progressed to boosting algorithms and tuned hyperparameters accordingly through Optuna analysis. 
- Compared model scores for RMSE, R^2 and adjusted R^2.

### Model selection and analysis
- Based on performance, proceeded with tuned LGBM model.
- Analysed feature score to determine factors driving house prices.

## Improvements
- Analysis indicated 'lat' and 'long' features were the strongest house price determinants, thus, alluding to the property's location. This suggests further feature engineering of these variables could have yielded a more specific and descriptive feature (did attempt this with 'distance_to_seattle' but it was relatively low in the final feature rankings).
