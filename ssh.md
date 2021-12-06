### ED25519 Key Generation
```
ssh-keygen -o -a 100 -t ed25519 -f ~/.ssh/id_ed25519 -C "thewallachian@wallachia.com"
```

### Add the SSH password to the ssh-agent
```
ssh-add -K ~/.ssh/id_ed25519
```
### Copy SSH Key to remote Host
```
ssh-copy-id -i ~/.ssh/id_ed25519.pub host-user@host-ip   
```

###   

