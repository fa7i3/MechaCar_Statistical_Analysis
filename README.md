# MechaCar_Statistical_Analysis
# Linear Regression to Predict MPG
I performed multiple Linear regression on vehicle_weight, spoiler_angle, ground_clearance, AWD and vehicle_length to check if they could predict MPG..

![Deliverable 1 results](https://user-images.githubusercontent.com/104453593/185812862-e2b9c9a3-f0d4-45e7-b1bc-31f68cf2cea4.PNG)



* According to the Pr(>|t|) values in the picture above, the Intercept (p-value is 5.08), ground_clearance (p-value is 5.21) and the vehicle_length (p-value is 2.60) all provided a non-random amount of variance to the mpg values in the dataset which means that there are variables that we haven't considered or observed.

* According to the linear regression model, the p-value 5.35e-11 is less than the our assumed significant p-value of 0.05. Therefore, there is sufficient evidence to reject the null hypothesis and the slope of our linear model is not considered to be zero.

* According to our results above, the Adjusted R-Squared value is 0.68 and the Multiple R-squared value is 0.71. This shows a positive relationship and this linear model can effectively predict mpg of MechaCar prototypes.  

# Summary Statistics on Suspension Coils
The summary statistics was calculated for the pounds per square ich of suspension coils for the manufacturig lots.

* The design specifications for the MechaCar suspension coils require that the variance of the suspension coils must not exceed 100 pounds per square inch. According to the total_summary dataframe below, the variance is 62.29 PSI which meets the required specification.

![total summary df del 2](https://user-images.githubusercontent.com/104453593/185813298-73499558-3f7b-4599-9d59-608dc065e06f.PNG)

* According to the lot_summary dataframe below, lot 1 (variance = 0.97 PSI) and lot 2 (variance = 7.46 PSI) meets the required specification. However, lot 3 (variance = 170.28 PSI) doens't meet the required specifications of 100pounds per square inch.

![del 1 lot summary dframe](https://user-images.githubusercontent.com/104453593/185813304-dc9aacad-24c1-476b-8b12-283221c663d0.PNG)
