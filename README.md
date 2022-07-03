# MechaCar_Statistical_Analysis

Overview
The company AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ senior management enlisted assistance from the data analytics team to review the production data for insights that may help the manufacturing team overcome their production issues.

The data analytics team provided the following:

Multiple linear regression analysis to determine which variables in the dataset predict MPG of MechaCar prototypes
Summary statistics on pounds per square inch (PSI) of the suspension coils from each manufacturing lot
T-test on the mean population in order to determin which manufacturing lots are statistically different
Designed a statistical study to compare vehicle performance of MechaCar vehicles against vehicles from other manufacturers

# Linear Regression to Predict MPG
The following variables provided a non-random amount of variance to the MPG values in the MechaCar_mpg dataset:

vehicle_length
vehicle_weight
ground clearance
These variables will always have a given value that does not change.

The p-value of this multiple linear regression analysis is 5.35 x 10(-11), which is much smaller than the assumed significance level of 0.05%; therefore, there is sufficient evidence to reject the null hypothesis since the slope of the linear model is not zero.

![image](https://user-images.githubusercontent.com/102105537/177051964-6bf3f7e4-c813-4204-ba2a-dc21f2708f2b.png)


This linear model predicts that roughly 71% of MPG predictions of MechaCar prototypes will be correct when using this model. This multiple linear regression model has an R-value of 0.71, which suggests there is a strong positive correlation between MPG and the variables of vehicle length, vehicle weight, spoiler angle, ground clearance, and AWD.

# Summary Statistics on Suspension Coils
Design specifications for MechaCar suspension coils dictates the variance of the suspension coils must not exceed 100 pounds per square inch (PSI).

The variance of the suspension coils for all three lots was 62.29. This is within MechaCar design specifications.

![image](https://user-images.githubusercontent.com/102105537/177052235-d4a4368d-8ca0-4fdc-81c3-bea139b14375.png)

When examining the PSI of suspension coils in Lots 1, 2, and 3 individually, analysis indicated that the variance in Lots 1 and 2 are below 100 PSI, so suspension coils in Lots 1 and 2 are within MechaCar design specifications.

The variance for suspension coils in Lot 3 was 170.28, which exceeds MechaCar design specifications.

![image](https://user-images.githubusercontent.com/102105537/177052262-9714a31b-be3f-4f17-82ce-83767eaa00dd.png)

# T-Tests on Suspension Coils
A one-sample t-test was used to determine whether or not if PSI across all manufacturing lots was statistically different from the population mean of 1500 PSI.

The distribution of the suspension coil dataset was visualized with a density plot, which showed that the suspension coil dataset was nearly evenly distributed.

![image](https://user-images.githubusercontent.com/102105537/177052299-e7507c91-0d4d-4265-8a23-8c1fc910d554.png)

For all t-tests conducted, the significance level was 0.05 percent. The t-test compared the means of the Suspension Coil dataset, which was 1498.78, against a mean of 1500. All t-tests conducted resulted in the means being statistically similar.

A t-test across all suspension coil manufacturing lots gave a p-value of 0.06 Since this is above the significance level, the two means are statistically similar.

![image](https://user-images.githubusercontent.com/102105537/177052381-7a3cb639-de37-4aef-99ee-855ca02332d3.png)


A t-test for Lot 1 gave a p-value of 1, which is above the significance level. The two means are statistically similar.	
![image](https://user-images.githubusercontent.com/102105537/177052564-7a8483d3-8c63-4430-be1e-1fbc377d020e.png)


![image](https://user-images.githubusercontent.com/102105537/177052449-99e7113d-c7b1-499b-a69f-1033baaadc6d.png)

The p-value for the Lot 2 t-test was 0.6072. This is above the significance level of 0.05 results in the two means being statistically similar.

![image](https://user-images.githubusercontent.com/102105537/177052470-919f0b7c-5cbf-439a-94a8-6dd331b70708.png)

The calculated p-value from the Lot 3 t-test was 0.4168. This is above the 0.05 significance level and results in the means being statistically similar.			
			
![image](https://user-images.githubusercontent.com/102105537/177052493-f28fbc5d-4760-4059-97f4-a1ad98ed65f1.png)


# Study Design: MechaCar vs. Competition
# Description of Statistical Study
It has always been known that the cost of maintaining a vehicle can be quite expensive over time. AutosRUs wants to look into making sure their customers are getting the best value. They want the make sur ethe value given to their customer's is greater than their competitors. They would like to also try to measure the rate of depreciation for MechaCars against their competition.

# Metric
Rate of depreciation (value of vehicle over time)
# Hypothesis
Null hypothesis: Rate of depreciation for MechaCars is equal to their competitors
Alternative hypothesis: Rate of depreciation for MechaCars is not equal to their competitors
# Statistical test
Data analysts will use multiple linear regression to predict MechaCar's rate of depreciation

# Data needed
In order to perform multiple linear regression to predict rate of depreciation, analysts will need vehicle values, age, and mileage.
