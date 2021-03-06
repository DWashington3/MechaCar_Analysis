# MechaCar Statistical Analysis using RStudio
## Overview
To assist with a MechaCar's production bottleneck, I've been tasked with performing multiple linear regression analysis to identify which variables in the data set predict the MPG. This was completed in RStudio. In addition, I completed summary statistics on the pounds per square inch (PSI) of the suspension coils, t-tests to determine if the manufacturing lots are statistically different and designing a study to compare the competition's production.

## Results
### Linear Regression to Predict MPG
<img width="573" alt="MPR_regression" src="https://user-images.githubusercontent.com/87162266/151458789-e415f6d0-2891-4140-a05a-20230d0d3fb5.PNG">

### Summary
In this Multi-Linear Regression vehicle length and ground clearance don't provide a random amount of variance to the MPG values. The slop wouldn't be considered Zero simply because the P-value of 5.85 x10^-11 is a very small number. Such a small P-value doesn't correlate the X and Y since it is below the significance level. Since the Multiple R-Squared value is 0.7149, this model does predict the MPG of the prototypes effectively.

## Summary Statistics on Suspension Coils
### Total Summary: Mean, Median,Variance,Standard Deviation
<img width="323" alt="total_summary" src="https://user-images.githubusercontent.com/87162266/151490386-e5a9129d-33f3-4c67-b6b9-3a30338cdc00.PNG">
### Lot Summary: Mean, Median,Variance,Standard Deviation By Lot
<img width="460" alt="lot_summary" src="https://user-images.githubusercontent.com/87162266/151490559-c241663b-8a14-4dc0-ae2d-96e98c320803.PNG">

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch.  On average the three lots suspension coils meet the design specification. However, after dividing it by lot, lot 3 does not meet the design specifications. Lot 1 and lot 2 have a variance of 0.98 and 7.47 respectively, while lot 3 has 170.87.

## T-Tests on Suspension Coils

### Total lots
- T-Test- This t-test compares the PSI for all three lots is statistically different from the population mean of 1,500 PSI. The successive t-tests are per lot. 
<img width="481" alt="ons_samplet" src="https://user-images.githubusercontent.com/87162266/151491850-a8ca7fa7-6247-486c-86a5-bf4f8f617159.PNG">

### Lot One
<img width="525" alt="Lot 1" src="https://user-images.githubusercontent.com/87162266/151491871-c35e78dd-ac20-41bf-8e4e-140252e3258e.PNG">

### Lot Two
<img width="539" alt="lot 2" src="https://user-images.githubusercontent.com/87162266/151491926-4179c1b4-6698-4c62-b5ac-6b6bf59881ae.PNG">

### Lot Three
<img width="527" alt="lot 3" src="https://user-images.githubusercontent.com/87162266/151491943-8652c783-4b47-47d8-8aac-07be13294ed3.PNG">

## Study Design: MechaCar vs Competition
There are several variables affect's decision to buy a car.  For  new or used cars things like miles driven, cost mileage efficiency, maintenance cost, performance and safety ratings matter. More buyers drive automatic transmission than manual, and that may be a deal breaker for some buyers. I am going to test MachaCar's price of used car population's automatic and manual transmissions against the population total. The hypothesis would go as follows:

H???= There is no statistical difference between MechaCar's price and their competitors' price when measuring like transmissions.

Ha=There is ??? statistical difference between MechaCar's price and their competitors' price when measuring like transmissions.

A two-sample t-test would be used to compare both the competitors population  and MechaCar's population for a statistical difference in price.
The information required to complete this task is MechaCar's price and transmission vehicle data and the competitors' respective vehicle data.
