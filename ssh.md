### ED25519 Key Generation
ssh-keygen -o -a 100 -t ed25519 -f ~/.ssh/id_ed25519 -C "thewallachian@wallachia.com"

### Add the SSH password to the ssh-agent
eval `ssh-agent`   
ssh-add /home/user/.ssh/id_rsa

## #
