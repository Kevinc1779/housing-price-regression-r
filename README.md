# Housing Price Prediction Using Multiple Linear Regression

This project analyzes factors influencing housing prices using a dataset containing property characteristics such as square footage, number of bedrooms, bathrooms, neighborhood, and year built. The goal was to build a regression model that identifies which features significantly affect property values.

## Dataset

The dataset contains approximately **50,000 housing observations** with the following variables:

- SquareFeet
- Bedrooms
- Bathrooms
- Neighborhood
- YearBuilt
- Price

Source: Kaggle Housing Price Prediction Dataset.

## Project Workflow

The analysis included the following steps:

1. Data exploration and summary statistics
2. Visualization of variable distributions
3. Correlation analysis to evaluate relationships between predictors
4. Regression modeling to estimate housing prices
5. Model selection using statistical significance and AIC
6. Diagnostic testing of regression assumptions
7. Train–test split evaluation of model performance

## Data Cleaning

- Negative house prices were removed because property values cannot be negative.
- No missing values were present in the dataset.

## Model Development

Multiple regression models were evaluated to identify the most important predictors of housing price.

Key findings:

- **Square footage was the strongest predictor of price**
- Bedrooms and bathrooms also had statistically significant positive effects
- Year built was not a significant predictor
- Urban neighborhoods showed slightly higher housing prices

## Final Model

The final regression model included:

- SquareFeet
- Bedrooms
- Bathrooms
- Neighborhood

## Model Performance

The dataset was split into:

- **70% training data**
- **30% testing data**

Test performance:

- **Test R² ≈ 0.568**
- **RMSE ≈ $49,629**
- **MAE ≈ $39,656**

This indicates the model explains approximately **57% of housing price variation** and predicts housing prices within roughly **$40k–$50k** on average.

## Key Insight

Housing prices were primarily driven by structural characteristics of the home. Square footage had the largest effect, with each additional square foot increasing predicted house price by approximately **$99**.

## Tools Used

- R
- RStudio
- Linear Regression
- Statistical Modeling
- Data Visualization

## Repository Structure

housing-price-regression-r  
│  
├── data  
│   └── housing_price_dataset.csv  
│  
├── notebooks  
│   └── HousingRegression.Rmd  
│  
├── report  
│   └── HousingRegression.docx  
│  
├── presentation  
│   └── HousingPriceRegression.pptx  
