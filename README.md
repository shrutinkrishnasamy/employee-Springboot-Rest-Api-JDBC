# 👨‍💼 Employee Spring Boot REST API (JDBC)

A RESTful Employee Management API built using **Spring Boot**, **Spring JDBC**, and **MySQL**. This project demonstrates CRUD (Create, Read, Update, Delete) operations without using JPA or Hibernate, providing direct database interaction through JDBC.

---

## 📖 Overview

This project is designed to demonstrate how to build REST APIs using Spring Boot and JDBC. It follows a layered architecture and exposes endpoints that allow clients to manage employee records using JSON requests and responses.

---

## ✨ Features

- ➕ Add a new employee
- 📋 Retrieve all employees
- 🔍 Retrieve employee by ID
- ✏️ Update employee details
- ❌ Delete employee
- 📦 JSON Request & Response
- 🗄️ MySQL Database Integration
- 🔗 Spring JDBC (JdbcTemplate)
- 🧪 API Testing with Postman
- 🏗️ Layered Architecture

---

## 🛠️ Tech Stack

| Technology | Description |
|------------|-------------|
| Java | Programming Language |
| Spring Boot | Backend Framework |
| Spring JDBC | Database Access |
| MySQL | Relational Database |
| Maven | Dependency Management |
| Postman | API Testing |

Spring Boot's JDBC support simplifies database access through components such as `JdbcTemplate`, making it suitable for lightweight REST applications that don't require an ORM. :contentReference[oaicite:0]{index=0}

---

## 📂 Project Structure

```
src
├── main
│   ├── java
│   │   └── com.example.demo
│   │       ├── controller
│   │       ├── service
│   │       ├── repository
│   │       ├── model
│   │       ├── exception
│   │       └── DemoApplication.java
│   │
│   └── resources
│       ├── application.properties
│       └── schema.sql
```

---

## ⚙️ Prerequisites

- Java 17+
- Maven
- MySQL Server
- Postman
- IntelliJ IDEA / Eclipse

---

## 🔧 Database Configuration

Configure your **application.properties** file.

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/employee_db
spring.datasource.username=root
spring.datasource.password=your_password

spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
```

---

## ▶️ Getting Started

Clone the repository

```bash
git clone https://github.com/shrutinkrishnasamy/employee-Springboot-Rest-Api-JDBC.git
```

Navigate to the project

```bash
cd employee-Springboot-Rest-Api-JDBC
```

Run the application

```bash
mvn spring-boot:run
```

The application will start at:

```
http://localhost:8080
```

---

# 📡 REST API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/employees` | Get all employees |
| GET | `/employees/{id}` | Get employee by ID |
| POST | `/employees` | Add a new employee |
| PUT | `/employees/{id}` | Update employee |
| DELETE | `/employees/{id}` | Delete employee |

---

# 📥 Sample Request

```json
{
  "name": "John Doe",
  "email": "john@example.com",
  "department": "IT",
  "salary": 60000
}
```

---

# 📤 Sample Response

```json
{
  "id": 1,
  "name": "John Doe",
  "email": "john@example.com",
  "department": "IT",
  "salary": 60000
}
```

---

# 🧪 Testing with Postman

All endpoints can be tested using **Postman**.

Example:

```
POST http://localhost:8080/employees
```

Select:

- Body
- Raw
- JSON

Paste the sample JSON and send the request.

---

# 📚 Concepts Covered

- REST API Development
- CRUD Operations
- Spring Boot
- Spring JDBC
- JdbcTemplate
- Dependency Injection
- Exception Handling
- JSON Serialization
- MySQL Database Connectivity
- API Testing with Postman

---

# 🎯 Learning Outcomes

This project helped in understanding:

- Building REST APIs with Spring Boot
- Performing database operations using JDBC
- Layered application architecture
- Request mapping and response handling
- Integrating MySQL with Spring Boot
- Testing REST endpoints using Postman

---

## 👨‍💻 Author

**Shrutin Krishnasamy**

- 💻 Java Backend Developer
- 🚀 Spring Boot Enthusiast
- 🤖 Exploring AI & Full-Stack Development

GitHub: https://github.com/shrutinkrishnasamy

---

## ⭐ Support

If you found this project useful, consider giving it a **⭐ Star** on GitHub.
