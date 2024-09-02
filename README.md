This project is a Spring Boot application that is part of a bigger system, related to big data and cloud computing (BDCC). The project includes various configurations and controllers designed to work with external APIs, such as OpenAI.

## Prerequisites
Before you begin, ensure you have met the following requirements:

- **Java JDK 11 or later**: Required for running Spring Boot.
- **Maven**: For building and managing the project dependencies.
- **MySQL**: Ensure you have MySQL installed for the database setup.

## Setup Instructions

### Clone the Repository
To start working with this project, you first need to clone it to your local machine:

```bash
git clone https://github.com/HIBA-ACHIR/projet-enset-bdcc.git
cd projet-enset-bdcc
```

### Configure the MySQL Database
1. Create a MySQL database named `bdcc`.
2. Update the `application.properties` file located in `src/main/resources/` with your MySQL credentials:

   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/bdcc
   spring.datasource.username=yourUsername
   spring.datasource.password=yourPassword
   ```

### Build and Run the Project
1. **Build the project:**

   ```bash
   mvn clean install
   ```

2. **Run the project:**
   ```bash
   mvn spring-boot:run
   ```

   The application should now be running on `http://localhost:8080`.

### Testing
You can run the unit tests provided in the project to ensure everything is working correctly:

```bash
mvn test
```

## Usage

- Access the application via `http://localhost:8080`.
- The project includes a REST controller (`OpenAiRestController`) that interacts with external APIs.

## Contributing

To contribute to this project, follow these steps:

1. Fork this repository.
2. Create a branch: `git checkout -b feature/AmazingFeature`.
3. Make your changes and commit them: `git commit -m 'Add some AmazingFeature'`.
4. Push to the branch: `git push origin feature/AmazingFeature`.
5. Open a pull request.

