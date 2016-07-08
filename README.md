# Ansible deployment scripts for Mayan-EDMS

Mayan EDMS is a fantastic open source solution for an Electronic Document
Management System. This system can be used to manage enterprise or personal documents.

Read the full feature list here: http://mayan-edms.com/

## Prepare the Ansible deployment

1. Create a virtualenv and install the requirements.
    
    `pip install -r requirements.txt`

2. Rename the `environments/mayan/group_vars/secrets.yml.example` file to `secrets.yml`

3. Replace the values values in the `secrets.yml` file with your values

4. Update the inventory file `environments/mayan/mayan` with your server ip address.

## Run the deployment

- Run the full deployment.

    `ansible-playbook mayan_all.yml -i environments/mayan/mayan --ask-become-pass`
    
