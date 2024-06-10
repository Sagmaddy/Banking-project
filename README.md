#Overview:
FinanceMe is a project aimed at transforming a monolithic banking application into a scalable microservice architecture using Spring Boot and an in-memory H2 database. The project implements DevOps practices to automate the CI/CD pipeline and streamline software delivery processes.

#Prerequisites:

JDK 8 or higher installed
Maven installed
Docker installed
Ansible installed
Jenkins installed and configured
Getting Started:

#Clone the repository:

bash
Copy code
git clone https://github.com/StarAgileDevOpsTraining/star-agile-banking-finance.git
Build the project:

bash
Copy code
cd star-agile-banking-finance
mvn clean install
Set up Jenkins:

#Install Jenkins if not already installed.
Go to "Manage Jenkins" > "Manage Plugins" > "Available" and install the Docker and Ansible plugins.
Configure Docker and Ansible in Jenkins:

#Ensure Docker and Ansible are properly installed on the Jenkins server.
Configure Jenkins to run Docker and Ansible commands without requiring passwords.
Run the application:

#Start Jenkins and navigate to the project.
Set up the CI/CD pipeline to trigger on changes to the master branch.
Push changes to the master branch to automatically trigger the CI/CD pipeline.
Monitor application performance:

#Utilize Prometheus and Grafana to monitor CPU utilization, disk space utilization, and total available memory.
Access Grafana dashboard to visualize metrics and ensure application reliability and performance.
Endpoints:

POST /createAccount
PUT /updateAccount/{accountNumber}
GET /viewPolicy/{accountNumber}
DELETE /deletePolicy/{accountNumber}
Testing:

#JUnit test cases are provided to ensure the functionality of the microservice.
Generate HTML reports using TestNG for comprehensive test coverage.
Continuous Integration & Deployment:

#Jenkins is configured to automate the CI/CD pipeline.
On pushing updates to the master branch, the code is compiled, tested, packaged, and containerized.
Terraform provisions a test server, automatically configured using Ansible, and the application is deployed.
Test automation tools verify the deployment, and if successful, the application is deployed to the production server.
Validation:

#Validate the solution against the provided GitHub repository: StarAgileDevOpsTraining/star-agile-banking-finance
Contributing:

#Contributions to the FinanceMe project are welcome. Please fork the repository, make changes, and submit a pull request.

3License:
This project is licensed under the MIT License.

#Acknowledgements:
Special thanks to the contributors and developers of the FinanceMe project.
