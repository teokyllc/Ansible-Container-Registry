# Ansible-Container-Registry
An Ansible playbook to create a private Docker container registry.<br>


Copy your SSH key to the target host prior to running playbook.<br>
```
ssh-keygen
ssh-copy-id 192.168.1.6
```
<br>

This playbook has dependency on the community.docker Ansible module.
```
ansible-galaxy collection install community.docker


ansible-playbook -K -i inventory main.yml
```