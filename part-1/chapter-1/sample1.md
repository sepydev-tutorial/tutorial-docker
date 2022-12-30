# Create Simple doker file 

- Create a js file 
- Add bellow code to the file 
```js
console.log('Hello docker')
```
- Next we want to create new docker file. name of file should be 'Dockerfile' with this content
```dockerfile
FROM node:alpine 
# Choose the base image we want to use,
# and select which distro, that image is based on
# alpine is a lightweight distro
COPY . /app
# copy all files in directory in to that image 
WORKDIR /app
# Change working directory to the new folder.
# All command after this like run in app directory
CMD node app.js
# run app
```

- Package application with this command
```commandline
docker build -t hello-docker .
```
Full command is 
```commandline
docker build -t <hub-user>/<repo-name>[:<tag>]
```
To set a tag on the docker image use `-t` tag-name <br>
Then you should set which directory has a docker file, so we set `.` as the root

- To see all images on this computer use this command
```commandline
docker images
```
or 
```commandline
docker image ls
```

- To run image 
```commandline
docker run hello-docker
```


- To push image to docker hub use this command after create repository in hub.docker
```commandline
docker push <hub-user>/<repo-name>:<tag>
```


- To pull image use this command
```commandline
docker pull mrprocs/hello-docker
```