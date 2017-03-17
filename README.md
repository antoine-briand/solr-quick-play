# SOLR Quickstart

This repository intend to give quickstart scripts for messing around with solr.

YOU SHOULD NOT USE ANY OF THE PROVIDED SCRIPTS TO DEPLOY SOLR IN A PRODUCTION ENVIRONMENT.

## Run SOLR in a docker container
You have a docker environment up and running. Just clone this repository and run

```sh
docker-compose up -d
```

## Run SOLR on a brand new Ubuntu server
You'll find a deadly simple ansible playbook that install docker, pull the solr image, and run it.
You should have ansible installed. If not follow the guidelines : [Install Ansible](http://docs.ansible.com/ansible/intro_installation.html)



Once it's installed clone this repository and run :
```sh
ansible-playbook -i {YOUR.SERVER.IP.ADRESS}, deploy-solr-docker.yml
```

Replace {YOUR.SERVER.IP.ADRESS} with the ip of your fresh Ubuntu 16.04 server

## Deploy SOLR using Vagrant
If you want to deploy Solr in a local virtual machine, you can use vagrant.
It's easy to install and use.
Follow the instructions to get started : (Vagrant Download)[https://www.vagrantup.com/downloads.html]
Once Vagrant is installed, clone this repository and run :

```sh
vagrant up
```

Finally browse http://localhost:8983 (replace localhost by a domain name or the IP of a server)
