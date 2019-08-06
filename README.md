# Automationclass with Ansible
## Automate Linux, Windows and Cloud

### Prerequsits
Environment

6 servers - made available in Azure - (use 01_class_setup.yml to deploy in Azure)

4 - Running Red Hat Enterprise Linux 8
Accessible with ssh and http/https
* ansible - 10.1.0.4
* tower   - 10.1.0.5
* server1 - 10.1.0.6
* server2 - 10.1.0.7

2 - Running Windows Server 2019 with GUI
Accessible with winRM and RDP
* server3 - 10.1.0.8
* server4 - 10.1.0.9

Software on your client
* VSCode (or other IDE)
* Git
* ssh client
* RDP client
* Webbrowser

# Tasks

## Task 1: Install Ansible

Log on to server "ansible" using ssh 

Type:

sudo dnf install -y python3-pip

![Alt text](pics/001_install_pip3.png?raw=true "Install Python3 PIP3")

sudo pip3 install --upgrade pip

![Alt text](pics/002_install_pip3_upgrade.png?raw=true "Upgrade PIP")

Note: Sudo Password is equal to your user account password

pip3 install ansible --user

![Alt text](pics/003_install_ansible.png?raw=true "Install Ansible")

## Task 2: Run ansible command

Log on to server "ansible" using ssh 

Type:

ansible --version

![Alt text](pics/004_install_ansible_version.png?raw=true "Ansible --version")

ansible --help