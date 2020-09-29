# Ansible-laboratories
This repository contain Ansible labs. 

## Requirements:
 - **Linux system** - You can administrate windows systems with Ansible, but Ansible controller 
   node must be installed on a Linux system (RHEL, CentOS, Debian, FreeBSD, Arch Linux...).
 - **Vagrant** - To managing virtual machines as code. [Vagrant instalation guide](https://www.vagrantup.com/docs/installation)
 - **VirtualBox** - [Virtualbox instalation link](https://www.virtualbox.org/wiki/Linux_Downloads)
 - **Ansible** - Virtual machines will be provisioned by Ansible. [Ansible instalation link](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)

 ## Directory contents
Each directory is a lab. These labs contain a file called *Vagrantfile* and a directory called *Provisioning* 
 - **Vagrantfile**: This file describe the virtual machines settings like VM box (operating system), 
  hardware, network configuration, provider (virtualbox in all cases) or provision method (Ansible).
- **Provisioning**: This directory content Ansible inventories, playbooks and roles.

## Deployment an Ansible lab
To run a specific lab on your local machine, you need clone this repository, **_access to_** 
**_the laboratory directory you want to run_**, and execute **vagrant up** command. This command creates,
configures and provisions the guest system automatically. Other important vagrant commands are:
- vagrant ssh: connects to machine via SSH.
- vagrant status: outputs status of the vagrant machine.
- vagrant provision: provisions the vagrant machine (if you edited any 
  playbook, you can run this command to re-provision the machine).
- vagrant halt: shuts down the running machines.
- vagrant destroy: stops the running machine Vagrant is managing and 
  destroys all resources (**_be carefull!_**).
- vagrant list-commands: outputs all available Vagrant subcommands.
