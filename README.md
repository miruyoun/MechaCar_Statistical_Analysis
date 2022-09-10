# MechaCar Statistical Analysis

## Linear Regression to Predict MPG
![Summary](https://user-images.githubusercontent.com/106292020/189478684-17fabca4-cbb6-4d00-9294-ff823d2d9135.PNG)
* The vehicle length and ground clearance provides a non-random amount of variance to the mpg value.
* The slope of the linear model cannot be considered zero because there are two variables that are statistically significant and have a coefficient of 6.27 (vehicle length) and 3.55 (ground clearance).
* The linear model does predict mpg because the R squared value is 0.71. There are some outside factors that we cannot consider but the model does relatively predict mpg well.

## Summary Statistics on Suspension Coils
### Total Summary
![Total](https://user-images.githubusercontent.com/106292020/189478732-ca93f0ba-f813-40f6-b362-db1a38715cd7.PNG)
### Lot Summary
![Lot](https://user-images.githubusercontent.com/106292020/189478735-6e9b301d-6c8e-41f5-8150-c5b73a7d2ebe.PNG)

According to the total_summary and lot_summary data, in total, the current manufacturing meets the design specification because its variance is 62.29 PSI. Based on lot, only the first two lots meet the design specification because their variance is 0.99 and 2.73. However, Lot 3's variance exceeded the 100 PSI limit and was over 170 PSI. 

## T-Tests on Suspension Coils

![test1](https://user-images.githubusercontent.com/106292020/189478801-0b15b1bb-e079-4ad1-94c9-ca69b03c751f.PNG)

* The t-test for the full manufacturing data gave us a p-value of 0.06 and this is above the 0.05 significance level so we fail to reject the null hypothesis. This means that across all manufacturing lots, the mean PSI is not statistically different from the population mean.

![test2](https://user-images.githubusercontent.com/106292020/189478805-65a07fac-e6ec-4cef-813f-57ecb235b26c.PNG)

* The t-test for the Lot 1 manufacturing data gave us a p-value of 1 and this is above the 0.05 significance level so we fail to reject the null hypothesis. This means that across manufacturing lot 1, the mean PSI is not statistically different from the population mean.

![test3](https://user-images.githubusercontent.com/106292020/189478808-f22b8eca-a2d4-4992-a098-a4a93650c5c4.PNG)

* The t-test for the Lot 2 manufacturing data gave us a p-value of 0.61 and this is above the 0.05 significance level so we fail to reject the null hypothesis. This means that across manufacturing lot 2, the mean PSI is not statistically different from the population mean.

![test4](https://user-images.githubusercontent.com/106292020/189478812-90e8d9e9-ab0b-4c0a-b6b9-8284803c7d9c.PNG)

* The t-test for the Lot 3 manufacturing data gave us a p-value of 0.04 and this is below the 0.05 significance level so we reject the null hypothesis. This means that across manufacturing lot 3, the mean PSI is statistically different from the population mean.

## Study Design: MechaCar vs Competition
Many aspects can make a car unique, and many brands today focus on different factors to make their car best appeal to customers. To conduct a test on whether MechaCar is better than its competitors we need to design a study. 
* The metric we are going to test is cost
* Null hypothesis: The mean of the paired difference of prices between MechaCar and their competitors equals zero. Alternative hypothesis: The mean of the paired difference of prices between MechaCar and their competitors does not equal to zero.
* I would use a two sample t-test because we are trying to test if the cost of a car affects the purchase of a car between two different brands.
* To run the statistical test, I would need the price of MechaCar and its competitors.
