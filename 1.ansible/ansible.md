### Install Ansible    
sudo apt update       
sudo apt install ansible      

### Setup Hosts Inventory File   
sudo nano /etc/ansible/hosts   
```
[EXAMPLE]    
[all-hosts]    
jenkins ansible_host=192.168.1.74    
wireguard ansible_host=192.168.1.71     

[jenkins-host]     
jenkins ansible_host=192.168.1.74    

[all:vars]
ansible_python_interpreter=/usr/bin/python3
ansible_user=username
ansible_ssh_private_key_file=/home/template/.ssh/id_ed25519
```

### Create a role
sudo ansible-galaxy init role-name    



