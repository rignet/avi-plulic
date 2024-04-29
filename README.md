# Provisioning the server

This repository contains scripts to automate and speed up the Protectli PP workflow and preparation

> **_Disclaimer_**:
> These scripts are related to Ubuntu with major version 18+, for other distributions you will need to adapt them
___
1. Install Ansible.
```bash
sudo apt update && sudo apt install ansible git -y
```
2. Clone this repository.
```bash
git clone https://github.com/rignet/avi-plulic.git
```
3. Change directory
```
cd avi-public
```
4. Apply the configuration.
```
ansible-playbook provisioning.yaml --ask-become-pass
```
>Enter your password when asked to grant root permissions for some actions.
5. During installation, you will be asked for the server number to complete the hostname starting with `propetro-intelie-` and then continue adding the sequential numbers.
