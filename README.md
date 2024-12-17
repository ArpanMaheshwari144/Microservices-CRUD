# Insurance System Backend and Customer Microservice

**Description:**  
This project comprises two microservices:
1. **Policy Microservice**
2. **Customer Microservice**

This microservices setup is built using Spring Boot and follows best practices for microservices architecture, including RESTful APIs and database connectivity.

## Table of Contents
- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
- [Running the Application](#running-the-application)
- [Configuration](#configuration)
- [Database Schema](#database-schema)

## Prerequisites
Before you begin, ensure you have the following installed:
- [Java 8+](https://www.oracle.com/java/technologies/javase-jdk8-downloads.html)
- [Maven 3+](https://maven.apache.org/download.cgi)
- [Git](https://git-scm.com/)
- An IDE of your choice (e.g., IntelliJ IDEA, Eclipse)

## Getting Started
To get started, clone the repository and set up the backend and microservices:
1. Clone the repository:
    ```bash
    git clone https://github.com/ArpanMaheshwari144/Microservices-CRUD.git
    ```

2. Build the project:
    ```bash
    mvn clean install
    ```

## Running the Customer Microservice
To run the **Customer Microservice**, follow these steps:
1. Navigate to the project directory:
    ```bash
    cd customer-microservice
    ```

2. Run the application:
    ```bash
    mvn spring-boot:run
    ```

## Running the Policy Microservice
To set up and run the **Policy Microservice**, follow these steps:
1. Navigate to the project directory:
    ```bash
    cd policy-microservice
    ```

2. Run the application:
    ```bash
    mvn spring-boot:run
    ```

## Configuration
Configuration files are located in the `src/main/resources` directory. Update the following properties in `application.properties` for both the **Microservices-CRUD** and **Customer Microservice**:

- **Database Configuration for Microservices-CRUD:**
  ```properties
  spring.datasource.url=jdbc:mysql://localhost:3306/insurance_db
  spring.datasource.username=root
  spring.datasource.password=yourpassword
  spring.jpa.hibernate.ddl-auto=update
