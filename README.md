# Automate-Nexus with Ansible

This repository contains Ansible playbooks, roles, and configurations to automate the installation of Nexus, a repository manager, using Ansible.

## About the Playbook

The playbook, `playbook.yaml`, contains the following main sections:

- `name`: This is the name of the play, "Automate Nexus Deployment".
- `hosts`: This specifies the hosts that the play will run on, in this case, AWS EC2 instances.
- `roles`: This specifies the roles that will be applied to the hosts. In this playbook, the "Nexus" role is applied.

## Prerequisites

Before running the Ansible playbooks, ensure that you have the following:

- Ansible installed on your local machine.
- Access to the target host where Nexus will be installed.
- SSH access to the target host with appropriate permissions.


## Getting Started

To get started with the installation, follow these steps:

1. Clone the repository to your local machine:

   ```bash
   git clone https://github.com/ahmedalaa14/Automate-Nexus.git
   ```

2. Navigate to the repository directory:
```
cd Automate-Nexus
```
3. Using Dynamic Inventory to get public hosts in specific region .

4. Run the playbook to install Nexus:
```
ansible-playbook playbook.yml
```
5.Access Nexus by navigating to http://<nexus-host>:8081 in your web browser.
