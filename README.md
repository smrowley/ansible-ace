# Ansible ACE Seed Project

Use this seed project to start writing your playbooks.

## Goal

Your playbook should do the following:

- Installs Apache (package: httpd)
- Starts Apache (service: httpd)
- Opens the port in the firewall
- Adds an index.html to `/var/www/html/`

You'll know it works if you can go to `ace-<fruit>.guy.sh`.

BONUS:

Make your playbook idempotent. An easy way to check if your playbook is idempotent is to run it again and make sure there are no changes (`changed: 0`).

## Setup

1. Install Ansible
    - On RHEL/Fedora/CentOS, run `sudo yum install ansible`
    - On MacOS, use Homebrew
    
2. After cloning this project, you'll need to set the permissions on the private key file (id_rsa).
    - Run `chmod 600 id_rsa`
    
3. Test Ansible can connect to your remote machine (after you populate your `hosts` file.
    - Run `ansible all -m ping` (you should get a successful "pong").
    - You should get prompted for a SUDO password AND a passphrase for the key (this will be provided in person).
