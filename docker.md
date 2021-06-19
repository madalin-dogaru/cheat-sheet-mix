### Docker Install Options
```curl -sSL https://get.docker.com/ | sh```    (install edge/beta version)    

+ Docker machine install    
```
base=https://github.com/docker/machine/releases/download/v0.16.0 \
  && curl -L $base/docker-machine-$(uname -s)-$(uname -m) >/tmp/docker-machine \
  && sudo mv /tmp/docker-machine /usr/local/bin/docker-machine \
  && chmod +x /usr/local/bin/docker-machine
```

### Basic commands
```
docker run -d -v jenkins_home:/var/jenkins_home -p 8080:8080 -p 50000:50000 jenkins/jenkins:lts-jdk11  
docker ps     
docker rm  container_id     
docker inspect container_id  
``` 
### Default attached volume location
/var/lib/docker/volumes/   


### Example sensitive data access via attached volumes
```
sudo cat /var/lib/docker/volumes/jenkins_home/_data/secrets/master.key      
sudo cat /var/lib/docker/volumes/jenkins_home/_data/secrets/hudson.util.Secret   
```
