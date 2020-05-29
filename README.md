# Dockerize Node Application

## Installing Docker 

Use the  [Link](https://stackoverflow.com/questions/30379381/docker-command-not-found-even-though-installed-with-apt-get) to install docker.

## Node and DockerFile

Refer this [Link](https://nodejs.org/fr/docs/guides/nodejs-docker-webapp/) to create node application and write Dockerfile.


```bash
 docker build -t node-app .
 docker images                        //image will be created
 docker run -p 49160:8080 -d node-app
 docker ps                            //container will be created
```

## Installing Jenkins 

Use the  [Link](https://vexxhost.com/resources/tutorials/how-to-install-configure-and-use-jenkins-on-ubuntu-14-04/) to install jenkins.

Command to start, stop and check status jenkins
```bash
 sudo service jenkins status
 sudo service jenkins restart
 sudo service jenkins stop
```


