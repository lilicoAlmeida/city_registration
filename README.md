## City and Person Management System
This is a Java-based system for managing cities and people using a graphical user interface (GUI) built with Java Swing. The project interacts with a relational database using JDBC, supporting operations such as creating, reading, updating, and deleting records for cities and people.

## Features
Manage Cities: Add, update, and delete city records with attributes such as code, name, and state (UF).
Manage People: Add, update, and delete person records with attributes such as name, salary, birthdate, and associated city.
Graphical User Interface (GUI): A user-friendly interface to manage cities and people, including dedicated forms for data input and management.
JDBC Integration: Handles database connectivity and operations using Java JDBC.
Data conversion utilities for Date and Double types, ensuring data consistency between the application and the database.
Project Structure
Cidade.java: Entity class representing a city.
Pessoa.java: Entity class representing a person.
Conexao.java: Manages the connection to the relational database using JDBC.
DAOCidade.java: Data Access Object (DAO) for city-related operations in the database.
DAOPessoa.java: Data Access Object (DAO) for person-related operations in the database.
Dados.java: Utility class for managing and processing data.
ConverterData.java & ConverterDouble.java: Utility classes for converting date and double values.
FormCidade.java: GUI form for managing city records.
FormPessoa.java: GUI form for managing person records.
FormPrincipal.java: The main GUI window that allows navigation between the person and city management features.
TesteJDBC.java: A test class to ensure the JDBC connection works as expected.
script.sql: SQL script for setting up the required database schema (tables for Pessoa and Cidade).

## Prerequisites
Java Development Kit (JDK): Version 8 or above.
JDBC Driver: Ensure the JDBC driver for your specific database is included in the project (e.g., MySQL, PostgreSQL).
Database: A relational database such as MySQL, PostgreSQL, or any other supported by JDBC.
SQL Script: Execute the provided script.sql file to create the necessary database tables before running the application.

## Installation and Setup
Clone the Repository:

git clone https://github.com/lilicoAlmeida/city_registration.git
cd city_registration

## Database Setup:

Ensure that your relational database is running and accessible.
Use the script.sql file to create the Pessoa and Cidade tables in the database.
Configure the database connection details in Conexao.java (e.g., URL, username, password).
Build the Project: Compile the Java classes using your preferred IDE (e.g., Eclipse, IntelliJ IDEA) or using the command line:
javac -d bin src/**/*.java
Run the Application: After compiling, you can run the main class (FormPrincipal.java):
java -cp bin pkgmodelo.FormPrincipal

## Usage
Cities: Navigate to the "Cities" section of the GUI to manage city records.
People: Navigate to the "People" section of the GUI to manage person records. You can link people to cities using the appropriate form.

## Troubleshooting
Ensure your JDBC driver is properly configured and accessible.
Verify that your database is running and the connection details in Conexao.java are correct.
If the GUI does not load properly, check the Java version and Swing libraries.

## License
This project is licensed under the MIT License - see the LICENSE file for details.
