# Personal Ansible playbook

A simple Ansible playbook to set up my personal Fedora Silverblue workstation.

To install Ansible with pip and the necessary collections:

```sh
python -m ensurepip
python -m pip install ansible
ansible-galaxy collection install community.general containers.podman
```

Optional: if you want to make sure only the specified flatpak are installed, then run before the playbook:

```sh
flatpak uninstall --all
```

To use the playbook:

```sh
ansible-playbook -K playbook.yml
```
