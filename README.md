# Employee CRUD - Spring Boot

A simple Employee Management web application built with:

- Java 17
- Spring Boot
- Spring MVC
- Spring Data JPA
- Thymeleaf
- MySQL
- Maven

## CRUD operations

- Create employee
- Read/list employees
- Update employee
- Delete employee

## Database setup

Open MySQL and run:

```sql
CREATE DATABASE employee_db;
```

Then check `src/main/resources/application.properties`.

Default configuration:

```properties
spring.datasource.username=root
spring.datasource.password=root
```

Change the password if your MySQL password is different.

## Run the project

From the project root:

```bash
mvn spring-boot:run
```

Or run `EmployeeCrudApplication.java` from IntelliJ IDEA / Eclipse / VS Code.

Open:

http://localhost:8080/employees

## Project flow

Browser
   ↓
EmployeeController
   ↓
EmployeeService
   ↓
EmployeeRepository
   ↓
MySQL Database
