# JDBC_hospital

# Hospital Management System

This is a simple Java application that implements a hospital management system using a MariaDB database for storing and managing doctors' data. The application allows the user to perform basic CRUD (Create, Read, Update, Delete) operations on the doctors' data stored in the database.

## Prerequisites

To run this application, you need to have the following software installed on your machine:

- Java Development Kit (JDK) 8 or higher
- MariaDB database server
- MariaDB JDBC driver

## Getting Started

Follow the instructions below to set up and run the hospital management system application:

1. Clone the repository or download the source code.
2. Set up the MariaDB database by running the SQL script `hospitalDB.sql` provided in the repository. This will create the necessary database and table.
3. Update the database connection details in the `openDatabaseConnection()` method of the `Application` class. Replace the `jdbc:mariadb://localhost:3306/hospitalDB`, `davidramirez`, and `password` with your own database URL, username, and password.
4. Compile the Java source code using a Java compiler of your choice.
5. Run the `Application` class to start the hospital management system application.

## Features

The hospital management system application provides the following features:

- Adding doctors: The user can enter the details of a doctor, including name, age, and speciality, and the data will be stored in the database.
- Reading doctors: The user can view the list of doctors stored in the database, sorted by age in descending order.
- Updating doctor's speciality: The user can update the speciality of a doctor by entering the doctor's name and the new speciality.
- Querying doctors by speciality: The user can query the doctors by entering a speciality, and the application will display the list of doctors with that speciality.
- Deleting doctors: The user can delete a doctor by entering the doctor's name, and the data will be deleted from the database.

## Usage

Upon running the hospital management system application, the user will be prompted with a series of options to perform various operations on the doctors' data. The user can follow the on-screen instructions to input the required data and perform the desired operation.

Please note that the application uses the `PreparedStatement` interface to execute SQL queries, which helps prevent SQL injection attacks by automatically escaping user input. However, it is always recommended to validate and sanitize user input to ensure data integrity and security.

## License

This hospital management system application is open-source and available under the MIT License. Feel free to use, modify, and distribute the code for personal and commercial purposes. However, please attribute the original authors by including a reference to this repository.
