# Project On Fitbit-Analysis
Here I consider a Fitbit data that measures daily vitals in human. I perform data analysis and build Statistical Model from this data. For these purposes, I used both Python and R programming language.

## About the Data set:
The data set named **'FitBit Data'** is in csv format. It has 50 rows/observations and 10 columns/values. These column are also called attributes. The data set .csv file is also attached in the files section of this project. The different attributes that are used in this data are - 
* Sleeping -  A continuous variable. Indicates number of hours slept everyday.
* HeartRate - A continuous variable. Indicates heart rate that is measured everyday.
* Glucose - A continuous variable. Indicates blood sugar level.
* Cholesterol - A continuous variable. Indicates amout of body fat.
* Run - A continuous variable. Indiacte distnace covered evertday in meter unit.
* BMI - A continuous varibale. Indicates Body Mass Index of human being in kg/m^2 unit
* Weight - A continuous variable. Indicates the weight of the person in kilogram unit.
* Height - A continuous variable. Indicates the height of the person in meter unit.
* HealthIndex - A continuous variable. Indicates the health score out of 10. A score of 10 means perfect BMI.
* Condition - A categorical variable, indicates health condition. It has two levels - Good and Bad

## Used Packages/libraries in this project: 
Here both R programming and Python programming language are used. So, as a result some packages of the both languages are used in this project work.

* **Python Packages:** The python packages that are used in this project are -
  - Matplotlib.pyplot and style module from Matplotlib
  - Pandas
  - Numpy
  - Seaborn

* **R Packages:** The R packages used in this project work are - **Tidyverse and dplyr library from tidyverse package**

## Data Analysis Using Python
The first step of any project is data analysis. It also has some sub stages. They are - EDA (Explanatory Data Analysis), Data Manipulation and Data Visualization. Here we will discuss these three steps shortly.

* **EDA (Explanatory Data Analysis):**
This step in the first basic step of any data analysis project. The things that comes under this step are -
  - Reading the data in a variable called 'data' using pandas library
  - Checking the data types of the data frame's columns.
  - Obserrving the Column names.
  - Determining the shape of the data frame.
  - Getting the first 5 rows of the data frame.

* **Data Manupulation:**
In Python the library that is mostly used for data manipulation is pandas. In this project I as a data analyst manipulates the data by performing the following operation -
  - Create a column called 'Day' in the data frame.
  - Check if there are any missing values after creating one additional column.
  - Rename the Column 'Day' to 'Person'.

* **Data Visulaization:**
This is the most important part of any data analysis project. In this step we make use of matplotlib.pyplot package , seaborn package to plot different amazing graphs, that will help us to better understand the project and inter-relations between the variables that are used in the dataset. Here, I create the following plots - 
  - Distribution of sleeping hours.
  - Distribution of heart rate hours.
  - Distribution of blood sugar.
  - Distribution of body fat (Cholesterol).
  - Distribution of weight.
  - Distribution of height.
  - Relationship between heart rate and sleeping hour.
  - Relationship bettwen sleeping hour , glucose and fat.
  - Relationship between distance run and weight.
  - Trend of BMI change over number of persons.
  - Trend of weight change over number of persons.
  - Trend of height change over number of persons.
  - Relationship of distnace run with number of persons (first 10).
  - Histogram of sleeping to understand its distribution.

## Statistical Model Building using R: 
Here I read the data set in R and by using dplyr library first, I remove the Condition column and stote in in a variable called data2. My purpose is to build a Multiple Linear Regression Model using only the continous predictors. Here I used the column 'HealthIndex' as response variable and the other variables as predictor variables (except Condition). The result we get is BMI is the only predictor that has a strong linear relationship with the 'HealthIndex' variable.

* **Backward Selection Uisng AIC and BIC:** To confirm my result, I peform Backward Selection method using both AIC and BIC. The result I got is the same as the previous result. 








