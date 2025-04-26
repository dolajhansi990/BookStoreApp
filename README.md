Bookstore Application:

A simple web-based bookstore application built using Spring 5.2 and Hibernate 5.4. The application allows users to view, add, edit, and delete books from the catalog.

Features:

1.View all books in the store
2.Add new books
3.Edit existing books
4.Delete books
5.Paginated book listing

Technologies Used:

Backend: Spring MVC, Hibernate, Java Mail API

Frontend: JSP, JSTL

Database: MySQL

Build Tool: Maven

Server: Tomcat 8.5

Project Structure

BookStoreApplication/
│── src/
│   ├── com.jlcindia.spring.config/
│   │   ├── JLCWebAppInitializer.java
│   │   ├── JLCWebConfig.java
│   ├── com.jlcindia.spring.controller/
│   │   ├── BookController.java
│   │   ├── IndexController.java
│   ├── com.jlcindia.spring.dao/
│   │   ├── BookDAO.java
│   ├── com.jlcindia.spring.daoimpl/
│   ├── com.jlcindia.spring.entity/
│   ├── com.jlcindia.spring.service/
│   ├── com.jlcindia.spring.serviceimpl/
│── build/
│── webapp/
│   ├── META-INF/
│   ├── WEB-INF/
│   │   ├── lib/  # Libraries folder for dependencies
│   │   ├── myjsps/
│   │   │   ├── addEditBook.jsp
│   │   │   ├── booksList.jsp
│   │   │   ├── index.jsp
│   │   │   ├── viewBook.jsp
│── Servers/
│── pom.xml
│── README.md

Installation and Setup:

Prerequisites:

JDK 8 or later

MySQL database

Apache Maven

Tomcat 8.5

Eclipse IDE (or any preferred IDE)

Steps to Run:

1. Add required JAR files

Download and add the following libraries to the webapp/WEB-INF/lib/ folder:
Spring JARs

Hibernate JARs

MySQL Connector JAR

JSTL JAR

2. Clone the repository

git clone https://github.com/yourusername/bookstore-app.git
cd bookstore-app

3. Set up the MySQL database

CREATE DATABASE bookstoredb;

4. Update database credentials in JLCWebConfig.java

ds.setUrl("jdbc:mysql://localhost:3306/bookstoredb");
ds.setUsername("your_mysql_user");
ds.setPassword("your_mysql_password");
You can download these from Maven repositories or official websites.

5. Run the application in Eclipse

Open Eclipse

Right-click on BookStoreApplication

Select Run As > Run on Server

Choose Apache Tomcat 8.5 and click Next

Click Finish to start the server

6. Access the application
Open a web browser and navigate to:
http://localhost:12345/BookStoreApplication/

Conclusion:
The Bookstore Application efficiently manage books using Spring MVC, Hibernate, MySQL and JSP enabling users to add, edit, view and delete books. It provides a scalable foundation for future enhancements like authentication, search and cloud deployment.



