![image](https://user-images.githubusercontent.com/112978144/227748363-7344b0b6-ee9f-43ba-98a8-35a23c6aeed5.png)


# Pewlett-Hackard-Analysis

In this challenge we were assign to  determine the number of retiring employees per title, and identify employees who are eligible to participate in a mentorship program. Then, we need to write a report that summarizes our analysis and helps prepare the manager for the “silver tsunami” as many current employees reach retirement age.
# Sections 

This challenge is consists of two technical analysis deliverables and a written report. we need to submit the following:

Deliverable 1: The Number of Retiring Employees by Title.
Deliverable 2: The Employees Eligible for the Mentorship Program.
Deliverable 3: A written report on the employee database analysis (README.md).

# Deliverable 1

For deliverable one we need to complete following steps

* Retrieve the emp_no, first_name, and last_name columns from the Employees table.

* Retrieve the title, from_date, and to_date columns from the Titles table.

* Create a new table using the INTO clause.

* Join both tables on the primary key.

* Filter the data on the birth_date column to retrieve the employees who were born between 1952 and 1955. Then, order by the employee number.

* Export the Retirement Titles table from the previous step as retirement_titles.csv 

after completing all these steps we got the following table

![image](https://user-images.githubusercontent.com/112978144/227747804-2d9c67bf-4e6c-42a2-901e-b3e47bf8607e.png)

# In the next step we follow these steps and got our required table.

* Copy the query from the Employee_Challenge_starter_code.sql and add it to our Employee_Database_challenge.sql file.

* Retrieve the employee number, first and last name, and title columns from the Retirement Titles table.


* Use the DISTINCT ON statement to retrieve the first occurrence of the employee number for each set of rows defined by the ON () clause.


* Exclude those employees that have already left the company by filtering on to_date to keep only those dates that are equal to '9999-01-01'.

* Create a Unique Titles table using the INTO clause.

* Sort the Unique Titles table in ascending order by the employee number and descending order by the last date (i.e., to_date) of the most recent title.

* Export the Unique Titles table as unique_titles.csv.

![image](https://user-images.githubusercontent.com/112978144/227747917-ff06a4f1-7ff8-4a3d-a3a5-3d3391b656a5.png)

After completing all the steps below we got the required table.

* Write another query in the Employee_Database_challenge.sql file to retrieve the number of employees by their most recent job title who are about to retire.

* First, retrieve the number of titles from the Unique Titles table.

* Then, create a Retiring Titles table to hold the required information.

* Group the table by title, then sort the count column in descending order.
![image](https://user-images.githubusercontent.com/112978144/227747981-13c3f2ce-6b0f-425b-aa8f-87318ae2fba8.png)


Export the Retiring Titles table as retiring_titles.csv 

# Deliverable 2

Using the ERD we created in this module as a reference and our knowledge of SQL queries,  we create a mentorship-eligibility table that holds the current employees who were born between January 1, 1965 and December 31, 1965.

* In the Employee_Database_challenge.sql file, we wrote a query to create a Mentorship Eligibility table that holds the employees who are eligible to participate in a mentorship program.

* Retrieve the emp_no, first_name, last_name, and birth_date columns from the Employees table.

* Retrieve the from_date and to_date columns from the Department Employee table.

* Retrieve the title column from the Titles table.

* Use a DISTINCT ON statement to retrieve the first occurrence of the employee number for each set of rows defined by the ON () clause.
* Create a new table using the INTO clause.
* Join the Employees and the Department Employee tables on the primary key.
* Join the Employees and the Titles tables on the primary key.
* Filter the data on the to_date column to all the current employees, then filter the data on the birth_date columns to get all the employees whose birth dates are between January 1, 1965 and December 31, 1965.

* Order the table by the employee number.

* Export the Mentorship Eligibility table as mentorship_eligibilty.csv 
# Deliverable two table
![image](https://user-images.githubusercontent.com/112978144/227748106-ecfe6f8d-9a0c-4f53-a0db-009a6c25f686.png)

# Summary

Pewlett Hackard is a large company boasting several thousand employees, and it's been around for a long time. As baby boomers begin to retire at a rapid rate, Pewlett Hackard is looking toward the future in two ways. First, it's offering a retirement package for those who meet certain criteria. Second, it's starting to think about which positions will need to be filled in the near future.

The number of upcoming retirements will leave thousands of job openings. What would happen to a company if they didn't look ahead and prepare for this many vacancies? It probably wouldn't be pretty.

Bobby is an up-and-coming HR analyst whose task is to perform employee research. Specifically, he needs to find answers to the following questions: Who will be retiring in the next few years? And how many positions will Pewlett Hackard need to fill? This analysis will help future-proof Pewlett Hackard by generating a list of all employees eligible for the retirement package. The employee data Bobby needs is only available in the form of six CSV files because Pewlett Hackard has been mainly using Excel and VBA to work with their data.

But now, they have decided to update their methods to use SQL, a definite upgrade considering the amount of data. our task was to help Bobby build an employee database with SQL by applying our data modeling, engineering, and analysis skills.

After completing all the requirements we got find that at Pewlett Hackard, 64% of their employees are about to retire or being redirected to their mentorship process, which means that they are likely going to need large number of hiring process in their upcoming years. 


