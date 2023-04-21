# Hospital Database Application

This is a Java application that interacts with a hospital database using JDBC (Java Database Connectivity). It allows you to perform basic CRUD (Create, Read, Update, Delete) operations on the database, such as adding doctors, reading doctor information, updating doctor speciality, querying doctors by speciality, and deleting doctors.

## Requirements

- Java Development Kit (JDK) 8 or higher
- MariaDB or MySQL database server
- JDBC driver for MariaDB or MySQL (included in the application)

## Setup

1. Clone the repository or download the source code.
2. Make sure you have a MariaDB or MySQL database server running and accessible.
3. Import the database schema using the `hospitalDB.sql` script provided in the repository.
4. Open the `Application` class in your Java IDE or editor of choice.
5. Update the database connection details in the `openDatabaseConnection()` method, including the database URL, username, and password.
6. Build and run the application.

## Usage

The application provides a command-line interface to interact with the hospital database. You can perform the following operations:

- **Read data**: Displays the list of doctors in the database, ordered by age in descending order.
- **Create data**: Allows you to add new doctors by providing their name, speciality, and age.
- **Update data**: Lets you update the speciality of a doctor by providing their name and the new speciality.
- **Delete data**: Allows you to delete doctors by their name or a partial name match.
- **Query data**: Lets you query doctors by their speciality, displaying their name, age, and speciality.

Note: The application uses a `try-with-resources` statement to ensure proper resource management and closing of database connections.

## Example Usage

Here's an example of how you can use the application:

1. Run the application.
2. Choose the appropriate option from the menu to perform the desired operation (e.g., create, read, update, delete, or query data).
3. Follow the prompts to provide the necessary input for the operation.
4. View the results of the operation in the console output.
5. Repeat steps 2-4 for other operations or exit the application when done.

