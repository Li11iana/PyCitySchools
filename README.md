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

## Results
### 1. Data collection into a Dataframe
To manage the data in cvs form a dataframe was created, this 2-dimensional data structure allows us to store and work with the data in a organized way.+

![Dataframe_1](https://github.com/Li11iana/PyCitySchools/blob/main/Resources/Images/Dataframe_1.png)
### 2. Data cleansing
Original data set contained incomplete or erroneous. 
As shown in the next image, the number of elements in each column varies between 17,546 elements in the "reading_score" column to 19,514 in must of the other columns, thus indicating that certain rows have incomplete data. 
![Missing_data_1](https://github.com/Li11iana/PyCitySchools/blob/main/Resources/Images/Missing_data_1.png)

Using the methods *drop* rows with incomplete data were removed while using the method *duplicated* reveal and allows remotion of repited rows. Results can be seen in the next image where number of elements was homogenous for all columns.
![Missing_data_2](https://github.com/Li11iana/PyCitySchools/blob/main/Resources/Images/Missing_data_2.png)

Finally the data within the "Grades" column was modified from text to numerical form
![Missing_data_3](https://github.com/Li11iana/PyCitySchools/blob/main/Resources/Images/Missing_data_3.png)
![Missing_data_4](https://github.com/Li11iana/PyCitySchools/blob/main/Resources/Images/Missing_data_4.png)


### 3. Summary of the data
### 4. Establishing subset for specific analysis
### 5. Comparing subsets of data

### Additional analysis


