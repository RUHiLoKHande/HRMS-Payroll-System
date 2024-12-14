# HRMS-Payroll-System
The HRMS Payroll System manages employee data and generates salary slips. Built with Java Spring Boot (backend) and React.js (frontend), it allows adding, updating, and deleting employees. Salary slips are generated automatically, and the project uses PostgreSQL for database storage.

Technologies Used
Backend:
Java 17 (or later): For backend development.
Spring Boot: For building REST APIs and handling server-side logic.
Spring Data JPA: To interact with the PostgreSQL database.
PostgreSQL: For database management.
Frontend:
React.js: For creating the user interface and managing frontend logic.
HTML/CSS: For structuring and styling the web pages.
JavaScript: For dynamic functionalities on the frontend.
Additional:
PDF Generation: For generating and downloading salary slips as PDF files.
Features
Employee Management:

Add an employee with details like Name, Email, Designation, Basic Salary, and Department.
View all employees in a table format.
Update and delete employee details.
Salary Slip Generation:

Automatically calculate:
PF Deduction: 12% of Basic Pay.
Professional Tax: ₹200 (fixed).
Net Salary: Basic Pay - (PF Deduction + Professional Tax).
Generate and download salary slips as PDF files.
Database Schema
Employee Table:
id (Primary Key)
name
email
designation
basic_salary
department
Salary Slip Table:
id (Primary Key)
employee_id (Foreign Key, references Employee table)
pf_deduction
professional_tax
net_salary
Setup Instructions
Prerequisites:
Java 17 (or later) installed on your machine.
Node.js (for React frontend).
PostgreSQL installed and running.

Example Usage
Add Employee: Fill in the form with employee details like name, email, and basic salary, then submit the form to add the employee.
Generate Salary Slip: Select an employee from the list and click on "Generate Salary Slip" to calculate deductions and download the salary slip.
    
