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

show docker version
```commandline
docker version
```
all command should run in root mode to go to root mode you can run this command.
```commandline
sudo -i
```
after run this command you should enter root password.

[For more information see docker.com](https://docs.docker.com/engine/install/ubuntu/)
