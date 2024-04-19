# Python_Group9

# Employee Data Storage and Website Presentation
This project is designed to gather employee data, store it within a SQLite database, and present it using a Flask-based website. The website provides simple formatting and incorporates an About page that offers details regarding the data source and variable definitions.


## Table of Contents
- Data Source
- Database Setup
- Website Implementation
- Installation


## Data Source
Data for the project is collected from Kaggle Datasets.
https://www.kaggle.com/datasets/tawfikelmetwally/employee-dataset

It consists of 4 data types and total 9 variables. Below are the variables present in the dataset along with their corresponding data types:

- Education: String (str) - Contains textual information about the educational qualifications of employees.
- Joining Year: Integer (int) - Represents the year each employee joined the company.
- City: String (str) - Contains textual information about the location or city where each employee is based or works.
- Payment Tier: String (str) - Categorization of employees into different salary tiers, hence also a string.
- Age: Integer (int) - Represents the age of each employee.
- Gender: String (str) - Contains textual information about the gender identity of employees.
- Ever Benched: Boolean (bool) - Indicates whether an employee has ever been temporarily without assigned work.
- Experience in Current Domain: Float (float) - Represents the number of years of experience employees have in their current field.
- Leave or Not: Boolean (bool) - Target variable, indicating whether an employee has taken leave or not.


## Database Setup
Database creation, table creation, and data insertion are performed using the sqlite3 package in Python.

**Data Collection and Database Creation**
The employee data is collected from a CSV file named "Employee.csv" and stored in a SQLite database named "Employee.db".

**Store data in SQLite database as a table**
It reads data from a CSV file named "Employee.csv" and then inserts the data into a table named "Employee".
    
**Database SQL query**
 It executes a SELECT query to fetch all data from the table "Employee"
  

## Website Implementation
The employee data is presented through a Flask web application with the following routes:

**Route for homepage**
route("/"): It renders the template file "index_links.html".Provides links to the about and data pages.

**Route for about page**
route("/about") : It renders the template file "about.html".Contains information regarding sources of data and definition of each variable.

**Route for data page**
route("/data"): Connects to the SQLite database and fetch employee data from the "Employee table" and it renders the template file "data_table.html" and provides the retrieved employee data for display in table format.



## Installation
- Clone the repository:

git clone https://github.com/ARDHRA95/Python_Group9

- Navigate to the project directory:

cd PYTHON_GROUP9

- Install the package:

pip install -r requirements.txt

- Run the Flask web application:

python app_template_detail_2.py

- Access the website in your browser at http://localhost:5000