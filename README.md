# 11th-lesson-with-php-backend-and-mysql

# 11th Lesson – PHP Backend and MySQL

This repository contains code and examples for the 11th lesson of a web development course, focusing on building a simple PHP backend that connects to a MySQL database. It is intended as a learning project to practice basic CRUD operations, form handling, and database integration with PHP.

## Features

- Simple PHP backend with separation between presentation and logic.
- MySQL database integration using standard PHP extensions (e.g., `mysqli` or `PDO`).
- Example CRUD operations (Create, Read, Update, Delete) on a sample table.
- Basic form handling with server-side validation examples.
- Starter structure that can be extended for future lessons.

## Technologies Used

- PHP (version 7.x or 8.x)
- MySQL or MariaDB
- HTML5, CSS3 (for basic frontend templates)
- Apache/Nginx or built-in PHP development server

## Prerequisites

Before running this project, make sure you have:

- PHP installed and added to your system path.
- A running MySQL or MariaDB server.
- A web server (Apache/Nginx) or the PHP built-in server.
- A tool to manage the database (e.g., phpMyAdmin, Adminer, or MySQL CLI).

## Getting Started

Follow these steps to run the project locally:

1. **Clone the repository**
git clone https://github.com/refat-pasha/11th-lesson-with-php-backend-and-mysql.git
cd 11th-lesson-with-php-backend-and-mysql


2. **Create the database**

- Log in to your MySQL server.
- Create a database, for example:

  ```
  CREATE DATABASE lesson11_php_mysql CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;
  ```

- Create the required tables using the provided SQL file (if you add one later, e.g. `database.sql`):

  ```
  SOURCE path/to/database.sql;
  ```

3. **Configure database connection**

- Create a configuration file (for example `config.php`) if it does not exist.
- Add your database credentials:

  ```
  <?php
  $db_host = 'localhost';
  $db_name = 'lesson11_php_mysql';
  $db_user = 'your_username';
  $db_pass = 'your_password';
  ?>
  ```

4. **Run the project**

- If you are using the PHP built-in server:

  ```
  php -S localhost:8000
  ```

- Then open `http://localhost:8000` in your browser.
- If you are using Apache or Nginx, place the project in your server’s document root and access it via your configured virtual host.

## Example Project Structure

You can organize your files similar to this (update this section according to your actual structure):

11th-lesson-with-php-backend-and-mysql/
├── config.php          # Database configuration
├── index.php           # Main entry point (list / home page)
├── create.php          # Form to create a record
├── edit.php            # Form to edit a record
├── delete.php          # Handle delete action
├── includes/
│   ├── db.php          # Database connection helper
│   └── functions.php   # Reusable helper functions
├── public/
│   ├── css/
│   │   └── style.css   # Basic styling
│   └── js/
│       └── main.js     # Optional JavaScript
└── database.sql        # SQL script for tables and sample data



Feel free to rename or rearrange these files to match how your course or lesson is structured.

## How to Use This Lesson

- Read through the PHP files to understand how each operation (create, read, update, delete) is implemented.
- Experiment by changing the database schema and updating the PHP code accordingly.
- Add input validation and error handling to make the backend more robust.
- Use this repository as a base for future lessons that add authentication, APIs, or more complex business logic.

## License

You can choose any license you prefer for this educational project (for example, MIT License). If you add a license, mention it here and include a `LICENSE` file in the repository.




