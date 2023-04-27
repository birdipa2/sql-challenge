# sql-challenge
# Employee Database Analysis

This project aims to analyze employee data from six different CSV files using PostgreSQL and SQLAlchemy. The project includes data modeling, data engineering, and data analysis.

The repository contains a main folder named [EmployeeSQL] and a ReadMe file. Within the main folder, there is a subfolder named [data] containing six CSV files that were used for employee data analysis. Additionally, there are two SQL files included in the main folder: 'Table_Schemata.sql' which was used to create a table schema for each of the six CSV files, and 'Queries.sql' which was used to analyze the employee data. The main folder also includes a snapshot of the Entity Relationship Diagram in both image and text file formats.

## Data Modeling

First, the CSV files were inspected, and an Entity Relationship Diagram (ERD) was sketched using QuickDBD. The ERD included six tables: departments, dept_emp, dept_manager, employees, salaries, and titles.

## Data Engineering

Next, a table schema was created for each CSV file. The schema included the data types, primary keys, foreign keys, and other constraints. The tables were created in the correct order to handle the foreign keys. Finally, each CSV file was imported into its corresponding SQL table. It is imperative to import the tables in the following order:
1. departments
2. titles
3. employees
4. dept_emp
5. dept_manager
6. salaries

## Data Analysis

Once the data was imported, several queries were executed to analyze the employee data. The following queries were executed:

1. List the employee number, last name, first name, sex, and salary of each employee.
2. List the first name, last name, and hire date for the employees who were hired in 1986.
3. List the manager of each department along with their department number, department name, employee number, last name, and first name.
4. List the department number for each employee along with that employee’s employee number, last name, first name, and department name.
5. List first name, last name, and sex of each employee whose first name is Hercules and whose last name begins with the letter B.
6. List each employee in the Sales department, including their employee number, last name, and first name.
7. List each employee in the Sales and Development departments, including their employee number, last name, first name, and department name.
8. List the frequency counts, in descending order, of all the employee last names (that is, how many employees share each last name).

## Conclusion

Through the above analysis, we can extract useful insights from employee data, such as the salary distribution of employees, the number of employees hired in a specific year, and the department-wise employee count. The analysis can help in decision-making processes, such as salary adjustments, department restructuring, and employee retention.

## Contact

If you have any questions or feedback about this script, please feel free to contact me at param.birdi@utoronto.ca.

## Acknowledgments

This code was written by Paramdeep Singh Birdi as part of a project for a data analysis course. Most of the data used in this project was provided by the course instructors.
