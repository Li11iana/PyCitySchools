# PyCitySchools Analysis
## Overview
Using Python Pandas the city school district will be able to review and compare the data from different schools. Condensing the data will allow to show trends in bugdet and school performance necessary to address the educational status of the distric and make strategic desicion based on the data insights and trends.

### Purpose
The objective of this project is to analyze the data and prepare a report that informs of school distric current characteristics supporting decision-making and strategic planning for stakeholders at school and distric level.

## Analysis
For the execution of this project the technical analysis was divided into 5 stages, results will be presented in the following order:
1. Data collection into a Dataframe
2. Data cleansing
3. Summary of the data
4. Establishing subset for specific analysis
5. Comparing subsets of data

### 1. Data collection into a Dataframe
To manage the data in cvs form a dataframe was created, this 2-dimensional data structure allows us to store and work with the data in a organized way.+

![Dataframe_1](https://github.com/Li11iana/PyCitySchools/blob/main/Resources/Images/Dataframe_1.png)

### 2. Data cleansing
Original data set contained incomplete or erroneous. 
As shown in the next image, the number of elements in each column varies between 17,546 elements in the "reading_score" column to 19,514 in must of the other columns, thus indicating that certain rows have incomplete data. 
![Missing_data_1](https://github.com/Li11iana/PyCitySchools/blob/main/Resources/Images/Missing_data_1.png)

Using the methods *drop* rows with incomplete data were removed while using the method *duplicated* reveal and allows remotion of repited rows. Results can be seen in the next image where number of elements was homogenous for all columns.
![Missing_data_2](https://github.com/Li11iana/PyCitySchools/blob/main/Resources/Images/Missing_data_2.png)

Finally the data within the "Grades" column was modified from text to numerical form:

-Original data type for the "Grades" column

![Missing_data_3](https://github.com/Li11iana/PyCitySchools/blob/main/Resources/Images/Missing_data_3.png)

-Modified data type for the "Grades" column

![Missing_data_4](https://github.com/Li11iana/PyCitySchools/blob/main/Resources/Images/Missing_data_4.png)

Additionally the average for the math_score was calculated, if needed the score of any other subject could have been calculated and filter as desired. The minimum overall reading score was stored as a variable for further review.

### 3. Summary of the data
Using the method *describe* we can obtain a summary of the dataset's descriptive statistics for numeric and object series. As shown in the image below we can obtain central tendency and distribution parameters for the numerical data. 

![Summary_data](https://github.com/Li11iana/PyCitySchools/blob/main/Resources/Images/Summary_data.png)
 
### 4. Establishing subset for specific analysis
The method used in the section before (*describe*) can be used for specific subsets of the data, in order to evaluate if there are any significant differences between them. In the image below the method *describe* is used to analyze the statistical parameters only for the rows were Grade = 9.

![Summary_data_9grade](https://github.com/Li11iana/PyCitySchools/blob/main/Resources/Images/Summary_data_9grade.png)

Specific rows and cells can be display 

### 5. Comparing subsets of data

## Results

### Additional analysis


