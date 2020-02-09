# youth-obesity-risk-factors
Obesity is a condition defined by the [World Health Organization](https://www.who.int/topics/obesity/en/) as a "major risk factor for a number of chronic diseases, including diabetes, cardiovascular diseases and cancer" and a leading preventable cause of death in the United States and worldwide.
It is also a condition that is seen increasingly in children.
The [Youth Risk Behavior Surveillance System (YRBSS)](https://www.cdc.gov/healthyyouth/data/yrbs/overview.htm) was developed in 1990 by the Centers for Disease Control and Prevention (CDC) to study obesity and other health outcomes and associated risk factors among youth in the United States.
The motivation for this project is to understand the rates of youth obesity over time and across locations and populations within the United States, and how they are correlated with certain nutritional, behavioral, institutional, and environmental risk factors.
Two datasets from the CDC are considered: [Youth Risk Behavior Surveillance System](https://chronicdata.cdc.gov/Nutrition-Physical-Activity-and-Obesity/Nutrition-Physical-Activity-and-Obesity-Youth-Risk/vba9-s8jp) contains information on the prevalence of youth obesity and associated risk factors gathered from the YRBSS, and [Policy and Environmental Data](https://data.cdc.gov/Nutrition-Physical-Activity-and-Obesity/Nutrition-Physical-Activity-and-Obesity-Policy-and/k8w5-7ju6) focuses on state policy and environmental factors.

The findings of the analysis are that the percents of high-school students in the United States that are obese and those that are overweight or obese have increased from 2001 to 2017, are higher in certain racial/ethnic groups, and are higher in males than females, although females are catching up.
Also, the five locations with the lowest rates of these high-BMI designations are all in the Rocky Mountains, and in those states students tend to watch less TV, eat more vegetables, and drink less soda than the national average.
Those states also have more farmers markets per capita and more people living within half a mile of a park than the national average.
The six locations with the highest rates of these high-BMI designations are Guam and five states along the Mississippi River, and students in those locations tend to watch more TV, eat fewer fruits and vegetables, and drink more soda than the national average.
Those locations also have fewer farmers markets per capita and fewer people living within half a mile of a park than the national average.
After training on 30% of the location-wide data samples (not those samples corresponding to a subset of the population such as a gender or race/ethnicity), a linear regression model was able to predict the rates of being obese and of being overweight or obese in the remaining 70% of samples with 48% and 50% accuracy, respectively, by considering only the associated risk factors.
By adding the geographic region in which the location lies as defined by the [U.S. Census Bureau](https://www2.census.gov/geo/pdfs/maps-data/maps/reference/us_regdiv.pdf), model accuracy increases to 53% and 57%, respectively; by adding the geographic division, accuracy increases to 61% and 61%, respectively.

This project uses the [math](https://docs.python.org/3/library/math.html) library for basic mathematical functions, [NumPy](https://numpy.org/) and [Pandas](https://pandas.pydata.org/) for data organization and management, [matplotlib](https://matplotlib.org/) and [seaborn](https://seaborn.pydata.org/) for visualization, and [scikit-learn](https://scikit-learn.org/stable/) for processing data and building, training, and evaluating machine learning models.

[Youth_Risk_Behavior_Surveillance_System.csv](https://github.com/Nick-G-Horvath/youth-obesity-risk-factors/blob/master/Youth_Risk_Behavior_Surveillance_System.csv) contains information on the prevalence of youth obesity and associated risk factors gathered from the YRBSS.

[Policy_and_Environmental_Data.csv](https://github.com/Nick-G-Horvath/youth-obesity-risk-factors/blob/master/Policy_and_Environmental_Data.csv) contains information on state policy and environmental factors.

[youth-obesity-risk-factors.ipynb](https://github.com/Nick-G-Horvath/youth-obesity-risk-factors/blob/master/youth-obesity-risk-factors.ipynb) contains all data analysis, visualization, and discussion.
