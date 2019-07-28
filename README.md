# setup_docker_on_centos7
A sample ansible playbook to setup VirtualBox, docker, docker-machine, docker-compose on a Centos 7 env

Steps to run the playbook:
1. add your env hostname into the /etc/ansible/hosts file:
ex.

[Home]

myhostname ansible_user=<ansible_user_name>


2. replace "var_docker_user: jonathan" line in the pb_setup_docker.yaml file to your docker user name

3. run command:
ansible-playbook --ask-pass --ask-become-pass pb_setup_docker.yaml


reference:

https://www.virtualbox.org/wiki/Linux_Downloads

https://docs.docker.com/install/linux/docker-ce/centos/

https://docs.docker.com/machine/install-machine/

https://docs.docker.com/compose/install/

https://gist.github.com/yonglai/d4617d6914d5f4eb22e4e5a15c0e9a03


