Project Setup and Configuration
Welcome to the My Project Setup repository! This project provides a comprehensive guide for deploying and configuring a front-end and back-end application with Docker, setting up MySQL, and configuring load balancers for high availability. Below is a detailed description of each component included in this repository.

Repository Structure
docker-compose/
front-end/
docker-compose.yml: Configuration for the front-end application.
back-end/
docker-compose.yml: Configuration for the back-end application and MySQL database.
scripts/
setup-vm.sh: Script for setting up virtual machines with Docker and Docker Compose.
setup-mysql.sh: Script for deploying MySQL using Docker.
screenshots/
Configuration and security settings screenshots for Azure (NSGs, Load Balancer, Security Center).
logs/
Performance metrics and cron job output logs.
api-interactions/
Screenshots of API interactions with the MySQL database.
README.md: Documentation for this project.
Project Overview
Docker Compose Files
Front-End
The docker-compose.yml file for the front-end application is located in the docker-compose/front-end/ directory. It defines how the front-end service should be built and run.

Back-End
The docker-compose.yml file for the back-end application and MySQL database is located in the docker-compose/back-end/ directory. It sets up the back-end service, MySQL database, and their configurations.

Setup Scripts
setup-vm.sh: This script automates the installation of Docker and Docker Compose on your virtual machine. Run this script to prepare your VM for deploying containers.

bash
Copy code
chmod +x setup-vm.sh
./setup-vm.sh
setup-mysql.sh: Use this script to deploy a MySQL container with predefined settings.

bash
Copy code
chmod +x setup-mysql.sh
./setup-mysql.sh
Configuration Screenshots
In the screenshots/ directory, you will find screenshots of the following:

Network Security Groups (NSGs) configuration
Load Balancer settings
Azure Security Center configuration
These screenshots demonstrate the configuration and security settings applied to the virtual machines and network.

Logs and Performance Metrics
The logs/ directory contains:

VM resource utilization metrics
Cron job output logs
These logs are essential for monitoring and analyzing the performance of your setup.

API Interactions
In the api-interactions/ directory, you will find screenshots showing interactions between API endpoints and the MySQL database. These screenshots validate the functionality and integration of your application with the database.

How to Use
Clone the Repository:

bash
Copy code
git clone https://github.com/your-username/my-project-setup.git
cd my-project-setup
Set Up Virtual Machines:

Execute the VM setup script to prepare your environment.

bash
Copy code
cd scripts
chmod +x setup-vm.sh
./setup-vm.sh
Deploy MySQL:

Run the MySQL setup script to start the database container.

bash
Copy code
chmod +x setup-mysql.sh
./setup-mysql.sh
Deploy Applications:

Navigate to the respective docker-compose directory and start the services.

For the front-end application:

bash
Copy code
cd docker-compose/front-end
sudo docker-compose up -d
For the back-end application:

bash
Copy code
cd docker-compose/back-end
sudo docker-compose up -d
Review Configuration and Logs:

Check the screenshots/ and logs/ directories for configuration and performance information.

Verify API Endpoints:

Use the api-interactions/ screenshots to test and verify the API functionality.

Conclusion
This repository provides a complete setup for deploying a front-end and back-end application with Docker, configuring MySQL, and ensuring high availability with load balancers. 
