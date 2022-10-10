# MechaCar_Statistical_Analysis
The purpose of this project is to help AutosRUs’ upper management to review the production data for insights that may help the manufacturing team. They need to understand why the newest prototype, the MechaCar, is suffering from production troubles which are blocking their progress.

## Linear Regression to Predict MPG

The first task in the project is to perform a multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes.

![D1](https://raw.githubusercontent.com/pladams777/MechaCar_Statistical_Analysis/main/Images/Deliv1image.PNG)

* Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
	- The two variables that provided a non-random amount of variance to the mpg values in the dataset were vehicle_length and ground_clearance.

* Is the slope of the linear model considered to be zero? Why or why not?
	- No the slope of the linear model is not considered to be zero because the p-value is 5.35e-11 which is less than the assumed significance level of 0.05%.

* Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
	- Yes the linear model did predict the mpg effectively because its r squared value is greater that 70%.


## Summary Statistics on Suspension Coils

The second task in the project is to create a summary statistics table to show:
1. The suspension coil’s PSI continuous variable across all manufacturing lots.
2. The following PSI metrics for each lot: mean, median, variance, and standard deviation.

![D2](https://github.com/pladams777/MechaCar_Statistical_Analysis/blob/main/Images/Deliv2image1.PNG)

![D2-2](https://github.com/pladams777/MechaCar_Statistical_Analysis/blob/main/Images/Deliv2image2.PNG)

* The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?
	- The current manufacturing data does meet this design specification for all manufacturing lots in total. However, when we group the data into the three separate manufacturing lots, we can see that Lot 3 exceeds the limit of 100 pounds per square inch by a large margin. **The Variance for Lot 3 is 170.2861224.**

## T-Tests on Suspension Coils

The final task is to perform t-tests to determine if all manufacturing lots and each lot individually are statistically different from the population mean of 1,500 pounds per square inch.

	Null Hypothesis - the sample mean is not statistically different from the population mean.
	Alternate Hypothesis - the sample mean is statistically different from the population mean.

![D3-1](https://github.com/pladams777/MechaCar_Statistical_Analysis/blob/main/Images/Deliv3image1.PNG)

* Once again we find that as a whole, with a mean of 1498.78 and a p-value of 0.06028, the PSI of all manufacturing lots is not statistically different from the population mean of 1,500.
	- Taken as a whole, we would not reject the Null Hypothesis
	
![D3-2](https://github.com/pladams777/MechaCar_Statistical_Analysis/blob/main/Images/Deliv3image2.PNG)

* The T-Tests do confirm that when divided by Manufacturing Lots, Lot 3 is statistically different, with a mean of 1496.14 and a p-value of 0.04168 that falls below the assumed 0.05 percent significance level.
	- We cannot reject the Null Hypothesis for Lots 1 & 2; *however, we can reject it for Lot 3.*

## Study Design: MechaCar vs Competition

### With the proper data we can perform a study to compare performance of the MechaCar vehicles against performance of vehicles from other manufacturers in key indices, such as fuel efficiency and safety rating.

What metric or metrics are you going to test?
* We can measure both city and highway miles per gallon for MechCar vehicles and competitor vehicles across all classes.
* The study can also measure safety ratings; such as, survival space, airbags, and seat belt effectiveness.

What is the null hypothesis or alternative hypothesis?
* The Null Hypothesis would indicate there is no statistical difference between MechaCar and its competitors.
* The Alternate Hypothesis would indicate there is a statistical difference between MechaCar and its competitors.

What statistical test would you use to test the hypothesis? And why?
* We would use a one-way ANOVA to measure fuel efficiency as it can test the means of a single dependent variable across a single independent variable with multiple groups. 
* A two-way ANOVA does the same thing, but for two different independent variables so it would be better suited to test multiple safety ratings.

What data is needed to run the statistical test?
* To run these tests would require a comprehensive data frame where the dependent variable is numerical and continuous, and the independent variables are categorical.



