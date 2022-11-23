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


2.Summary Statistics on Suspension Coils
![image](https://user-images.githubusercontent.com/109991916/203139440-f2efd4ea-32ed-4828-ac01-229093bb2fb4.png)
![image](https://user-images.githubusercontent.com/109991916/203139655-a95ce09f-3d93-4304-97fe-d513bce9eb6c.png)

While the overall variance, as shown in the Total Summary data above, is under 100 psi and meets specifications,one of the individual lots does not meet the necessary specifications. As shown in the Lot Summary stats, the variance for Lot 3 is well over the acceptable threshold, at 170.28.
 
3.T-Tests on Suspension Coils
![image](https://user-images.githubusercontent.com/109991916/203141564-6dc31ceb-5ac2-412b-b0ae-d8bad77c03a2.png)


## Summary
### Results
Based on the information provided, the following can be determined:
1. Bike Repairs for 1/3 of the Citibikes should be done during non-peak hours around 1-5 am.
2. Male subscribers are the highest users and follow the traditional high use times of travel to and from work.
3. Target market for Citibike should be males needing transportation to work and weekend activities and push for subscribing to the services.

### Additional Queries
Overall, the use of this data can be very helpful for future Citibike analysis. I also observed the following:
1. ![Ridesharing_Locations_by_Gender](https://user-images.githubusercontent.com/109991916/201751870-a9589e5f-98be-47b0-a7d2-6a7e9ad35124.png)
Males are more likely to start a trip farther than the main city center of NYC than others.
2. ![User_Type_Starting_Location](https://user-images.githubusercontent.com/109991916/201752113-d3d1d7cd-5c2d-4a43-925b-684b1b2a988a.png)
Subscribers are more likely to start trip farther than the main city center of NYC than others.
