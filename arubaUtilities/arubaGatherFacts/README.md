Aruba Fact Gathering
=============================

This Play can be used to gather facts used in Aruba Configuration Templates 

___

## How to use
Run the playbook with an inventory pointing to aruba controllers. Vars will be output in host_vars in a file named for the host.


#### Run the playbook via ansible-playbook command

###### Example: 
```
ansible-playbook --ask-vault-pass arubaGather.yaml

```

Host_vars will be generated. 

### This playbook has been designed to use an ansible-vault

```
mkdir group_vars
mkdir group_vars/all
ansible-vault create group_vars/all/vault.yaml
```

###### Example:
```
---
aruba_ssh_user: <user>
aruba_ssh_pass: <password>
```