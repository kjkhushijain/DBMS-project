# E-Commerce Website

## Overview
This is a fully functional e-commerce website built using **Spring Boot** and **Thymeleaf** with a **MySQL database**. The project includes user authentication, product management, cart, orders, payments, and wishlist features.

## Features
- **User Authentication**: Register, login, and manage user accounts.
- **Product Management**: View, search, and filter products.
- **Shopping Cart**: Add and remove items, manage quantities.
- **Order Processing**: Place orders and track order history.
- **Payments**: Integrated payment gateway.
- **Wishlist**: Save favorite products.
- **Admin Dashboard**: Manage products, orders, and users.

## Technologies Used
- **Backend**: Spring Boot, Spring Security, Hibernate, JPA
- **Frontend**: Thymeleaf, HTML, CSS, JavaScript
- **Database**: MySQL
- **Build Tool**: Maven

## Setup Instructions

### Prerequisites
- Java 17+
- MySQL Server
- Maven
- Git

### Steps to Run the Project
1. Clone the repository:
   ```sh
   git clone https://github.com/kjkhushijain/DBMS-project.git
   cd DBMS-project
   ```

2. Configure the database:
   - Create a MySQL database named `ecommerce_db`.
   - Update `src/main/resources/application.properties` with your MySQL credentials:
     ```properties
     spring.datasource.url=jdbc:mysql://localhost:3306/ecommerce_db
     spring.datasource.username=root
     spring.datasource.password=yourpassword
     ```

3. Import the database schema:
   - Run the SQL script located in `database.sql`.

4. Build and run the project:
   ```sh
   mvn clean install
   mvn spring-boot:run
   ```

5. Access the application:
   - User Interface: `http://localhost:8080`
   - Admin Panel: `http://localhost:8080/admin`

## Folder Structure
```
Ecom-main/
│── src/
│   ├── main/
│   │   ├── java/ecom/demo/
│   │   │   ├── controllers/
│   │   │   ├── models/
│   │   │   ├── repositories/
│   │   │   ├── services/
│   │   ├── resources/
│   │   │   ├── templates/
│   │   │   ├── static/
│   ├── test/
│── database.sql
│── mvnw.cmd
│── pom.xml
│── README.md
```

## Contributors
- **Khushi Jain** ([GitHub](https://github.com/kjkhushijain))

## License
This project is licensed under the MIT License.

