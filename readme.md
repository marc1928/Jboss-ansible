![JBoss Domain Mode Management](https://via.placeholder.com/800x400.png "Ansible Playbook for JBoss Domain Mode Management")

# Ansible Playbook for JBoss Domain Mode (WildFly 24) Management

This repository contains an Ansible playbook designed to automate the management of JBoss servers in **domain mode** (WildFly 24). The playbook performs the following tasks:

## Features

1. **Create a Server Group**  
    Define and create a new server group for managing JBoss servers in domain mode.

2. **Add a Server to the Server Group**  
    Provision and add a server to the previously created server group.

3. **Start the Server**  
    Ensure the server is started and operational within the domain.

4. **Deploy a `.war` File**  
    Deploy a specified `.war` file to the server group in the domain.

5. **Modify JVM Parameters**  
    Update the default JVM parameters for the host controller or server group as required.

6. **Conditional Server Restart**  
    Restart the server only if the JVM parameters have been modified.

## Prerequisites

- Ansible installed on your local machine.
- Access to the target JBoss environment in domain mode.
- Properly configured inventory file with the necessary host details.

## Usage

1. Clone this repository:
    ```bash
    git clone https://github.com/marc1928/Jboss-ansible.git
    cd jboss-ansible
    ```

2. Update the inventory file with your server details.

3. Run the playbook:
    ```bash
    ansible-playbook -i inventory playbook.yml
    ```

## Notes

- Ensure you have the required permissions to manage the JBoss environment in domain mode.
- Test the playbook in a staging environment before deploying to production.


