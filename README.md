# College Registration & Login System

A simple Java desktop application to handle faculty registration and login functionality for a college system using Swing GUI and MySQL for database storage.

## 🔍 Overview

This project is built using **Java Swing** and **MySQL**, allowing secure registration and login for faculty members. It includes user-friendly features like password hiding/showing, validation for correct faculty ID, and clean form transitions.

## 🧰 Features

- 🔐 Faculty login with credential validation  
- 📝 Registration page with:
  - Faculty ID verification from database
  - Password and confirm password matching
  - Toggle password visibility
- 🎯 GUI-based application with intuitive form layout
- 📂 Connected to MySQL using JDBC
- ❌ Error handling and input validations

## 📸 UI Screens

- Welcome Page  
- Login Page  
- Registration Page  
- Admin Dashboard

## 💻 Technologies Used

- Java (Swing)
- NetBeans IDE
- MySQL
- JDBC (Java Database Connectivity)

## 📂 Database Structure

### Database Name: `regdetails`

- Table `fid`  
  - `id` (faculty ID to verify during registration)

- Table `regd`  
  - `UserName` (username of faculty)
  - `NewPass` (hashed or raw password - can be improved for security)

## 🚀 Getting Started

### Prerequisites

- NetBeans installed
- MySQL server running
- MySQL JDBC connector added to the project

### Steps to Run

1. Clone or download this repo.
2. Set up your MySQL database and run the required `CREATE TABLE` queries.
3. Open the project in NetBeans.
4. Update DB credentials in the code:
   ```java
   Connection con = DriverManager.getConnection("jdbc:mysql://127.0.0.1:3306/regdetails", "root", "your_password");
   ```
5. Run the `Welcome` class to launch the application.

## 📌 Future Enhancements

- Password hashing for secure storage  
- Faculty and student module separation  
- Role-based login (admin vs user)  
- Search & view registered data  
- Export to CSV

## 📚 Topics

```
java swing netbeans jdbc mysql database crud login-system registration gui password-toggle jframe sql-authentication
```

## 📃 License

This project is for educational/demo purposes.

---

**Made with ❤️ by Imran Shaik**
