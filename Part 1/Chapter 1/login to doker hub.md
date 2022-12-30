# Login to docker hub 

```commandline
docker login
```

if get error about docker.sock has no permission 

```commandline
sudo chmod 666 /var/run/docker.sock
```
retry 
```commandline
docker login
```

Verify that the Docker Engine installation is successful by running the hello-world image:
```commandline
sudo docker run hello-world
```
