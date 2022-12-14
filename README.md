MechaCar_Statistical_Analysis
=============================

Linear Regression to Predict MPG
--------------------------------
![1](./images/1.png)

- In the MechaCar dataset, ground_clearance and vehicle_length provided non-random
amount of variance to the mpg values.

- In addition, there is evidence that vehicle_weight may have also provided a
slight amount of variance to the mpg values, but this is not significant (if we
use a significance level of 0.05).

- According to the multiple linear regression model, the slope of the linear model
is not considered to be zero because the p-value of the hypothesis test was
5.35e-11, which is smaller than the 0.05 significance level.

- The multiple regression model does an adequate job of predicting the mpg of
MechaCar prototypes because the multiple r-squared value was 0.71.

- Which means that roughly 71% of the time the model will predict mpg values
correctly.

- Most likely there are other more impactful variables and factors that were not
captured in the dataset that contribute to the mpg variability of the MechaCar
prototypes.

![2](./images/2.png)

Summary Statistics on Suspension Coils
--------------------------------------

Across the suspension coil manufacturing lots, Lot 1 and Lot 2 are both within
design specifications, and both have the same calculated mean and median.

However, Lot 3 is far more variable than the other manufacturing lots.

Lot 3 has a calculated variance that exceeds the manufacturing specs.

![3](./images/3.png)

If we combine all three lots and look at the total data, the overall calculated
variance is within specifications.

![4](./images/4.png)

T-Tests on Suspension Coils
---------------------------

According to each of the one-sample t-tests, Lot 1 and Lot 2 PSI values are not
statistically different from the population mean.

![5](./images/5.png)

![6](./images/6.png)

However the p-value of Lot 3 is 0.041 which is below the significance level,
which means there is evidence that the Lot 3 mean suspension coil PSI is
statistically different from the population mean.

![7](./images/7.png)

![8](./images/8.png)

Study Design: MechaCar vs Competition
-------------------------------------

One metric that people are interested in when it comes to vehicles is
horsepower.

Horsepower is a common performance metric that is reported alongside car
fuel-efficiency and engine size.

Therefore it would be really easy to collect horsepower data for a large number
of vehicles.

We can create a study that tests whether or not the horsepower of MechaCar is
statistically different from a collection of other comparable vehicles.

The null hypothesis would be that there is no statistical difference between
MechaCar horsepower and the horsepower of all other comparable vehicles.

The alternative hypothesis would be that there is a statistical difference
between horsepower of MechaCar versus the other vehicles.

The statistical test we can use is a one-sample t-test, where the population
data will be all comparable vehicles.

To test this, we will need multiple horsepower data points from vehicles as well
as multiple data points from the MechaCar vehicles, so it will be important that
we include the horsepower of multiple vehicle configurations.
