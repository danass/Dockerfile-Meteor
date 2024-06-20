# docker-meteor

After struggling with Docker containerisation of a Meteor installation, I finally succeded and here is my working [Dockerfile](https://github.com/danass/docker-meteor/blob/main/Dockerfile), using **node 14** and **fresh meteor installation** command `curl https://install.meteor.com/ | sh`.

Go in *your_app* folder and place the Dockerfile in it and run following commands:

`docker build -t myapp .`

`docker run -p 3000:3000 myapp`

Mongo tools will be installed inside your docker, so you can enter the docker container and `run meteor mongo -U` to check your current mongo connection, and restore a previous database if needed, using **mongorestore**. 

This [Dockerfile](https://github.com/danass/docker-meteor/blob/main/Dockerfile) is **working** as of **20/06/2024.**


