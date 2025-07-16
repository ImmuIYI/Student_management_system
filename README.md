# 🎓 College Graduated Students Management System (Java Swing)

A desktop-based Java Swing application to manage records of already graduated students. Built purely using Java Swing and JDBC with MySQL — no frameworks like Spring Boot or REST APIs used. Designed for admin/faculty access only, with secure login and faculty ID validation.

## 🎯 Features

- 🔐 **Login and Registration System**
  - Admin/faculty can register and login securely.
  - Faculty ID must be valid (verified from MySQL `fid` table).
  - Re-enter password validation included.

- 🧑‍🎓 **Student Record Management**
  - View student details based on roll number from the database.
  - Edit and Delete the student Details based on roll number from the database.
  - And we can see Academic details of the Students. 
  - Results displayed in a `JTable_studentdetails`-based UI.

- 👁️ **Password Visibility Toggle**
  - Show/hide password functionality using a checkbox.
  - Hidden by default with dot `•` characters.

- 🔄 **Navigation Between Screens**
  - Seamless transitions between Login, Register, Welcome, Admin, and Info pages using `JFrame` controls.

- ⚠️ **Form Validation & Error Handling**
  - Empty field checks.
  - Password match validation.
  - Dialogs for incorrect login or invalid data using `JOptionPane`.

- 🧩 **Modular Structure**
  - Each screen in its own class (Login.java, Register.java, Admin.java, etc.).
  - Easy to modify and scale.

- 💡 **No External Libraries or Frameworks**
  - Fully functional without Spring Boot, REST APIs, or third-party tools.


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

- Table `studentdetails`

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
