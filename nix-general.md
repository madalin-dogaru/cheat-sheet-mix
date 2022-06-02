Change Ubuntu Hostname
---
`hostnamectl set-hostname new-hostname`   

Update linux hostnames
---
`sudo nano /etc/hosts`

Upload the local file test.apk to a remote host via SCP
---
`scp test.apk will@10.129.102.174:/home/will`


Setup a network bridge
---
Show existing bridges   
`brctl show`   
Delete bridge   
`brctl delbr bridgeName`   
Create bridge   
`brctl addbr bridgeName`    
Add interfaces to bridge    
`brctl addif bridgeName eth0 eth1`


