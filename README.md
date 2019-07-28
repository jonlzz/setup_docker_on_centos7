# setup_docker_on_centos7
Ansible playbook to setup docker, docker-machine, docker-compose on an Centos 7 env

Steps to run the playbook:
1. add your env hostname into the /etc/ansible/hosts file:
ex.

[Home]

myhostname ansible_user=<ansible_user_name>


2. replace "var_docker_user: jonathan" line in the pb_setup_docker.yaml file to your docker user name
3. run command:
ansible-playbook --ask-pass --ask-become-pass pb_setup_docker.yaml


