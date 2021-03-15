# MechaCar_Statistical_Analysis

## Lineal Regression to Predict MPG
Vehicle length, ground clearance and the intercept provivded a non-random amount of variance to the mpg values in the dataset. The slope of the linear model is not considered to be zero becuase the p-value is 5.35e-11, significantly less than the p-value needed to reject the null hypohtesis that the slope is zero.  The linear model can effectively predict 72% of the mpg of the MechaCar prototypes as indicated by the r-sqauared value (0.7149).

![LineRegression](/console_log/deliverable1_lm_mpg.png)


## Summary Statistics on Suspension Coils

The variance of the total data set meets the design specification of PSI less than 100.  The variance for lot 3 does not meet the specification (170.29 PSI).  

![SummaryStats](/console_log/deliverable2_total_summary.png)

![LotsSummary](/console_log/deliverable2_lot_summary.png)

## T-Tests on Suspension Coils

T-tests of both the full dataset and subsets grouped by lot show the mean of all groups except Lot 3 are not statisically different than the population mean of 1500PSI.  The P-value of the t-test for Lot 3 was 0.04168 which is lower than the p-value needed to reject the null hyphothesis that the mean of this subset is statistically different than 1500PSI.  

![T-Tests](/console_log/deliverable3_t_test_lots.png)

## Study Design: MechaCar vs Competition

To test the MechaCar's performance against competetors, fuel efficeiency (city and highway) for cars of similar size and ground clearance should be compared.  The null hypothesis would be that threre is no statsically significant difference in mpg between the MechaCar ans similar competetors.  The alernative hypothesis is that there is a statiscally signifcant difference between the mpg of the MechaCar and its competition.  T-test comparing the MPG of the MechaCar against both its competitors in aggregate and separately would be used to test the hypothesis.  It would be necessary to test both aggregately and individually to see if there were other underlying factors worth further investigating.  Thos study would require the make, model, vehicle size, city and highway mpg, and ground clearance for the competators.  Horse-power and number of cylinders would also be insightful but not necessary.  
