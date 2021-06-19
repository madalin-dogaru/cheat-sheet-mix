### ED25519 Key Generation
ssh-keygen -o -a 100 -t ed25519 -f ~/.ssh/id_ed25519 -C "thewallachian@wallachia.com"

### Add the SSH password to the ssh-agent
eval `ssh-agent`   
ssh-add /home/user/.ssh/id_rsa

### Copy SSH Key to remote Host
ssh-copy-id -i ~/.ssh/id_ed25519.pub user@192.170.1.70   

###

