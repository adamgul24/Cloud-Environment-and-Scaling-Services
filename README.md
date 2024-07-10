# Cloud Environment Deployment and Scaling Services

## Project Overview
This project involves deploying web services within a cloud environment and scaling them using orchestration tools. The initial deployment focuses on setting up a LAMP server on Amazon AWS and configuring WordPress. The scaling phase utilizes Ansible for automation and orchestration to manage and scale the cloud infrastructure efficiently.

## Table of Contents
- [Project Overview](#project-overview)
- [Lab 1: Deploy Web Services](#lab-1-deploy-web-services)
  - [Objectives](#objectives)
  - [Technologies Used](#technologies-used)
  - [Process](#process)
  - [Results](#results)
- [Lab 2: Scale Cloud Services](#lab-2-scale-cloud-services)
  - [Objectives](#objectives-1)
  - [Technologies Used](#technologies-used-1)
  - [Process](#process-1)
  - [Results](#results-1)
- [Installation](#installation)
- [Usage](#usage)
- [Report](#report)
- [Contributing](#contributing)
- [License](#license)

## Lab 1: Deploy Web Services

### Objectives
- Deploy a LAMP (Linux, Apache, MySQL, PHP) server on Amazon AWS.
- Install and configure WordPress on the server.

### Technologies Used
- **Cloud Platform**: Amazon AWS
- **Operating System**: Ubuntu 18.04
- **Web Server**: Apache
- **Database**: MySQL
- **Programming Language**: PHP
- **Automation Tool**: Ansible

### Process
1. **Setting up AWS Instance**:
   - Created an AWS EC2 instance with Ubuntu 18.04.
   - Configured security groups to allow necessary traffic.
   - Connected to the instance using SSH.

2. **Installing LAMP Stack**:
   - Installed Apache:
     ```bash
     sudo apt update
     sudo apt install apache2
     ```
   - Installed MySQL:
     ```bash
     sudo apt install mysql-server
     ```
   - Installed PHP:
     ```bash
     sudo apt install php libapache2-mod-php php-mysql
     ```

3. **Installing WordPress**:
   - Downloaded and configured WordPress.
   - Set up the database and completed the installation.

### Results
Successfully deployed a LAMP server on AWS and configured WordPress, providing a robust web service environment.

## Lab 2: Scale Cloud Services

### Objectives
- Use automation and orchestration tools to scale web services.
- Configure AWS LAMP instance for Ansible-based configuration management.
- Automate setup and management with Ansible.

### Technologies Used
- **Automation Tool**: Ansible
- **Cloud Platform**: Amazon AWS
- **Operating System**: Ubuntu 18.04

### Process
1. **Connecting to EC2 Instance**:
   - Used AWS Instance Connect to access the EC2 instance.

2. **Generating RSA Key Pair**:
   - Created an RSA key pair for passwordless SSH login.
     ```bash
     ssh-keygen
     cat id_rsa.pub >> authorized_keys
     ```

3. **Installing and Configuring Ansible**:
   - Added Ansible PPA and installed Ansible.
     ```bash
     sudo apt-add-repository ppa:ansible/ansible
     sudo apt-get update
     sudo apt-get install ansible
     ```
   - Created a custom inventory file for Ansible.

4. **Running Ansible Commands**:
   - Installed packages, checked system information, and managed cloud infrastructure using Ansible commands.

### Results
Successfully used Ansible to automate configuration management and scale cloud services, demonstrating the effectiveness of orchestration tools in managing cloud infrastructure.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/adamguled/Cloud-Environment-Deployment-and-Scaling.git
