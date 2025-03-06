# Ansible Playbook Repository

## Overview
This repository contains Ansible playbooks for managing Docker and Apache installations on Ubuntu servers. These playbooks automate the installation and removal processes, ensuring consistent and efficient deployment.

## Playbooks
### 1. Docker Playbooks
#### Installation (`Ansible-Docker/playbook.yml`)
This playbook installs Docker on an Ubuntu server, including necessary dependencies and configurations.

#### Removal (`Ansible-Docker/remove-docker.yml`)
This playbook removes Docker and its associated components from the server.

### 2. Apache Playbooks
#### Installation (`Ansible-apache/playbook.yml`)
This playbook installs Apache2 on an Ubuntu server and ensures the service is running.

#### Removal (`Ansible-apache/remove-apache2.yml`)
This playbook removes Apache2 from the server.

## Inventory Files
Each playbook folder contains an `inventory.ini` file defining the target servers:
- `Ansible-Docker/inventory.ini` for Docker-related tasks.
- `Ansible-apache/inventory.ini` for Apache-related tasks.

## Usage
### Running the Playbooks
Ensure Ansible is installed on your local machine and execute the playbooks using the following commands:

#### Installing Docker:
```bash
ansible-playbook -i inventory.ini playbook.yml
```

#### Removing Docker:
```bash
ansible-playbook -i inventory.ini remove-docker.yml
```

#### Installing Apache:
```bash
ansible-playbook -i inventory.ini playbook.yml
```

#### Removing Apache:
```bash
ansible-playbook -i inventory.ini remove-apache2.yml
```

## Requirements
- Ansible installed on the control machine.
- Target servers configured with SSH access.
- Correct inventory file entries with valid IP addresses and credentials.

## Author
[Saurabh Dnyaneshwar Mate](https://github.com/saurabh-mate)

