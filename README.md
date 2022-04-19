# MechaCar Statistical Analysis

## Linear Regression to Predict MPG
A linear regression analysis was performed on the MechaCar dataset to determine which factors impact MPG.  This dataset contained data on mpg, vehicle length and weight, spoiler angle, ground clearance, and AWD.

According to the analysis, both vehicle length and ground clearance contribute to MPG due to their p-values < 0.05. The slope of the linear model is not zero due to the model p-value being less than 0.05 as well.  The R-squared value is 71.5 which means 71.5% of the variability in mpg is explained through this model. This is sufficient to effectively predict mpg.

![MPG Linear Regression](/Resources/mpg_linear_regression.png)

## Summary Statistics on Suspension Coils
The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. The total summary of all three lots showed the variance to be within the specs at 62.

![Total Summary](/Resources/total_summary.png)

However, a closer look at the individual lots showed that lot 1 and lot 2 had acceptable variances while lot 3 exceded the PSI variance requirement by over 70 PSI.

![Lot Summary](/Resources/lot_summary.png)
