# Ansilbe-Code-GCP
Fist step 

Download Ansible on your compute. 
Access the https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html
choose your operating system 

Second step

Access your project or create the project. go to IAM & Admin and go to service account choose your project in actions create key and download key in format .json or .pem, indicate path for example
---
- name: Create an instance
  hosts: localhost
  gather_facts: no
  vars:
      gcp_project: # input project id the google cloud platform 
      gcp_cred_kind: serviceaccount
      gcp_cred_file: # add /home/credentials/gcp/credential.json
      zone: "us-central1-a"
      region: "us-central1"