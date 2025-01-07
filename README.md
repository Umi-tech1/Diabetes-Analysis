# Diabetes-Analysis

## Objective
The primary goal of this analysis is to identify key factors contributing to diabetes (Outcome) using univariate and multivariate analysis. 
The dataset comprises several features, including Pregnancies, Glucose, BloodPressure, SkinThickness, Insulin, BMI, DiabetesPedigreeFunction, Age, and Outcome. 
By understanding the relationships between these features and diabetes, we aim to provide actionable insights for better diagnosis, prevention, and management.

## Overview of the Dataset
Data Source: https://www.kaggle.com/datasets/mathchi/diabetes-data-set

## Data Description
The dataset contains the following features:
Pregnancies, Glucose, BloodPressure, SkinThickness, Insulin, BMI, DiabetesPedigreeFunction, Age, and Outcome.

- Pregnancies: Number of pregnancy
- Glucose: Plasma glucose concentration
- Bloodprssure: Diastolic bloodpressure
- SkinThickness: Triceps skin fold thickness
- Insulin: 2-Hour serum insulin
-  BMI: Body Mass Index (weight in kg/ height in meter square)
-  DiabetesPedigreeFunction: This indicates the likelihood of diabetes based on family history
-  age:age(in years)
- Outcome: The target variable, whether a patient is diagnose with diabetes or not(0 for No, 1 for yes)

# Tool: Python

# Steps: The follwing steps was used in performing the analysis

- I start by importing the necessary libraries (pandas, numpy, matplotlib and seaborn)
- Loaded the dataset into dataframe
- I explore the dataset to gain detail understanding of the dataset.
- All the missing values in the columns were replaced with the median.

# Visualization
In the visualization, I used countplot, histplot, pie chart, boxplot, violinplot

# Result
Here is the result
## Univeriate Analysis

### Analysis of Glucose
Median(117.0) and mean(121.6) of Glucose lie very close to each other i.e the distribution is more or less symmtric and uniform
- There are no rows with Glucose value as 0

### Analysis of BloodPressure
Median of BloodPressure: 72.0
Maximum of BloodPressure: 122
Mean of BloodPressure: 72.38671875

- Median(72.0) and mean(69.1) of BloodPressure lie very close to each other i.e the distribution is more or less symmtric and uniform . 

### Analysis of the Insulin
Median of Insulin: 31.25
Maximum of Insulin: 846.0
Mean of Insulin: 94.65234375

### Analysis of BloodPressure
Median of BMI: 32.0
Maximum of BMI: 67.1
Mean of BMI: 32.45091145833333

### Analysis of DiabetesPedigreeFunction
Median of DiabetesPedigreeFunction: 0.3725
Maximum of DiabetesPedigreeFunction: 2.42
Mean of DiabetesPedigreeFunction: 0.47187630208333325

### Analysis of Age
Median of Age: 29.0
Maximum of Age: 81
Mean of Age: 33.240885416666664

## Multivariate Analysis
### Analysis of Glucose and outcome
From the analysis, we observe a positive linear correlation
As the value of Glucose increases, the count of patients having diabetes increases i.e. value of Outcome as 1, increases
Also, after ther Glucose value of 125, there is a steady increase in the number of patients having Outcome of 1
so, there is a significant amount of positive linear correlation

### Analysis of BloodPressure and Outcome
We observe that,Outcome and BloodPressure do not have positive or negative linear correlation. THe value of Outciome do not increases linearly as value of BloodPressure increases
However, for BlioodPressure values greate than 85, count of patients with outcome as 1 is ,more

### Analysis of BMI and Outcome
a positive linear correlation is observe in BMI

### Analysis of Age and Outcome
For age greater than 35 years , the chances of patients having diabetes increases as seen in the plot ie. the number of patients having diabetes is more than the number of poeple not having diabetees. 
But this does not hold true for age like 60+.
There is a positive correlation between pregnancies and Outcome

### Analyzing correlations
Outcome                     1.000000
Glucose                     0.492782
BMI                         0.312249
Age                         0.238356
Pregnancies                 0.221898
SkinThickness               0.189065
DiabetesPedigreeFunction    0.173844
BloodPressure               0.165723
Insulin                     0.148457

# Insights
## Top Predictors:
Glucose, BMI, and Age emerge as the strongest predictors of diabetes.
Blood Pressure and Insulin show limited predictive power and may contribute as secondary features.
## Age-Specific Risks:
Middle-aged adults (35–60) are at higher risk for diabetes, highlighting the need for targeted interventions for this group.
## Glucose as a Key Factor:
Elevated Glucose levels strongly correlate with diabetes risk, emphasizing its importance in early detection and diagnosis.

# Recommendations
- Screening and Diagnosis:
Focus on Glucose and BMI as primary metrics for diabetes risk assessment.
Target middle-aged adults (35–60) for early screening and intervention.

- Health Interventions:
Implement community programs to reduce obesity (high BMI) through diet and exercise.
Raise awareness about managing Glucose levels to prevent diabetes onset.


