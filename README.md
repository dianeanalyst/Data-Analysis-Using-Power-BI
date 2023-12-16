# Data-Analysis-Using-Power-BI
# Introduction
The relevance of Business Intelligence tools in data analysis cannnot be over emphasized. Its use ranges from data integration, data transformation, data modelling, creating interactive reports and data visualization, etc. This repository hosts tasks that followed my first Power BI lessons.
# Context
Understanding the basics of Power BI made the foundation of my learning journey. This included importing datasets from other sources and connecting Power BI to databases and other cloud data sources for the purpose of importing and analysing data. Proceeding from this, I got introduced to cleaning and transforming data using Power BI. As in other tools, the key steps in cleaning data in this tool is not any different. However, data transformation takes place in a Power BI feature called Power Query Editor which cleans and refine data into usable forms before loading them into their models. Other data transformation processes involves grouping, sorting, filtering and merging of data from multiple sources.
# Task 1: Data Importation, Cleaning and Transformation
As the topic of this task holds, the first step of this task involved importing three datasets into Power BI using the Text/CSV option from the 'Get Data' menu. These are the Employee dataset (100 rows), Salary dataset (199 rows) and Department dataset (199 rows).

![image](https://github.com/dianeanalyst/Data-Analysis-Using-Power-BI/assets/120665115/6636ef5c-7a0b-4b8b-b7de-7680b49b25be)
![image](https://github.com/dianeanalyst/Data-Analysis-Using-Power-BI/assets/120665115/cefe127e-060b-4707-bb2b-90c5c00bb814)
![image](https://github.com/dianeanalyst/Data-Analysis-Using-Power-BI/assets/120665115/3c0b2447-f73f-4dc0-a3e9-cb25ad212018)
These datasets were imported raw and unclean and thus required data cleaning techniques. Using the 'Transform Data' menu in this step, I started by capitalizing the column headers across the datasets and assign the appropriate data types to each columns where necessary, removed duplicates and blank cells.
#
Moving on with cleaning the datasets, the Date of Birth column in the Employee dataset was noticed to have inconsistencies in the input. This required using the 'Replace Values' menu to change the dividing symbol into one such that it is consistent across the rows. Furthermore, the column had to be formatted to Date seeing that the presence of inconsistencies caused it to be recognised as Text by Power BI. Here, I employed the 'Split Column by Delimiter' option to split the date into three columns; Day, Month and Year. Next, I selected the split columns and merged them using the 'Merge Columns' usign the custom separator (/) and then changed the datatype to Date.
![image](https://github.com/dianeanalyst/Data-Analysis-Using-Power-BI/assets/120665115/cca14a4f-e09c-421e-bf23-b7e677039c8c)
![image](https://github.com/dianeanalyst/Data-Analysis-Using-Power-BI/assets/120665115/8a6c3367-6ac0-4285-b691-a969d9ec870a)
![image](https://github.com/dianeanalyst/Data-Analysis-Using-Power-BI/assets/120665115/c18a40d6-8a76-4c98-8707-ad0fec2a6d5a)
![image](https://github.com/dianeanalyst/Data-Analysis-Using-Power-BI/assets/120665115/a545daa8-2156-4917-b535-8ef0fdabea50)
I also used the column preview option to check and ascertain the column quality and column distribution.
#
Another requirement in this task was to merge all three datasets into one dataset. Data merging and appending is also another step in data transformation process using Power Query Editor. Just like JOINS in Structured Query Language, the common columns are used when merging datasets in Power BI. Using the Employee ID columns, I merged the Employee and Salary datasets as new (naming it Employee/Salary) and went further to use the Department ID column to merge the Employee/Salary with the Department datasets as new (naming it Full Data).
![image](https://github.com/dianeanalyst/Data-Analysis-Using-Power-BI/assets/120665115/7c89535e-532e-4546-bf8c-91a4cea5d441)
![image](https://github.com/dianeanalyst/Data-Analysis-Using-Power-BI/assets/120665115/90e063b9-3603-4d97-9116-703cd2b12578)

