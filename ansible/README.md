# Examples

## Intro

This directory contains 3 examples of Ansible projects that increase in complexity.

1. [playbook_basic](https://github.com/cgillions/examples/tree/master/ansible/playbook_basic)
   This project lists tasks in the playbook file

2. [playbook_role](https://github.com/cgillions/examples/tree/master/ansible/playbook_role)
   This project uses a role to encapsulate the tasks

3. [playbook_role_structure](https://github.com/cgillions/examples/tree/master/ansible/playbook_role_structure)
   This project makes use of the role directory structure for a more advanced deployment

## Ansible

Ansible is the program used in these examples to provision applications on remote servers.

You can install Ansible by following [these instructions](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html).

## Vagrant

Each example can be ran using a local Centos 7 Virtual Machine created with Vagrant. The Vagrantfile is provided in the root directory.

Install Vagrant by following [these instructions](https://www.vagrantup.com/intro/getting-started/install.html).

## Commands

1. Start the VM
   1. Open a POSIX terminal session
   2. Clone the repository with `git clone git@github.com:cgillions/examples.git`
   3. Move to the directory with `cd examples`
   4. Start the virtual machine with `vagrant up`

2. Provision the example website
   1. Move to the project directory with `cd playbook_basic`
   2. Provision the server started above with `ansible-playbook --inventory env/dev playbook.yml`
