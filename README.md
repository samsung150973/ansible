# ansible

# INVENTORY : List of Machines managed 
# Default ANSIBLE is 2.9 - Python 2
# "all" is a group to include all entries
# ansible -i inv all --list-hosts

# playbook is a list of plays & always starts with -
# play is a list of tasks
# task is an action to perform

# How to run a playbook

# syntax command  " ansible-playbook -i inventoryFileNme -e ansible_user=username -e ansible_password=password nameOfThePlaybook.yaml

# ansible-playbook -i inv -e ansible_user=centos -e ansible_password=DevOps321 01-playbook.yaml

# set of facts ansible is going to collect
# ansible -i inv all -e ansible_user=centos -e ansible_password=DevOps321 -m setup
# connects to the destination instance and extracts Facts about the instance