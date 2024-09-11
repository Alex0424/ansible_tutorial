# ansible_tutorial

This is my awesome Ansible repository!

ansible all --key-file ~/.ssh/ansible -i inventory -m ping           #make a connection / establish a connection

create inventory and ansible.cnf

ansible all -m ping

ansible all --list-hosts

ansible all -m gather_facts --limit 192.168.56.101



# COMMANDS

ansible all -m apt -a update_cache=true --become --ask-become-pass # same as apt update

ansible all -m apt -a "upgrade=dist" --become --ask-become-pass # same as apt dist-upgrade

ansible all -m apt -a name=cloud-init --become --ask-become-pass # download package

ansible all -m apt -a "name=cloud-init state=latest" --become --ask-become-pass # upgrade package


# TROUBLESHOOT

check commands manually on the vm 

cat /var/log/apt/history
