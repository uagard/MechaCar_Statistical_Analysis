# MechaCar_Statistical_Analysis

Overview
The company AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ senior management enlisted assistance from the data analytics team to review the production data for insights that may help the manufacturing team overcome their production issues.

The data analytics team provided the following:

Multiple linear regression analysis to determine which variables in the dataset predict MPG of MechaCar prototypes
Summary statistics on pounds per square inch (PSI) of the suspension coils from each manufacturing lot
T-test on the mean population in order to determin which manufacturing lots are statistically different
Designed a statistical study to compare vehicle performance of MechaCar vehicles against vehicles from other manufacturers

# Resources
R
Dependency
dplyr
RStudio
Datasets
MechaCar_mpg.csv
Suspension_Coil.csv

# Linear Regression to Predict MPG
The following variables provided a non-random amount of variance to the MPG values in the MechaCar_mpg dataset:

vehicle_length
vehicle_weight
ground clearance
These variables will always have a given value that does not change.

The p-value of this multiple linear regression analysis is 5.35 x 10(-11), which is much smaller than the assumed significance level of 0.05%; therefore, there is sufficient evidence to reject the null hypothesis since the slope of the linear model is not zero.

Residual standard error: 	8.774 on 44 degrees of freedom		
Multiple R-squared:  	0.7149		
F-statistic:   	22.07 on 5 and 44 DF		
Adjusted R-squared:  	0.6825		
p-value: 	5.35E-11		
![image](https://user-images.githubusercontent.com/102105537/177051964-6bf3f7e4-c813-4204-ba2a-dc21f2708f2b.png)


This linear model predicts that roughly 71% of MPG predictions of MechaCar prototypes will be correct when using this model. This multiple linear regression model has an R-value of 0.71, which suggests there is a strong positive correlation between MPG and the variables of vehicle length, vehicle weight, spoiler angle, ground clearance, and AWD.
Summary Statistics on Suspension Coils
Design specifications for MechaCar suspension coils dictates the variance of the suspension coils must not exceed 100 pounds per square inch (PSI).

The variance of the suspension coils for all three lots was 62.29. This is within MechaCar design specifications.

Deliverable_2_TotalSum

When examining the PSI of suspension coils in Lots 1, 2, and 3 individually, analysis indicated that the variance in Lots 1 and 2 are below 100 PSI, so suspension coils in Lots 1 and 2 are within MechaCar design specifications.

The variance for suspension coils in Lot 3 was 170.28, which exceeds MechaCar design specifications.

Deliverable_2_LotSum

T-Tests on Suspension Coils
A one-sample t-test was used to determine whether or not if PSI across all manufacturing lots was statistically different from the population mean of 1500 PSI.

The distribution of the suspension coil dataset was visualized with a density plot, which showed that the suspension coil dataset was nearly evenly distributed.

Deliverable 2_DensityPlot

For all t-tests conducted, the significance level was 0.05 percent. The t-test compared the means of the Suspension Coil dataset, which was 1498.78, against a mean of 1500. All t-tests conducted resulted in the means being statistically similar.

A t-test across all suspension coil manufacturing lots gave a p-value of 0.06 Since this is above the significance level, the two means are statistically similar.

Deliverable_3_All_T-test

A t-test for Lot 1 gave a p-value of 1, which is above the significance level. The two means are statistically similar.

Deliverable_3_Lot1_T-test

The p-value for the Lot 2 t-test was 0.6072. This is above the significance level of 0.05 results in the two means being statistically similar.

Deliverable_3_Lot2_T-test

The calculated p-value from the Lot 3 t-test was 0.4168. This is above the 0.05 significance level and results in the means being statistically similar.

Deliverable_3_Lot3_T-test

Study Design: MechaCar vs. Competition
Description of Statistical Study
The cost of owning and maintaining a vehicle can be expensive, so AutosRUs wants to make sure their customers are getting the best value over their competitors and would like to measure the rate of depreciation for MechaCars against other manufacturers.

Metric
Rate of depreciation (value of vehicle over time)
Hypothesis
Null hypothesis: Rate of depreciation for MechaCars is equal to their competitors
Alternative hypothesis: Rate of depreciation for MechaCars is not equal to their competitors
Statistical test
Data analysts will use multiple linear regression to predict MechaCar's rate of depreciation

Data needed
In order to perform multiple linear regression to predict rate of depreciation, analysts will need vehicle values, age, and mileage.
