# ansible-docker

This project example installs docker on a CentOS server. As of CentOS 8, Red Hat has decided not to provide support for docker. So by default CentOS has 
[`podman`](https://podman.io/) installed.

## Configure files

Before running the playbook, change the IP address of `server1` in the `hosts` file to match the IP of your virtual machine.

## Run the Ansible playbook

```
ansible-playbook site.yml -i hosts --ask-pass --ask-become-pass
```