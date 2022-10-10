# MechaCar_Statistical_Analysis
The purpose of this project is to help AutosRUs’ upper management to review the production data for insights that may help the manufacturing team. They need to understand why the newest prototype, the MechaCar, is suffering from production troubles which are blocking their progress.

## Linear Regression to Predict MPG

The first task in the project is to perform a multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes.

![D1]()

** Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
	** The two variables that provided a non-random amount of variance to the mpg values in the dataset were vehicle_length and ground_clearance.

** Is the slope of the linear model considered to be zero? Why or why not?
	** No the slope of the linear model is not considered to be zero because the p-value is 5.35e-11 which is less than the assumed significance level of 0.05%.

** Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
	** Yes the linear model did predict the mpg effectivly because its r squared value is greater that 70%.


## Summary Statistics on Suspension Coils

The second task in the project is to create a summary statistics table to show:
	** The suspension coil’s PSI continuous variable across all manufacturing lots
	** The following PSI metrics for each lot: mean, median, variance, and standard deviation.

![D2]()

** The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?
	** The current manufacturing data does meet this design specification for all manufacturing lots in total. However when we group the data into the three separate manufacturing lots, we can see that Lot 3 exceeds the limit of 100 pounds per square inch by a large margin. The Variance for Lot 3 is 170.2861224.

