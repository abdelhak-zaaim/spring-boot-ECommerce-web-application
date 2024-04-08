## Introduction

This project is a web application developed using Java, Spring Boot, and JavaScript. It provides an e-commerce platform where users can view, add, and manage products.

## Prerequisites

Before you begin, ensure you have met the following requirements:

- You have installed the latest version of Java, Maven, and Mysql.
- You have a `<Windows/Linux/Mac>` machine. State which OS is supported or all.

## Installation :wrench:

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

```bash
# Clone the repository
git clone https://github.com/Zaaim-Halim/spring-boot-ECommerce-web-application.git

# Navigate to the project directory
cd spring-boot-ECommerce-web-application

```

## Database Configuration

This application is configured to use a MySQL database. The configuration is specified in the `application.properties` file in the `src/main/resources` directory:

1. Install MySQL on your machine. You can download it from [here](https://dev.mysql.com/downloads/installer/).

2. Once installed, create a new database for the application. You can do this via the MySQL command line interface or a GUI tool like MySQL Workbench. Here's how you can do it via the command line:

   ```bash
   mysql -u root -p
   CREATE DATABASE your_database_name;
    ```
   
- `spring.datasource.url`: JDBC URL for the MySQL database. Specifies the database server's location, the database name, and several connection parameters.
- `spring.datasource.username` and `spring.datasource.password`: Username and password to connect to the MySQL database.
- `spring.jpa.properties.hibernate.dialect`: Tells Hibernate to generate SQL queries that are compatible with MySQL.
- `spring.jpa.hibernate.ddl-auto`: Hibernate will automatically create or update the database schema on startup.
- `logging.level.org.hibernate.SQL`: Hibernate will log all the SQL statements it generates.
- `server.port`: The port number on which the Spring Boot application will run.
- `spring.banner.charset`: The character set for the Spring Boot banner.

Please update these properties with your actual MySQL configuration.

