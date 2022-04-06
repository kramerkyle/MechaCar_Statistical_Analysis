# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG

Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
- The vehicle length and ground clearance variables provide a non-random amount of variance to the mpg values in the data set.

Is the slope of the linear model considered to be zero? Why or why not?
- No, the slope of the linear model is not considered to be zero because the co-efficients of each variable are non-zero and do not cancel each other to zero.

Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
- Yes, it does. We can see that the measure of goodness of fit (Multiple R-Squared) is high (0.7149).

![Ln Regression to Predict MPG](https://github.com/kramerkyle/MechaCar_Statistical_Analysis/blob/e0c43e9f8931593199f0fec46236311c2b6e3ba0/Linear%20Regression%20to%20Predict%20MPG.png)

## Summary Statistics on Suspension Coils
The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?
- In aggregate, the variance for all lots is acceptable at ~62 lbs per square inch as shown in the total summary image.
- The variance for Lot 3, however, is unacceptably high. It exceeds the limit by ~70.28 lbs per square inch.

## T-Tests on Suspension Coils
The t-test of the entire table showed a p-value of 0.60, which fails to reject the null hypothesis that the dataset is not statistically different from the population mean.

![Suspension Coil Test](https://github.com/kramerkyle/MechaCar_Statistical_Analysis/blob/e0c43e9f8931593199f0fec46236311c2b6e3ba0/Suspension_Coil%20T-Test.png)

The t-test for Lot1 had a p-value of 1. This result clearly fails to reject the null hypothesis.

![Lot 1](https://github.com/kramerkyle/MechaCar_Statistical_Analysis/blob/e0c43e9f8931593199f0fec46236311c2b6e3ba0/Linear%20Regression%20to%20Predict%20MPG.png)

The t-test for Lot2 had a p-value of 0.61. This value is far too large and fails to reject the null hypothesis.

![Lot 2](https://github.com/kramerkyle/MechaCar_Statistical_Analysis/blob/e0c43e9f8931593199f0fec46236311c2b6e3ba0/Lot2%20T-Test.png)

The t-test for Lot3 resulted in a p-value of 0.04. This result allows the acceptance of the alternative hypothesis that the mean is statistically different than the population mean of 1500 pounds per square inch.

![Lot 3](https://github.com/kramerkyle/MechaCar_Statistical_Analysis/blob/e0c43e9f8931593199f0fec46236311c2b6e3ba0/Lot3%20T-Test.png)

## Study Design: MechaCar vs Competition
MechaCar can commission a statistical study that examines how it compares against the competition in resale value for vehicles with over 100,000 miles. This would be beneficial because cost-conscious consumers may be swayed by the perception of long-term value between automotive organizations.

The null hypothesis would be that the mean of MechaCar resale value is below that of competitors. Conversely, the alternative hypothesis is that MechaCar resale value is not below that of competitors.

To test this hypothesis, a two-sample t-test should be conducted. This is appropriate because two samples will be used: MechaCar's and competitors'. By evaluating if the p-value is significantly small enough, it can be determined if there is a statistical difference between the distribution means of the samples.

The data necessary for this test could be gained by scraping Facebook marketplace and similar resale marketplaces. The resale value variable is continuous in nature and will allow precise measurements to be made against it.
