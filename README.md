# To-Do App

## Overview
This is a simple To-Do application built using **Spring Boot** and **MySQL**. It allows users to manage their tasks efficiently.

## Features
- Add, update, and delete tasks
- Mark tasks as completed
- Store tasks in a MySQL database
- RESTful API implementation

## Tech Stack
- **Java 17+**
- **Spring Boot** (Spring MVC, Spring Data JPA, Hibernate)
- **MySQL**
- **Lombok** (Optional)
- **Postman** (For testing APIs)

## Setup Instructions

### Prerequisites
Ensure you have the following installed:
- [Java 17+](https://adoptopenjdk.net/)
- [Maven](https://maven.apache.org/download.cgi)
- [MySQL](https://dev.mysql.com/downloads/installer/)
- [Postman](https://www.postman.com/) (Optional, for API testing)

### Database Configuration
Update `application.properties` (or `application.yml`) file with your MySQL credentials:

```properties
spring.application.name=todoapp
spring.datasource.url=jdbc:mysql://localhost:3306/todo-app
spring.datasource.username=root
spring.datasource.password=password
spring.jpa.hibernate.ddl-auto=update
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQLDialect
```

### Running the Application
1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/todo-app.git
   cd todo-app
   ```
2. Build the project:
   ```sh
   mvn clean install
   ```
3. Run the Spring Boot application:
   ```sh
   mvn spring-boot:run
   ```

### API Endpoints
| Method | Endpoint       | Description         |
|--------|--------------|---------------------|
| GET    | `/tasks`      | Get all tasks      |
| POST   | `/tasks`      | Create a new task  |
| PUT    | `/tasks/{id}` | Update a task      |
| DELETE | `/tasks/{id}` | Delete a task      |



