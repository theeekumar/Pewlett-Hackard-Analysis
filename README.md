# Pewlett-Hackard-Analysis
## Overview of the analysis
Create entity relationship diagrams, perform data modeling, and complete analysis on an employee database using SQL techniques.
### Purpose 
The purpose of this analysis was to help Bobby's manager prepare for the "silver tsunami"  by determining the number of retiring employees per title and identifying employees who are eligible to participate in a mentorship program.
### Resources
Data Source:
- departments.csv
- dept_emp.csv
- dept_manager.csv
- employees.csv
- salaries.csv
- titles.csv

Software:
- SQL
- PostgreSQL
- pgAdmin
## Results
- The Unique Titles table was created by retrieving columns from the Retirement Titles table, using the DISTINCT ON statement to retrieve the first occurence of the employee number for each set of rows, filtering the table by current employees only, and sorting the table in ascending order by employee number and descending order by the last date of the most recent title. The results of the table revealed how there are **90,398 employees retiring according to the table's criteria.**

![8806A8E2-9516-4265-8FA9-E3D669B38D98_4_5005_c](https://user-images.githubusercontent.com/92240407/150467799-6768bee1-bc6a-4ec9-8f7d-e0ce72eec0ee.jpeg)

- The Retiring Titles table was created by retrieving the number of titles from the Unqiue Titles table, applying the COUNT function, grouping the table by title, and sorting the count column in descending order. The results of the table revealed the exact amount of employees retiring from each title: **29,414 from Senior Engineer, 28,254 from Senior Staff, 14,222 from Engineer, 12,243 from Staff, 4,502 from Technique Leader, 1,761 from Assistant Engineer, and 2 from Manager.**

![947EEF54-C539-4DCF-8620-B3DD9101F1FB_4_5005_c](https://user-images.githubusercontent.com/92240407/150468754-539a70fd-aa51-46b0-aaa2-ac9e0d32b628.jpeg)

- The Mentorship Eligibilty table was created by retrieving the columns from the Employees, Department Employees, and Titles table, applying the DISTINCT ON statement to the employee number, joining tables, and filtering/ordering the data. The results of the table revealed how there are **1,549 employees applicable for the Mentorship Eligibilty program.**
![340EA532-9AB2-464B-82F5-5A794D9C0FE7_4_5005_c](https://user-images.githubusercontent.com/92240407/150470099-ec553705-5f61-4edf-8c3f-abe65137a7f7.jpeg)

- The ERD (Entity Relationship Diagram) was created as the first step in this analysis to help visualize the relationship between the different data tables and to act as a guideline for creating queries. 

![25C9CD77-D58F-4D03-9C88-22ECB03653AE](https://user-images.githubusercontent.com/92240407/150470329-72bbe43d-a5df-47e5-b53e-2755829a9fb6.jpeg)

## Summary
Due to the "silver tsunami" arriving at the company, about 30% of the amount of employees will be retiring. This means the titles for the rows from the results we found will need t be filled. From the results of the Mentorship Eligibilty table, there seems to be enough qualified, retirement-ready employees in the departments to mentor th next generation of Pewlett Hackard employees.









