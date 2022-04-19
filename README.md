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

## T-Tests on Suspension Coils

The p-value on the total dataset is 0.06.  Assuming a 0.05 confidence level, we could determine that the mean for the total dataset is statistically similar to the mean of 1,500.  The mean of 1498.78 falls within the 95% confidence interval.

![T-test total](/Resources/ttest_total.png)

When analyzed individually, lot 1 and lot 2 both have p-values greater than 0.05 and are considered statistically similar to the 1500 PSI mean.  Lot 3's p-value falls below 0.5 at 0.42 and is not statistically similar.  The 95% confidence interval does not contain 1500 psi.

![Lot Summary](/Resources/ttest_lots.png)

## Study Design: MechaCar vs Competition
I would like to see more analysis into horsepower compared to competition.  Is the HP in line with competitors for similarly priced vehicles?  Consumers expect that as price increase, we should also see more powerful and responsive engines.

*Null Hypothesis:* The horsepower offered on MechaCar vehicles is not statistically different than similarly priced competitor vehicles    

*Alternative Hypothesis:* MechaCar horsepower is significantly less than similarly priced competitor vehicles.

A one sided t-test could be used to test MechaCar vehicles against the horsepower of competitor vehicles.  This test would determine if our vehicles are at least as good or better than competitors.  Performing t-tests on subsets of vehicle categories and prices would allow us to make sure we are comparing apples to apples on vehicle model offerings.

Data required for this test would be manufacturer, model, horsepower, MSRP, vehicle type.