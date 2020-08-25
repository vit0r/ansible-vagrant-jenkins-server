# How to use

## Vagrant up VM

```bash

vagrant up

```

## Include hosts on ansible hosts file - master ansible or local machine

```bash

vim /etc/ansible/hosts

[jenkinsservers]
192.168.100.13

[jenkinsservers:vars]
ansible_ssh_private_key_file=/home/vit0r/Projects/ansible-jenkins-server/.vagrant/machines/default/virtualbox/private_key

```

## Check and run playbook

```bash

ansible-playbook jenkins.yaml -C

ansible-playbook jenkins.yaml -v

```
