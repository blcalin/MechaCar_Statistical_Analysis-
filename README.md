# MechaCar_Statistical_Analysis
## Overview of Project
### Purpose
The purpose of this project was to analyze automobile performance using R. AutosRUs' production of MechaCar is suffering from production issues, and the goal is to:
1. Determine the variables that predict MPG for vehicle prototypes
2. Collect summary statistics on the PSI of suspension coils
3. Determine whether manufacturing lots vary statistically from mean population
4. Design a study comparing MechaCar performance against vehicles from other manufacturers

## Results and Analysis
### Results
Through our data set and the analysis of Citibike data, we determined the following:
 1. Linear Regression to Predict MPG
 ![image](https://user-images.githubusercontent.com/109991916/203135794-34220340-1d53-441d-a1d5-a13f3045b8fb.png)
The most significant variables in our dataset which show a non-random effect on the MPG of the MechaCar are the Vehicle Length and the Ground Clearance. A linear regression model run on these variables against figures for MPG, resulted in p-values of 2.6x10-12 and 5.21x10-8, respectively. The intercept was also statistically significant, indicating that there are likely other factors, not included in our dataset, that have an impact on the MPG.
The slope of the linear model can not be considered to be zero, as the p-value of 5.35x10-11, is lower than even an extreme level of significance, and thus the null hypothesis must be rejected. This means that the relationship between our variables and the miles per gallon is subject to more than random chance.
Although there are still unconsidered factors, this model does predict the mpg of the MechaCar prototype with some relative effectiveness. The r-squared value of 0.7149, indicates that the model is 71% accurate.


2. Summary Statistics on Suspension Coils

![image](https://user-images.githubusercontent.com/109991916/203139440-f2efd4ea-32ed-4828-ac01-229093bb2fb4.png)
![image](https://user-images.githubusercontent.com/109991916/203139655-a95ce09f-3d93-4304-97fe-d513bce9eb6c.png)

While the overall variance, as shown in the Total Summary data above, is under 100 psi and meets specifications,one of the individual lots does not meet the necessary specifications. As shown in the Lot Summary stats, the variance for Lot 3 is well over the acceptable threshold, at 170.28.
 
3. T-Tests on Suspension Coils
![image](https://user-images.githubusercontent.com/109991916/203141564-6dc31ceb-5ac2-412b-b0ae-d8bad77c03a2.png)

Results of the T-test for the suspension coils across all manufacturing lots shows that they are not statistically different from the population mean, and the p-value is not low enough (0.0603) for us to reject the null hypothesis.

The T-test for the suspension coils for Lot 1 shows that they are not statistically different from the population mean, and the p-value is not low enough (1) for us to reject the null hypothesis.

Results of the T-test for the suspension coils for Lot 2 shows that they are not statistically different from the population mean, and the p-value is not low enough (0.6072) for us to reject the null hypothesis.

The T-test for the suspension coils for Lot 3 shows that they are slightly statistically different from the population mean, and the p-value is low enough (0.0417) for us to reject the null hypothesis. This lot may need to be further evaluated to determine whether the data should be discarded altogether.


## Study Design: MechaCar vs. Competition
### Summary
There are many factors that consumers take into consideration when purchasing a vehicle. In a world where ridesharing is popular, and easily accessible, customers looking to purchase a car are looking for more than just convenience. They will be looking to buy a car that is an economical means to regularly transport themselves, and items, on a regular basis.

### Metric to Test
The test will further evaluate MechaCar's carrying capacity, in cubic inches, in comparison to various competitors' vehicles.

### Null and Alternative Hypothesis
H0: MechaCar prototypes' average carrying capacity is comparable to competitor's vehicles in the same vehicle class Ha: MechaCar prototypes' average carrying capacity is statistically above or below that of competitor vehicles.

### Statistical Test
The appropriate statistical test for this study would be two-sample t-tests, as the means of two groups are used.

### Data Needed
Cubic space data from the carrying compartments of all MechaCar prototypes is necesary, as well as from all major competitor vehicles to test our hypotheses properly.
