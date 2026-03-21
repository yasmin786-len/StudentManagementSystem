# Student Management System - Spring Boot

A simple **RESTful backend application** built using **Spring Boot** that performs CRUD operations on student data.
This project demonstrates how to build a clean backend architecture using **Controller → Service → Repository → Database** layers.

---

## Technologies Used

* Java 21
* Spring Boot
* Spring Data JPA
* Hibernate ORM
* MySQL
* Maven

---

## 📂 Project Architecture

The application follows a standard layered architecture:

Client
↓
Controller
↓
Service
↓
Repository
↓
MySQL Database

Project structure:

src/main/java/com/example/studentmanagement

* entity → Contains JPA entities (Student.java)
* repository → Handles database access (StudentRepository.java)
* service → Business logic (StudentService.java)
* controller → REST API endpoints (StudentController.java)

---

## 🧩 Features

* Add new student
* Get all students
* Update student details
* Delete student

This project demonstrates **CRUD operations using REST APIs**.

---

## ⚙️ API Endpoints

### Create Student

POST /students

Request Body (JSON):

{
"name": "Rahul",
"email": "[rahul@gmail.com](mailto:rahul@gmail.com)"
}

---

### Get All Students

GET /students

---

### Update Student

PUT /students/{id}

Request Body (JSON):

{
"name": "Rahul Updated",
"email": "[rahulupdated@gmail.com](mailto:rahulupdated@gmail.com)"
}

---

### Delete Student

DELETE /students/{id}

---

## 🗄 Database Configuration

Create a database in MySQL:

CREATE DATABASE studentdb;

Update `application.properties`:

spring.datasource.url=jdbc:mysql://localhost:3306/studentdb
spring.datasource.username=root
spring.datasource.password=YOUR_PASSWORD

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true

---

## ▶️ How to Run the Project

1. Clone the repository

git clone https://github.com/yourusername/student-management-system.git

2. Navigate into the project folder

cd student-management-system

3. Run the application

./mvnw spring-boot:run

or run `StudentManagementApplication.java` from your IDE.

The server will start at:

http://localhost:8080

---

## 🧪 API Testing

You can test the APIs using:

* Postman
* curl
* Browser (for GET requests)

---

## 📌 Future Improvements

* Add validation for request data
* Implement exception handling
* Add DTO pattern
* Implement authentication using Spring Security

---

## 👨‍💻 Author

Developed by **Sayyad Yasmin**

---
