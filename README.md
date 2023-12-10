# Automated Web Application Deployment with Ansible

This project automates the deployment and configuration of a multi-tier web application environment using Ansible. It includes the setup of a load balancer, multiple web servers, and a database server.

## Project Components

- **Load Balancer**: Configures Nginx as a load balancer to distribute traffic to web servers.
- **Web Servers**: Hosts a sample web application, demonstrating scalable web server configuration.
- **Database Server**: Sets up and configures a PostgreSQL database.

## Prerequisites

- Ansible 2.9 or higher.
- SSH access to all servers listed in the inventory.
- Servers running a Linux distribution (preferably Ubuntu or CentOS).
- Basic knowledge of Ansible playbooks, roles, and inventory.

## Setup

1. Clone this repository to your Ansible control machine.
2. Update the `inventory/hosts.yml` file with the IP addresses or hostnames of your servers.
3. Configure any specific variables in `group_vars/` as per your requirement.

## Running the Playbooks

Execute the main playbook using the following command:

```bash
ansible-playbook -i inventory/hosts.yml site.yml
```
This command will start the configuration of the entire environment as per the defined roles and tasks.

## Customization

Modify the playbooks and roles to fit your specific environment needs.
Add additional roles or tasks as required for your deployment.

## Contributing

Contributions to this project are welcome! Please fork the repository and submit a pull request with your improvements.
License

This project is licensed under the MIT License - see the LICENSE.md file for details.
Author

Oscar Tejada