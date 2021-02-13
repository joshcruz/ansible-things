# ansible-initial-setup

This playbook runs a configuration setup for a new server, so you won't need to. Doing this removes the tideous tasks of manually installing packages, managing user/groups/folders/files, enabling/disabling ports, etc.

It will perform the following tasks:
- Update the system packages
- Install defined packages
- Copy over your ssh key

Note: We will be expanding this example to include other linux distributions.

## Configure files

Before running the playbook, change the IP address of `centos` in the `hosts` file to match the IP of your virtual machine.

## Run the Ansible playbook

```
ansible-playbook site.yml -i hosts --ask-pass --ask-become-pass
```