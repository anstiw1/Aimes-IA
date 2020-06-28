# Predicting The Prices of Homes in Ames, IA.

________________________________________________

### Project Summary 

We are tasked with creating a model to accurately predict prices on houses in Ames. The data we are provided are a range of housing prices and features from 2006 until 2010. To accurately predict prices of homes, we will be using feature engineering and linear regression to build a model.

### Problem Statement 

Despite the 2008/2009 recession and subsequent housing price drop, Ames' housing prices were seemingly unaffected and weathered the economic downturn with poise. With the lowered interest rates avaiable from the Federal Reserve, some homeowners may be interested in selling, refinancing, or opening a home equity line of credit on their homes. How can we provide accurate data to homeowners as well as banks, and home buyers with the list of home features available to us? 

________________________________________________

### Conclusions

I attempted three different modeling types to study and predict this data: Lasso Regression, Linear Regression, and Ridge Regression. The Linear Regression model is able to predict the value of a home with a high degree of accuracy based on the following qualities: Total Square Footage (the size of the home in its entirety), Living Area (Total Square Footage of the home's living spaces), Garage Cars (number of cars the home's garage can fit), Basement SF (square footage of the home's basement). 

________________________________________________

### Data

We are utilizing housing data from 2006 until 2010 from from Ames Land & Title Division which was used to appriase the value of homes in the town. The data accessible to us includes 80 columns of various features each home sold, including ordinal data (ratings of quality), numerical data (the year the home was built, square feet), and nominal data (neighborhood, zone, sale month/year).

### Sampling of Data Types and Data Descriptions

| Predictive Variable | Data type | Description |
  ------------------- | --------- | ----------- 
| overall_qual | Scale of 1 to 10 | Rates the overall material and finish of the house |
| full_bath | int | Full bathrooms |
| year_built | int | Original construction date |
| totalsqft | total square feet | Total living area by SQFT |
| exter_cond | Ordinal 1 to 5 | Condition of the home's exterior |
| lot_area | Total lot size | Lot size |
| garage_cars | float | Total number of cars that fit in the home's garage | 
| bsmt_qual | Ordinal 1 to 5 | Evaluates the overall quality of the basement |
| remodelyrs | 0 or 1 | Number of years between the home being built and then remodeled |

### Modeling

| Model Type | RMSE | RSquared Train Data | RSquared Test Data |
  ---------- | ---- | ------------------- | ------------------ 
| Lasso | 38934.07 | 0.73 | 0.72 |
| Linear Regression | 38907.47 | 0.79 | 0.73 
| Ridge Regression | 38885.49 | 0.79 | 0.73

## Graph of predicted housing prices versus actual housing prices, including a line of best fit:

![Predicted vs. Actual](https://i.imgur.com/azYceq7.png)

## Outside Research/Outside Data:

1. City of Ames (Housing): https://www.cityofames.org/government/departments-divisions-a-h/housing
    
2. Rental/Housing Deals: https://www.rentalhousingdeals.com/housing-authority/IA/Ames/Ames-Housing-Authority
    
3. City of Ames (Neighborhood/Income): https://www.cityofames.org/living/neighborhoods
    
4. Neighborhood Scout: https://www.neighborhoodscout.com/ia/ames
    
5. Ames Neighborhood Map: http://jse.amstat.org/v19n3/decock/AmesResidential.pdf