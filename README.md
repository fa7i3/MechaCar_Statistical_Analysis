# MechaCar_Statistical_Analysis
The purpose of this analysis is to analyze data from an automotive manufacturing company called 'AutosRU'. Their newest prototype, MechaCar is having production issues which is blocking the manufacturing team’s progress. This analysis provides insights that may help the manufacturing team and resolve the issues.

# Data:
* MechaCar MPG dataset
* Suspension Coil dataset

# Software:
* RStudio

# Linear Regression to Predict MPG
I performed multiple Linear regression on vehicle_weight, spoiler_angle, ground_clearance, AWD and vehicle_length to check if they could predict MPG..

![Deliverable 1 results](https://user-images.githubusercontent.com/104453593/185812862-e2b9c9a3-f0d4-45e7-b1bc-31f68cf2cea4.PNG)



* According to the Pr(>|t|) values in the picture above, the Intercept (p-value is 5.08), ground_clearance (p-value is 5.21) and the vehicle_length (p-value is 2.60) all provided a non-random amount of variance to the mpg values in the dataset which means that there are variables that we haven't considered or observed.

* According to the linear regression model, the p-value 5.35e-11 is less than the our assumed significant p-value of 0.05. Therefore, there is sufficient evidence to reject the null hypothesis and the slope of our linear model is not considered to be zero.

* According to our results above, the Adjusted R-Squared value is 0.68 and the Multiple R-squared value is 0.71. This shows a positive relationship and this linear model can effectively predict mpg of MechaCar prototypes.  

# Summary Statistics on Suspension Coils
The summary statistics was calculated for the pounds per square inch of suspension coils for the manufacturing lots.

* The design specifications for the MechaCar suspension coils require that the variance of the suspension coils must not exceed 100 pounds per square inch. According to the total_summary dataframe below, the variance is 62.29 PSI which meets the required specification.

![total summary df del 2](https://user-images.githubusercontent.com/104453593/185813298-73499558-3f7b-4599-9d59-608dc065e06f.PNG)
* According to the lot_summary dataframe below, lot 1 (variance = 0.97 PSI) and lot 2 (variance = 7.46 PSI) meets the required specification. However, lot 3 (variance = 170.28 PSI) doesn't meet the required specifications of 100pounds per square inch.

![del 1 lot summary dframe](https://user-images.githubusercontent.com/104453593/185813304-dc9aacad-24c1-476b-8b12-283221c663d0.PNG)


# T-Tests on Suspension Coils
T-test results and images on Suspension coils for combined lots and individual lots are below:

* Combined Lots T-test:
According to the T-test result below, the p-value (0.06) is higher than the assumed significant value (0.05), which means the null hypothesis that the mean of all the combined lots is statistically similar to the population mean of 1500 cannot be rejected.
![Combined lot t-test'](https://user-images.githubusercontent.com/104453593/185814291-137b6de2-6658-49c6-89b6-19857585087f.PNG)


* Lot 1 t-test:
According to the T-test result below, the p-value (1) is significantly higher than the assumed significant value (0.05), which means the null hypothesis that the mean of lot 1 is statistically similar to the population mean of 1500 cannot be rejected.
![lot1 t-test](https://user-images.githubusercontent.com/104453593/185814315-bede18eb-3fde-428b-a6d9-cd83e0e0e3d0.PNG)


* Lot 2 t-test:
According to the T-test result below, the p-value (0.60) is higher than the assumed significant value (0.05), which means the null hypothesis that the mean of lot 2 is statistically similar to the population mean of 1500 cannot be rejected.

![lot 2 t-test](https://user-images.githubusercontent.com/104453593/185814319-2b5ee528-e864-4217-963b-14a6b8bd4622.PNG)


* Lot 3 -test:
According to the T-test result below, the p-value (0.04) is significantly lower than the assumed significant value (0.05), which means the null hypothesis can be rejected.


![lot 3 t-test](https://user-images.githubusercontent.com/104453593/185814329-fb2090b1-dc6b-4853-a98f-5c241c7bbddb.PNG)


# Study Design: MechaCar vs Competition
For this study, the company can compare these categories (i.e. maintenance cost, safety rating, gas mileage and cost) using the ANOVA test. Since the ANOVA test is able to check if the means from multiple different samples are significantly similar or different; which means that the averages of MechaCar can be compared in these categories with the averages of the competition. Therefore, if the p-value is greater than 0.05, then MechaCar has a significant similar performance within these categories (accept the null hypothesis). If the p-value is less than 0.05, then MechaCar is significantly different within these categories (reject the null hypothesis). This will show the performance of MechaCar within the categories when compared with the competitor.
 
