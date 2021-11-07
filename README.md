# Pewlett-Hackard-Analysis

## Overview of the Analysis

In this project we are helping Bobby, an HR analyst at company - Pewlett Hackard peform a research on employees that are going to retire in the near future. Using SQL we we will create a database of all the employees and then write queries to perform the required analysis.

### Purpose
The purpose of this analysis is to determine the number of retiring employees per title and identify the employees that are eligible to participate in the mentorship program.

## Results

- **Employees retiring by title** -
First, we will find out all the employees who were born between 1952 and 1955 and get their titles from the titles table by using Inner Join on the primary key(emp_no). These are the employees who will be retiring soon.

![Employees retiring by title](https://github.com/vedikanigam/Pewlett-Hackard-Analysis/blob/main/Resources/Employees_retiring_by_title.png)


- **Duplicate Entries** -
Some of the employees have had more than one title. So, we will keep only the most recent title by using Distinct On statement.

![Duplicate Entries](https://github.com/vedikanigam/Pewlett-Hackard-Analysis/blob/main/Resources/Removing_duplicate_entries.png)

- **Count of retiring employees by title** -
A count of the employees by title is done by using Group By statement and Count Statement on the title column.

![Count of retiring employees by title](https://github.com/vedikanigam/Pewlett-Hackard-Analysis/blob/main/Resources/Count_of_retiring_employees_by_title.png)


- **Employees eligible for mentorship program** -

Finally, employees who are born in 1965 will have an opportunity to participate in a mentorship program for new employees. Using the distinct on statement we will find their most recent title.

![Employees eligible for mentorship program](https://github.com/vedikanigam/Pewlett-Hackard-Analysis/blob/main/Resources/Employees_eligible_for_mentorship_program.png)


## Summary 
Some 90,398 employees are going to retire in the near future. Around 33% are senior engineers, 16% are engineers and 5% are assistant Engineers. Around 31% are senior staff and 14% are staff. 
A quick count of the titles in the mentorship eligibility table reveals that there are only around 700 engineers (senior engineer, engineer, and assistant engineer) who will be eligible to participate in the mentorship program which is clearly much lower than the numbers retiring. Similary the numbers in the staff category (around 700) are also much lower than the numbers that are retiring.

### Additional tables-
A count of titles in the mentorship eligibility tables will be useful to find out how many employees in what roles are available for mentorship.

A count of mentees in the employees table would be useful to find out how many employees need mentorship and how many new employees should be hired.

