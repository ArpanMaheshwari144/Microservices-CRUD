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
- [Testing](#testing)
- [Configuration](#configuration)
- [API Endpoints](#api-endpoints)
- [Database Schema](#database-schema)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

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
    git clone https://github.com/your-username/insurance-system-backend.git
    cd insurance-system-backend
    ```

2. Build the project:
    ```bash
    mvn clean install
    ```

## Running the Insurance System Backend
To run the **Insurance System Backend**, follow these steps:
1. Navigate to the project directory:
    ```bash
    cd insurance-system-backend
    ```

2. Run the application:
    ```bash
    mvn spring-boot:run
    ```

3. Access the API at `http://localhost:8081`.

## Running the Customer Microservice
To set up and run the **Customer Microservice**, follow these steps:
1. Navigate to the project directory:
    ```bash
    cd customer-microservice
    ```

2. Build the project:
    ```bash
    mvn clean install
    ```

3. Run the application:
    ```bash
    mvn spring-boot:run
    ```

4. Access the API at `http://localhost:8082`.

## Testing
To run unit and integration tests:
1. Run the tests for the **Insurance System Backend**:
    ```bash
    mvn test
    ```

2. Run the tests for the **Customer Microservice**:
    ```bash
    mvn test
    ```

## Configuration
Configuration files are located in the `src/main/resources` directory. Update the following properties in `application.properties` for both the **Insurance System Backend** and **Customer Microservice**:

- **Database Configuration for Insurance System Backend:**
  ```properties
  spring.datasource.url=jdbc:mysql://localhost:3306/insurance_db
  spring.datasource.username=root
  spring.datasource.password=yourpassword
  spring.jpa.hibernate.ddl-auto=update
