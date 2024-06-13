# FinanceMe Project
FinanceMe is a global leader in banking and financial services based in Germany. This project focuses on transforming the existing monolithic application architecture into a microservice architecture using DevOps practices, leveraging AWS for cloud services, and implementing CI/CD for efficient, reliable, and automated software delivery.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Technologies Used](#technologies-used)
3. [Getting Started](#getting-started)
    - [Prerequisites](#prerequisites)
    - [Installation](#installation)
4. [Running the Application](#running-the-application)
5. [Testing](#testing)
6. [Continuous Integration & Deployment](#continuous-integration--deployment)
7. [Monitoring](#monitoring)


## Project Overview
FinanceMe aims to enhance its application infrastructure by adopting a microservice architecture and DevOps practices. The project involves creating a Mavenized microservice using Spring Boot and an in-memory H2 database, automating deployments with CI/CD pipelines, and monitoring application performance.

## Technologies Used
* **Spring Boot** - for building the microservice.
* **H2 Database** - as the in-memory database for development.
* **Maven** - for continuous build.
* **Git** - for version control.
* **Jenkins** - for continuous integration and deployment.
* **Docker** - for containerizing applications.
* **Ansible** - for configuration management.
* **Terraform** - for infrastructure provisioning.
* **Selenium** - for automated testing.
* **Prometheus and Grafana** - for monitoring and visualization.


## Getting Started
### Prerequisites
* Java 8 or higher
* Maven
* Docker
* Git
* AWS Account
* Terraform
* Ansible
* Jenkins
* Selenium

## Installation

 ### Clone the repository:
```
git clone https://github.com/StarAgileDevOpsTraining/star-agile-banking-finance.git
cd star-agile-banking-finance
```
### Build the project using Maven:
   ```
   mvn clean install
```


## Running the Application

 ### Start the Spring Boot application:
  ```
mvn spring-boot:run
```
 ### Access the application at:
```
http://localhost:8080
```


## Testing
 ### Run JUnit tests:
```
mvn test
```
 ### Generate TestNG report:
```
mvn surefire-report:report

```

## Continuous Integration & Deployment
The CI/CD pipeline is set up using Jenkins. The following tools are used:

* **Git** for version control.
* **Maven** for continuous build.
* **Docker** for containerization.
* **Ansible** for configuration management.
* **Terraform** for infrastructure provisioning.
* **Selenium** for automated testing.

Steps:

- Code is pushed to the GitHub repository.
- Jenkins pipeline is triggered.
- Code is checked out, built, tested, and containerized.
- Infrastructure is provisioned using Terraform.
- Application is deployed using Ansible.
- Automated tests are executed using Selenium.
- If tests pass, the application is deployed to production.


## Monitoring
Prometheus and Grafana are used for monitoring and visualization. The following metrics are monitored:

* CPU utilization
* Disk space utilization
* Total available memory

