# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG
	* The vehicle length and ground clearance provides a non-random amount of variance to the mpg value.
	* The slope of the linear model cannot be considered zero because there are two variables that are statistically significant and have a coefficient of 6.27 (vehicle length) and 3.55 (ground clearance).
	* The linear model does predict mpg because the R squared value is 0.71. There are some outside factors that we cannot consider but the model does relatively predict mpg well.

## Summary Statistics on Suspension Coils
	* According to the total_summary and lot_summary data, in total, the current manufacturing meets the design specification because its variance is 62.29 PSI. Based on lot, only the first two lots meet the design specification because their variance is 0.99 and 2.73. However, Lot 3's variance exceeded the 100 PSI limit and was over 170 PSI. 

## T-Tests on Suspension Coils
	* The t-test for the full manufacturing data gave us a p-value of 0.06 and this is above the 0.05 significance level so we fail to reject the null hypothesis. This means that across all manufacturing lots, the mean PSI is not statistically different from the population mean.
	* The t-test for the Lot 1 manufacturing data gave us a p-value of 1 and this is above the 0.05 significance level so we fail to reject the null hypothesis. This means that across manufacturing lot 1, the mean PSI is not statistically different from the population mean.
	* The t-test for the Lot 2 manufacturing data gave us a p-value of 0.61 and this is above the 0.05 significance level so we fail to reject the null hypothesis. This means that across manufacturing lot 2, the mean PSI is not statistically different from the population mean.
	* The t-test for the Lot 3 manufacturing data gave us a p-value of 0.04 and this is below the 0.05 significance level so we reject the null hypothesis. This means that across manufacturing lot 3, the mean PSI is statistically different from the population mean.

## Study Design: MechaCar vs Competition
Many aspects can make a car unique, and many brands today focus on different factors to make their car best appeal to customers. To conduct a test on whether MechaCar is better than its competitors we need to design a study. 
	* The metric we are going to test is cost
	* Null hypothesis: The mean of the paired difference of prices between MechaCar and their competitors equals zero. Alternative hypothesis: The mean of the paired difference of prices between MechaCar and their competitors does not equal to zero.
	* I would use a two sample t-test because we are trying to test if the cost of a car affects the purchase of a car between two different brands.
	* To run the statistical test, I would need the price of MechaCar and its competitors.
