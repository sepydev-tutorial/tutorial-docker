# Uninstall old versions
```commandline
sudo apt-get remove docker docker-engine docker.io containerd runc
```

# Install docker engine 

```commandline
sudo apt-get update
```
if receiving a GPG error when running. try to grant read permission

```commandline
sudo chmod a+r /etc/apt/keyrings/docker.gpg
sudo apt-get update
```

install latest version
```commandline
sudo apt-get install docker-ce docker-ce-cli containerd.io docker-compose-plugin
```

Verify that the Docker Engine installation is successful by running the hello-world image:
```commandline
sudo docker run hello-world
```

[For more information see docker.com](https://docs.docker.com/engine/install/ubuntu/)