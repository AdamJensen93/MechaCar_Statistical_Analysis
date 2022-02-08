# MechaCar Statistical Analysis
## Linear Regression to Predict MPG
As seen in linear_regression_model.png, we can observe the outcome of creating a linear regression model to predict MPG. When observing the p-value of "vehicle_length" and "ground_clearance" we see they are 2.60e-12 and 5.212-08 respectively. The hypothesis that vehicle length and ground clearance did not contribute to to MPG would be viewed as unlikey. It seems that there may be some statistical relationship between the two factors in question and MPG.

We can also observe the p-value of our linear regression is 5.35e-11. The caluculated p-value is below the .05 threshold, concluding we can reject our null hypothesis. Based on these observations we can determine that the MechaCar prototypes are dependent on Vehicle Length and Ground Clearance for MPG. We can also infer that the other three factors do not have an impact on MPG in regards to the MechaCar.
## Summary STatistics on Suspension Coils
We calculated the total summary statistics that can be seen in totaly_summary.png. We generated the mean, median, variance, and standard deviation of the suspension coil's pounds per square inche (PSI). We also looked at the summary statistics for each individual lot, shown in lot_summary.png. The specifications show that the variance of the suspension coils must not exceed 100 PSI. Wen looking at the total summary table, we see the varicance in PSI PSI for all vehicles is 62.29. This shows the current data meets the design specifications. However, when observing each lot indivually we see Lot 1 has a variance of 0.98, Lot 2 has a variance of 7.47, and Lot 3 has a variance of 170.29. Lots 1 & 2 are within the normal range of variance but Lot 3 is well above the threshold.
## T-Test on Suspension Coils
To further analyze the lots, we performed a T-Test (first_t_test.png) to determine the PSI across each manufacturing lot, looking for statisical differences from the population mean of 1,500 PSI. Assuming our level of significance is .05, with a p value of 0.06, we can not declare there is a statictical difference between the data sets. However, it is not enough to reject our null hypothesis. We then completed three additional T-Tests on each individual Lot (t_test_lot1.png, t_test_lot2.png, t_test_lot3.png) to look deeper at the data. The p-value of lot 1 is 1.0 exactly, meaning it is statistically similar and we cannot reject the null hypothesis. The p-value of lot 2 is .61, which fails to reject the null hypothesis. The p-value of lot 3 is 0.04 which shows a statistical difference and rejects the null hypothesis.
## Design a Study Comparing the MechaCar to the Competition
When shopping for a car, there are multiple variables that people consider. Living in the Pacific Northwest, there's a strong focus on outdoor recreation. Individuals spend time in their cars going to the beach or on top of mountains. Vehicles in this region aren't simply for commuting, but they need to be able to perform on pavement, sand, rain, snow, and mud. It seems like AWD could be an attractive option for the adventurers of the Pacific Northwest, so the question to ask: Do vehicles with AWD sell at a significantly different rate in this region?
### Metrics to Test:
-Sales of vehicles with AWD compared to all vehicle sales Nationwide
-Sales of vehicles with AWD compared to all vehicles in Oregon/Washington
### Null and Alternative Hypothesis:
-Null: There is no impact on sales of a vehicle in Oregon/Washington.
-Alternative: People in Orgon/Washington purchase AWD vehicles at a much greater rate than the rest of the nation.
### Statisical Test:
-A linear regression model would determine is there was a difference between AWD vechicles and non-AWD vehicles sales. A T-Test would be needed to determine if state specific sales data would be dependent on AWD vehicles or not.
### Data Needed:
-Sales Data for automobiles nationwide for the past 3 years specifying whether or not the vehicle was AWD or not. Sales data for Oregon and Washington specifically with the same parameters.
