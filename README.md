Employee Database Analysis

Overview
The purpose of this analysis is to determine the number of retiring employees per titles as there are many current employees about to reach retirement age. In this analysis, we also identified the employees that are eligible to participate in the mentorship program. We utilized pgAdmin software to create these tables and analyze the data. 
In this analysis, we discovered that some employees have multiple titles in the system, most likely due to promotions, therefore, we use the DISTINCT ON statement to create a table that contains only the most recent title for each employee. We used the COUNT() function to create a final table that has the number of employees about to reach retirement age by their most recent job title.

RESULTS
In the table below, we created a retirement titles table that includes the employee number, first and last name, title of the employee and we filtered the data by their birth date. In the table below, we can see that an employee (Sumant Peac) name appeared three times with different titles. As we continue with our analysis, we will filter the results to show only the most recent title for employees that were promoted, and therefore have multiple titles in the system. 

 

In the table below, we created a Unique Titles table where we removed the duplicate titles and keep only the most recent title for each employee. We used the DISTINCT ON statement to retrieve the first occurrence of the employee number for each set of rows. We used the INTO clause to create the Unique Titles table and sorted the table in ascending order by the employee number and descending order by the last date of the most recent title. 
 


In the Retiring Titles table pictured below, we created a table to hold the number of titles filled by employees who are retiring. 
 

In the final table for this analysis, we created a Mentorship Eligibility table for current employees that were born between January 1, 1965 and December 31, 1965, as pictured below.

 


Summary 

Using the SELECT COUNT(*)FROM unique_titles statement, we discovered that 90,398 roles will need to be filled as the “silver tsunami” begins to make an impact. More than 60% of the current number of employees will be retiring.  
 


Using the SELECT COUNT (*) FROM mentorship_eligibility statement, we discovered there are 1,549 retirement-ready employees in the departments to mentor the next generation. With these figures, I believe the company should be able to refill the positions of the employees that are retiring. 



![image](https://user-images.githubusercontent.com/85265504/128623414-01de83bd-12ac-470a-9ec3-b238ec258675.png)
