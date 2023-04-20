# CMSE_202_team_5_-Project

In simple terms, diabetes is a chronic health condition that affects how a person's body turns food into energy. Although a lot of enviromental factors and eating habits are associated with Diabetes, it is unclear how Diabetes actually correlates with different trends of general health. Thus, this project sought to understand how diabetes relates to factors of general health such as BMI, cholesterol, blood pressure, and other trends. Having an insight into this parameters helped us not only understand what factors seem to be highly correlating with Diabetes but also allow us to develop a model that predicts whether a person is prone to developing diabetes given to where they stand on these different trends. 



The data analysis was subdivided into three different datasets:


## Kaggle "Diabetes" Dataset




## The Center for Disease Control and Prevention Diabetes Surveillance



## Kaggle "Heart Disease Indicator" Dataset

### Correlation Plot of Variables in the Dataset against Diabetes
The following analysis showed that the health variables that have higher correlations with diabetes are. Running this code will result in the following significant correlations:

- High Blood Pressure
- BMI
- Body Mass Index (BMI)
- Heart Disease or Attack

### Cleaning the Data
To be able to better visualize the data the daat was cleaned up to get better results. A critical issue to note is that there were too many cases of non-diabetic patients—which were skewing the results. 

In order to change the split between diabetic and non-diabetic change the value "150000" to a bigger or smaller number.

### Running a Logistic Regression with the Variables of Interest
This logistic regression gives a better representation of what variabels are actually correlated with diabetes. Similar to the correlation plot, running the following piece of code resulted in the significant correlations:

- High Blood Pressure
- Heavy Alcohol Consumption
- High Cholesterol
- Body Mass Index (BMI)
- Heart Disease or Attack

### Correlation Matrices
Because of some disagreements between the previous correlations (specifically about the influence of Heavy Alcohol Consumption), different correlation matrices were used given variables of interest from both the bar plot and Logistic Regression. 


### Prediction Model
The following piece of code uses a prediction model given a logistic regression which is able to classify individuals as diabetic or not according to the following variables:

- High Blood Pressure (0 for no; 1 for yes)
- High Cholesterol (0 for no; 1 for yes)
- Body Mass Index (as a continuous variable)
- Heart Disease or Attack (0 for no; 1 for yes)


The model resulted in a prediction accuracy of 0.66, making it somewhat useful to classify patients as diabetic or not according to their different health factors.




















