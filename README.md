# CMSE_202_team_5_-Project

In simple terms, diabetes is a chronic health condition that affects how a person's body turns food into energy. Although a lot of enviromental factors and eating habits are associated with Diabetes, it is unclear how Diabetes actually correlates with different trends of general health. Thus, this project sought to understand how diabetes relates to factors of general health such as BMI, cholesterol, blood pressure, and other trends. Having an insight into this parameters helped us not only understand what factors seem to be highly correlating with Diabetes but also allow us to develop a model that predicts whether a person is prone to developing diabetes given to where they stand on these different trends. 



The data analysis was subdivided into three different datasets:


## Kaggle "Diabetes" Dataset

### Cleaning the data
0 values were inside the dataset for some variables that would not make sense. For example, "SkinThickness" had a 0 value for 1 patient which wouldn't be true. This piece of code weeded out the 0 values by dropping all the rows that had 0 values in them for variables like BMI, Skin Thickness, and Age. 

### Heatmap of Correlations &
### Linear Regression
This heatmap illustrates the levels of correlations among the variables in the dataset. The results were analyzed and written down below. A linear regression was also done for this dataset with the outcome variable (that being whether a patient has diabetes or not) and all other variables. This resulted in different correlation coefficients so further analysis was done to analyze the trends. 

### Curve Fitting: BMI vs the Diabetes Pedigree Function
These lines of code define a curve fit model using curve_fit from scipy. On the x-axis there is the diabetes pedigree function, which is the possibility of a person having diabetes, against BMI. Results that it tends to follow a linear trend. Limitations include the fact that most samples are clustered along low diabetes pedigree function values. 

### Ordinary Least Squared Regression
The same regression that was done with the outcome variable was done with the diabetes pedigree function. The main result to focus on here was it's correlation with BMI. 



## The Center for Disease Control and Prevention Diabetes Surveillance

### Cleaning the Dataset
Columns that didn't provide any values were found in the dataset and dropped. Variables were assigned to the different columns in order to make analysis of them later easier.

### Curve Fitting
Similar to the dataset above, a curve fitting model was used to visualize the trends found in the dataset. Specifically, this dataset was used to looked into the relationship of diabetes over the years and try to predict future trends. Results are shown below the three plots.  





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


How to run this code: This project works from the top-down, start with the imports section, and continue to run all cells as you progress, making sure to wait that the cell has loaded before moving to the next cell. "Run all" Can work but there are sometimes issues with the cells that take longer to load.


Divison of Work: 

William: Presentation Slides, Provided code for Section 2, commented code, wrote explanations in markdown cells. Sorted out and cleaned the datasets, removed erroneous values and such

Leo:

Andrew:

Ishan:















