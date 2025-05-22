# Java Lab Internal Assessment – Shetty Vinith

This repository contains Java programs for data structures, string handling, Swing GUI, Servlets, JSP, and JDBC projects.

## 📁 Folder Structure

- [1_ArrayList_and_LinkedList](./1_ArrayList_and_LinkedList)
- [2_String_Handling_and_Performance](./2_String_Handling_and_Performance)
- [3_String_Operations_and_Exercises](./3_String_Operations_and_Exercises)
- [4_Swing_Basics_and_Buttons](./4_Swing_Basics_and_Buttons)
- [5_JList_and_TabbedPane](./5_JList_and_TabbedPane)
- [6_Servlet_Basics](./6_Servlet_Basics)
- [7_JSP_Session_and_Cookie_Management](./7_JSP_Session_and_Cookie_Management)
- [8_JDBC_Coffee_and_Emp_CRUD](./8_JDBC_Coffee_and_Emp_CRUD)
- [9_JDBC_Advanced_Coffee_and_Emp](./9_JDBC_Advanced_Coffee_and_Emp)

---

## 🛠️ JDBC and Web Programs Execution Instructions

### 1. Install XAMPP
Download and install from: https://www.apachefriends.org/index.html  
Start **Apache** and **MySQL** from XAMPP Control Panel.

### 2. Setup the Database
- Open [phpMyAdmin](http://localhost/phpmyadmin)
- Import `database.sql` file from this repo to create necessary tables.

### 3. Install Apache Tomcat (for Servlet, JSP, and JDBC Web programs)
- Download Apache Tomcat 9 or 10 from: https://tomcat.apache.org/download-90.cgi  
  (Versions 6 to 10 are compatible, but newer is recommended.)
- Install and configure Tomcat.

### 4. Deploy Web Programs
- Copy your `.jsp`, `.java` servlet classes (compiled to `.class`) and related files into the Tomcat `webapps` folder under your project directory.
- Alternatively, use an IDE like Eclipse or IntelliJ IDEA configured with Tomcat to run and debug programs.

### 5. Configure JDBC Driver in Tomcat
- Place the MySQL Connector/J JAR file (`mysql-connector-java-x.x.x.jar`) in the Tomcat `lib` folder.

### 6. Update Database Connection Details
In your Java/JSP files, ensure the connection string matches your MySQL setup, for example:

```java
Connection con = DriverManager.getConnection("jdbc:mysql://localhost:3306/your_db_name", "root", "");
