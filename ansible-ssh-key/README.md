# ansible-ssh-key

This is a simple Ansible project for copying over your ssh-key to a server. Doing this we can easily ssh into the desired machine without inputting a password.

## Configure files

Before running the playbook, change the IP address of `server1` in the `hosts` file to match the IP of your virtual machine.

## Run the Ansible playbook

```
ansible-playbook site.yml -i hosts --ask-pass -ask-become-pass
```