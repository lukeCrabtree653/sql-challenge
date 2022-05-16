# sql-challenge
HW9


1)
SELECT employees.emp_no,last_name,first_name,sex,salary 
FROM employees
INNER JOIN salaries
ON employees.emp_no=salaries.emp_no
