# Study Design: MechaCar vs Competition.

## Resources
• Data Source: MechaCar_mpg.csv and Suspension_Coil.csv

• Data Tools: tidyverse, dplyr, ggplot2 and MechaCarChallenge.RScript.

• Software: RStudio and 

## Overview of Project

A few weeks after starting his new role, Jeremy is approached by upper management about a special project. AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has called on Jeremy and the data analytics team to review the production data for insights that may help the manufacturing team.

In this challenge, you’ll help Jeremy and the data analytics team do the following:

*Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes

*Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots

*Run t-tests to determine if the manufacturing lots are statistically different from the mean population

*Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. --For each statistical analysis, you’ll write a summary interpretation of the findings.



## Results

### When doing a linear regression  summary of our data we see that the significant variable in the dataset our vehicle_length and ground_clearance. We reduce that model by removing vehicle_weight,spoiler_angle and AWD. This changes the p-vale from 5.35e-11 to  3.637e-12 making this model significant. when we break them up by groups we see that Lot 3 has the most variance and lower PSI average and Lot1 has the least varience. This could mean that Lot 3 should not be used within the MechaCar.
 ![image](https://user-images.githubusercontent.com/31675832/151857278-5096894b-9161-47c4-a306-fa6c2117da8f.png)
               
![image](https://user-images.githubusercontent.com/31675832/151856032-c3a6334f-938e-4b00-b0b7-8c764f997baa.png)

## Summary


1) What metric or metrics are you going to test?
Collecting data for comparable models across all major manufacturers for past 3 years for the following metrics:

  • Safety Feature Rating: Independent Variable

  • Current Price (Selling): Dependent Variable

  • Drive Package : Independent Variable
  
  • Engine (Electric, Hybrid, Gasoline / Conventional): Independent Variable

  • Resale Value: Independent Variable

  • Average Annual Cost of ownership (Maintenance): Independent Variable

  • MPG (Gasoline Efficiency): Independent Variable

2) What is the null hypothesis or alternative hypothesis?

After determining which factors are key for the MechaCar's genre:

   • Null Hypothesis (Ho): MechaCar is priced correctly based on its performance of key factors for its genre.

   • Alternative Hypothesis (Ha): MechaCar is NOT priced correctly based on performance of key factors for its genre.

3) What statistical test would you use to test the hypothesis? And why?
A multiple linear regression would be used to determine the factors that have the highest correlation/predictability with the list selling price (dependent variable); which combination has the greatest impact on price.

4) What data is needed to run the statistical test?
-MechaCar_mpg.csv
-Suspension_Coil.csv
