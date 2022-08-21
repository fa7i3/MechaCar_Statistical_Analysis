# MechaCar_Statistical_Analysis
# Linear Regression to Predict MPG
I performed multiple Linear regression on vehicle_weight, spoiler_angle, ground_clearance, AWD and vehicle_length to check if they could predict MPG..

![Deliverable 1 results](https://user-images.githubusercontent.com/104453593/185812862-e2b9c9a3-f0d4-45e7-b1bc-31f68cf2cea4.PNG)



* According to the Pr(>|t|) values in the picture above, the Intercept (p-value is 5.08), ground_clearance (p-value is 5.21) and the vehicle_length (p-value is 2.60) all provided a non-random amount of variance to the mpg values in the dataset which means that there are variables that we haven't considered or observed.

* According to the linear regression model, the p-value 5.35e-11 is less than the our assumed significant p-value of 0.05. Therefore, there is sufficient evidence to reject the null hypothesis and the slope of our linear model is not considered to be zero.

* According to our results above, the Adjusted R-Squared value is 0.68 and the Multiple R-squared value is 0.71. This shows a positive relationship and this linear model can effectively predict mpg of MechaCar prototypes.  

