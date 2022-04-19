# MechaCar Statistical Analysis

## Linear Regression to Predict MPG
A linear regression analysis was performed on the MechaCar dataset to determine which factors impact MPG.  This dataset contained data on mpg, vehicle length and weight, spoiler angle, ground clearance, and AWD.

According to the analysis, both vehicle length and ground clearance contribute to MPG due to their p-values < 0.05. The slope of the linear model is not zero due to the model p-value being less than 0.05 as well.  The R-squared value is 71.5 which means 71.5% of the variability in mpg is explained through this model. This is sufficient to effectively predict mpg.

![MPG Linear Regression](/Resources/mpg_linear_regression.png)