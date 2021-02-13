# ansible-nginx

This project example installs nginx as a web server and copies a local hello world html file to the nginx html folder. We then set a firewall rule to permanently enable ports 80(http) and 443(https).

## Configure files

Before running the playbook, change the IP address of `server1` in the `hosts` file to match the IP of your virtual machine.

## Run the Ansible playbook

```
ansible-playbook site.yml -i hosts --ask-pass --ask-become-pass
```