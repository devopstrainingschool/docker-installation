# docker-installation
#On centos 7
## Uninstall old versions
```
sudo yum remove docker \
                  docker-client \
                  docker-client-latest \
                  docker-common \
                  docker-latest \
                  docker-latest-logrotate \
                  docker-logrotate \
                  docker-engine
                  
  ```
## Setup the repository
```
sudo yum install -y yum-utils
```
```
sudo yum-config-manager \
    --add-repo \
    https://download.docker.com/linux/centos/docker-ce.repo

```
## Install docker engine
```
sudo yum install docker-ce docker-ce-cli containerd.io docker-compose-plugin -y
```
## Start and enable docker
```
sudo systemctl start docker
```
```
sudo systemctl enable docker
```
## check if docker is running
```
sudo systemctl status docker
```



![image](https://user-images.githubusercontent.com/107158398/177837463-62620ce4-e786-4b47-8447-236f99d8a0bd.png)
