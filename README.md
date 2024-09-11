# ansible_tutorial

This is my awesome Ansible repository!

ansible all --key-file ~/.ssh/ansible -i inventory -m ping           #make a connection / establish a connection

create inventory and ansible.cnf

ansible all -m ping

ansible all --list-hosts

ansible all -m gather_facts --limit 192.168.56.101


