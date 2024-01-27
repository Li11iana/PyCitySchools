# PyCitySchools Analysis
## Overview
Using Python Pandas the city school district will be able to review and compare the data from different schools. Condensing the data will allow us to show trends in budget and school performance necessary to address the educational status of the district and make strategic decisions based on the data insights and trends.

### Purpose
The primary purpose of this report is to provide stakeholders with a detailed overview of each school's performance and to identify areas for improvement. The insights derived from this analysis are intended to drive data-driven decisions that will contribute to ongoing efforts to enhance overall school performance.


## Analysis
For the execution of this project the technical analysis was divided into 5 stages, results will be presented in the following order:
1. Data collection into a Dataframe
2. Data cleansing
3. Summary of the data
4. Establishing subset for specific analysis
5. Comparing subsets of data

### 1. Data collection into a Dataframe
To manage the data in cvs form a dataframe was created, this 2-dimensional data structure allows us to store and work with the data in an organized way.

![Dataframe_1](https://github.com/Li11iana/PyCitySchools/blob/main/Resources/Images/Dataframe_1.png)

### 2. Data cleansing
The original data set contained incomplete or erroneous information. 
As shown in the next image, the number of elements in each column varies between 17,546 elements in the **reading_score** column to 19,514 in the other columns, thus indicating that certain rows have incomplete data. 
![Missing_data_1](https://github.com/Li11iana/PyCitySchools/blob/main/Resources/Images/Missing_data_1.png)

Using the methods *drop* rows with incomplete data were removed while using the method *duplicated* reveal and allow remotion of repeated rows. Results can be seen in the next image where the number of elements was homogenous for all columns.

![Missing_data_2](https://github.com/Li11iana/PyCitySchools/blob/main/Resources/Images/Missing_data_2.png)

Finally, the data within the "Grades" column was modified from text to numerical form:

- Original data type for the "Grades" column.

![Missing_data_3](https://github.com/Li11iana/PyCitySchools/blob/main/Resources/Images/Missing_data_3.png)

- Modified data type for the "Grades" column.

![Missing_data_4](https://github.com/Li11iana/PyCitySchools/blob/main/Resources/Images/Missing_data_4.png)

Additionally the average for the **math_score** was calculated, if needed the score of any other subject could have been calculated and filtered as desired. The minimum overall reading score was stored as a variable for further review.

### 3. Summary of the data
Using the method *describe* we can obtain a summary of the dataset's descriptive statistics for numeric and object series. As shown in the image below we can obtain central tendency and distribution parameters for the numerical data. 

![Summary_data](https://github.com/Li11iana/PyCitySchools/blob/main/Resources/Images/Summary_data.png)
 
### 4. Establishing subset for specific analysis
The method used in the section before (*describe*) can be used for specific subsets of the data, to evaluate if there are significant differences. In the image below the method *describe* is used to analyze the statistical parameters only for the rows where Grade = 9. Specific rows and columns can be displayed, and statistical parameters can be applied to these subsets.

![Summary_data_9grade](https://github.com/Li11iana/PyCitySchools/blob/main/Resources/Images/Summary_data_9grade.png)



### 5. Comparing subsets of data
Using filters and subgroups comparison between different factors is facilitated. For this project it was shown that public schools have a higher average budget than charter schools, with $872625.65 as the charter school average budget and $ 911195.56 for public schools.
Another subset revealed that public schools' average mathematics score is lower than that of charter schools.
- Average budget per school type

![Budget_vs_schooltype](https://github.com/Li11iana/PyCitySchools/blob/main/Resources/Images/Budget_vs_schooltype.png)

- Average math score per school type

![Schooltype_vs_mathscore](https://github.com/Li11iana/PyCitySchools/blob/main/Resources/Images/Schooltype_vs_mathscore.png)

## Findings

- Data cleaning:

This exercise showed the importance of reviewing the data set for missing and duplicate values before further assessment. It is very convenient that Pandas has specific methods for that, which makes it much more intuitive than cleaning data through repetitive actions in Excel, for example. 

- Data description:

Being able to preview the dataset provides actionable information, for example the "Grades" subset reveals that there are more students in 9th and 10th grade than 11th and 12th grade, this could potentially mean that an important number of students could be dropping out of school, depending on the school administration the reason behind that could be reviewed. Using. describe we can see that the average score on mathematics is 64.675733 while for reading the average score is 72.357865, both parameters should be improved, however you could argue the more resources to make mathematics more appealing to the students.

- Dataset and subset comparison:

Pandas provides great tools to filter, summarize and compare subsets of the data frame allowing you to review from a macro school district view or turn to a specific school and adapt to their precise needs and development opportunities. An additional analysis that could be of importance would be the quantity of students and budget assigned to the school and compare that with the average budget for each school-type table since the last one revealed that public school have on average a higher budget than charter schools however this higher budget could be diluted in a bigger student population.


