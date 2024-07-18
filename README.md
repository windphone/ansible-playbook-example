# Ansible Playbook Example

This repository contains an example of an Ansible Playbook for installing and configuring Nginx on a local machine.

## Files

- `hosts`: Ansible inventory file with local connection configuration.
- `site.yml`: Ansible Playbook to install and configure Nginx.

## Usage

To run the playbook, use the following command:

```sh
ansible-playbook -i hosts site.yml

