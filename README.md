# Python_Group9

# Data Storage and Website Presentation
This project is designed to gather data, store it within a SQLite database, and present it using a Flask-based website. The website provides simple formatting and incorporates an About page that offers details regarding the data source and variable definitions.
## Table of Contents
- Data Source
- Database
- Website
- Installation
- Usage

## Data Source
Data for the project is collected from Kaggle Datasets. It consists of 4 data types and total 9 variables. Below are the variables present in the dataset along with their corresponding data types:

- Education: String (str) - Contains textual information about the educational qualifications of employees.
- Joining Year: Integer (int) - Represents the year each employee joined the company.
- City: String (str) - Contains textual information about the location or city where each employee is based or works.
- Payment Tier: String (str) - Categorization of employees into different salary tiers, hence also a string.
- Age: Integer (int) - Represents the age of each employee.
- Gender: String (str) - Contains textual information about the gender identity of employees.
- Ever Benched: Boolean (bool) - Indicates whether an employee has ever been temporarily without assigned work.
- Experience in Current Domain: Float (float) - Represents the number of years of experience employees have in their current field.
- Leave or Not: Boolean (bool) - Target variable, indicating whether an employee has taken leave or not.

## Database
Data is stored in a SQLite database with a single table. Database creation, table creation, and data insertion are performed using the sqlite3 package in Python. Pandas is used as an intermediary for data manipulation.

## Website
The website features the following components:

- Simple formatting for a clean appearance.
- An About page that furnishes details regarding the data source and provides definitions for each variable.
- A Data page that showcases the dataset or a  sample of it.

## Installation
- Clone the repository:

git clone https://github.com/ARDHRA95/Python_Group9

- Install dependencies:

pip install -r requirements.txt

## Usage
- Navigate to the project directory:

cd PYTHON_GROUP9

- Run the Flask server:

python app_template_detail_2.py

- Access the website in your browser at http://localhost:5000