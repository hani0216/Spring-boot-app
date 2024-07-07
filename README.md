This project demonstrates the creation of a CI/CD pipeline for a Spring Boot application using GitHub Actions for continuous integration and Docker Hub for containerization and deployment.

Features :

Automated Builds: Every push to the main branch triggers the pipeline.
Unit Testing: Executes unit tests to ensure code quality.
Build and Packaging: Compiles and packages the application using Apache Maven.
Docker Integration: Builds a Docker image from the application and pushes it to Docker Hub.

GitHub Actions Workflow :

The GitHub Actions workflow (.github/workflows/ci-cd.yml) is configured to perform the following steps:

Checkout Code: Fetches the latest code from the repository.
Setup JDK: Configures JDK 17 using Corretto distribution.
Unit Tests: Runs the unit tests with Maven.
Build the Application: Cleans and packages the application.
Build Docker Image: Builds a Docker image from the application.
Login to Docker Hub: Authenticates to Docker Hub using secrets stored in GitHub.
Push to Docker Hub: Pushes the Docker image to Docker Hub.
