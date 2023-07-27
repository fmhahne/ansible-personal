# Personal ansible

A simple Ansible playbook to set up my personal Fedora Silverblue workstation.

To install Ansible (using pipx) and the necessary collections:

```sh
pipx install --include-deps ansible
ansible-galaxy collection install community.general containers.podman
```

To use the playbook:

```sh
ansible-playbook -K playbook.yml -l $(hostname)
```

If you want to make sure only the specified flatpak are installed, then run before the playbook:

```sh
flatpak uninstall --all
```
