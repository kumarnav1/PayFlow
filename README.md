# PayFlow API

## Project Overview

PayFlow is a simplified payment backend application built using Spring Boot, Spring Data JPA, and H2 Database. The application provides REST APIs for user registration, user lookup, and recording money transfer transactions between users.

The project demonstrates a layered Spring Boot architecture consisting of Controller, Service, Repository, and Entity layers.

---

## Tech Stack

* Java
* Spring Boot
* Spring Web
* Spring Data JPA
* H2 Database
* Maven

---

## How to Run

### Clone the Repository

```bash
git clone your-github-repository-url
cd payflow-api
```

### Run the Application

```bash
mvn spring-boot:run
```

The application will start on:

```text
http://localhost:8080
```

### Access H2 Console

```text
http://localhost:8080/h2-console
```

Connection Details:

```text
JDBC URL : jdbc:h2:mem:payflow
Username : sa
Password :
```

---

## API Endpoints


| Method | Endpoint                  | Description                                          |
| ------ | ------------------------- | ---------------------------------------------------- |
| POST   | `/users`                  | Register a new user                                  |
| GET    | `/users`                  | Retrieve all users                                   |
| GET    | `/users/{id}`             | Retrieve user by ID                                  |
| GET    | `/users/upi/{upiId}`      | Retrieve user by UPI ID                              |
| GET    | `/users/balance/{amount}` | Retrieve users with balance above a specified amount |
| POST   | `/transactions`           | Record a money transfer transaction                  |

---

## GitHub Repository

Repository Link:

```text
https://github.com/kumarnav1/PayFlow
```
