# Personal ansible

A simple Ansible playbook to setup my personal Fedora Silverblue workstation.

To install Ansible and the necessary collections:

```
python3 -m ensurepip
python3 -m pip install ansible
ansible-galaxy collection install community.general containers.podman
```
