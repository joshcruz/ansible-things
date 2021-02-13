# ansible-wordpress

This Ansible playbook updates an already existing WordPress to the latest version. Your database and WordPross root folder are backed up before the update.

## Configure files

Before running the playbook, change the IP address of `server1` in the `hosts` file to match the IP of your virtual machine.

## Run the Ansible playbook

```
ansible-playbook site.yml -i hosts --ask-pass --ask-become-pass
```