# Pewlett_Hackard_Analysis

## Overview
My analysis will help Pewlett Hackard store information in databases to get specific information on employees and their company.  I have stored this information in their own tables on the database and exported the information to csv files.  I created 4 new tables and csv files with the below analyses:
1. A table with all the employees eligible for retirement, with their title
2. A unique table with the eligible employees with their most recent title, if they have switched roles in the job
3. The count of eligible per each title
4. A unique table of employees eligible for the mentorship program and their most recent title 

## Results
The results of my analysis show the follow:
1. The retirement title table shows the employee number, first name, and last name from the employee table and the title, from date and to date from the titles table.  We joined the employees and titles table from the employee number key. I filtered the birth date column from employees to get all the entries with employees eligible for retirement.
2. the Unique titles table takes the informatiomn from my retirement titles table and removes any duplicate entries if an employee switched jobs and had different titles at some point in the company. By sorting in descending order by to date, we will get their most recent title.
3. The retiring titles tables takes the info from the unique titles table and counts each entry to group by title.  This shows how many unique employees of each title are eligible for retirement.
4. The mentorship eligibilty table takes the emp_no, first_name, last_name, and birth_date from the employees table, the rom_date and to_date from the employee department table, and the title from the titles table.  We join the 3 tables based om the emp_no key. We apply the conditional of current employees and a specific date range to get the employees eligible for the mentorship program. 

## Summary
The 4 tables I created give quick insight and easy storage of employee eligibilty for retirement or mentorship.  The helps the company have accessibility into database information and can easily grab useful information needed for company organization.  Another helpful table that can be created is joining the employee, salary, and title tables to get the avergae salary by each title.  This can show how the pay per titles compare to market pay to stay competitive in the industry.   A second table we could create is by using the department info to the take the count of current employees by each deptartment.  This could be helpful for hiring and recruitment information if a department is in need of employees. 