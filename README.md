# sql-challenge
HW9


1)
SELECT employees.emp_no,last_name,first_name,sex,salary 
FROM employees
INNER JOIN salaries
ON employees.emp_no=salaries.emp_no

2)
SELECT first_name,last_name,hire_date 
FROM employees
WHERE hire_date LIKE '%1986'

3)
SELECT departments.dept_no,dept_name,employees.emp_no, last_name, first_name
FROM dept_manager
INNER JOIN employees
ON dept_manager.emp_no = employees.emp_no
INNER JOIN departments
ON dept_manager.dept_no = departments.dept_no

4)
SELECT employees.emp_no,last_name,first_name,dept_name
FROM dept_emp
INNER JOIN employees
ON dept_emp.emp_no = employees.emp_no
INNER JOIN departments
ON dept_emp.dept_no = departments.dept_no

5)
SELECT first_name,last_name,sex
FROM employees
WHERE first_name = 'Hercules'
AND last_name LIKE 'B%'

6)
