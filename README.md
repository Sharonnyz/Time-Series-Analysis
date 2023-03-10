# Evaluate business applications for all NAICS of New Jersey

This project is to evaluate business development for New Jersey. The aim of this study is to find relationships between business applications and two predictive factors associated with housing and earnings and provide forecasts for the next 12 months of business applications.

## Dataset

- NAICSNJ.csv

Response Variable: Business Applications: Total for All NAICS—Monthly & Not Seasonally Adjusted for New Jersy. It has 219 data points from July 2004 to September 2022.

- NAICSUS.csv

Business Applications: Total for All NAICS at the national level

- New_Private_Housing.csv

Explanatory Variables 1: New Private Housing Units Authorized by Building Permits for New Jersy

- Average_Hourly_Earnings.csv

Explanatory Variables 2: Average Hourly Earnings of all Employees: Total Private for New Jersy

## Methods

### Basic explanatory data analysis tools
ACF plots, PACF plots, boxplot, smoothing techniques(Lowess),scatterplot matrix, cross-correlations, etc.

### Regression analysis
I utilized the linear regression models between the response variable and two predictive variables respectively. I also formed a multiple linear regression model using both explanatory variables. Meanwhile, I have added time dummy with Housing and Earnings to produce regression models.

I have chosen the models with significant p-values for each term. Then I applied the two-sided Durbin-Watson Test for the autocorrelation parameter on the models. If the DW statistic indicates the presence of serial correlation of the residuals, I remedied it using the Cochrane-Orcutt method.

### Forecast

- Forecast based on regression model
- Holt-Winters method
- SARIMA

