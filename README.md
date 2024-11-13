# Gym Management System

A simple web-based gym management system developed using PHP, MySQL, and HTML/CSS. This system allows administrators to manage gym members, add new members, delete existing members, and view all registered members in a tabular format.

## Features

- **Login System**: Users (admin) must log in to access the members page.
- **Member Management**: Add, delete, and view gym members.
- **Responsive Interface**: The system is designed to work on both desktop and mobile devices.
- **Database Integration**: All member data is stored in a MySQL database.

## Technologies Used

- **PHP**: For server-side scripting and handling the logic.
- **MySQL**: For storing and managing gym members' data.
- **HTML/CSS**: For the front-end structure and design.
- **XAMPP**: For local development and running the Apache server and MySQL database.

## Prerequisites

To run this project locally, you need to have the following installed:

- [XAMPP](https://www.apachefriends.org/index.html) (or any PHP and MySQL environment)
- A web browser (e.g., Chrome, Firefox)

## Setup Instructions

1. **Clone the Repository** (or download the project files):
   ```bash
   git clone (https://github.com/Adityamaurya790/GymManagement.git)
   
2. **Install XAMPP:

    Download and install XAMPP from the official site.
    Start the Apache and MySQL services via the XAMPP control panel.

3. **Create a Database:

    Open phpMyAdmin in your browser (usually at http://localhost/phpmyadmin).
    Create a new database named gym_management.

4. **Set Up the Database:

    Import the SQL file (if provided) or create the necessary tables in the database.
    Create a users table for admin login and a members table for storing member information.

Example SQL for creating users table:

CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    username VARCHAR(50) NOT NULL,
    password VARCHAR(255) NOT NULL
);

Example SQL for creating members table:

CREATE TABLE members (
    id INT PRIMARY KEY,
    name VARCHAR(100) NOT NULL,
    age INT NOT NULL,
    membership_type VARCHAR(50) NOT NULL
);

5. **Configure Database Connection:

    Open the login.php and other PHP files that handle database connections.
    Ensure the servername, username, password, and dbname variables match your MySQL setup.

6. **Access the Application:

    Open your web browser and go to http://localhost/gym_management/login.php to start using the system.
    Log in with the appropriate admin credentials (you can add a user in the users table in the database).

Live Demo: You can also view the live version of the project at gym-project.wuaze.com.
