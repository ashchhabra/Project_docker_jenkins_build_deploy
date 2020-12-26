# Docker-Jenkins Inegration
This is my first personal project ! 

Just trying my hands on docker.

# About Project

Creating Jenkins as a docker container, and using Jenkins pipeline to create docker image(Jar), build it and deploy it on Docker Swarm

# Initial Installations to start off!! 

- Install ubuntu(Virtual Machine) on Oracle VirtualBox

   I 'll update the links soon :)

- Docker Installation https://docs.docker.com/engine/install/ubuntu/

# Create Jenkins Container from Jenkins Image

1) Sudo docker run -p 8070:8080 -p 50000:50000 --name jenkins1 --mount source=jenkins_home1,target=/var/jenkins_home jenkins/jenkins:lts

About this command: 

8070- to access jenkins from browser
8080- port open for tomcat, since jenkins is hosted on apache tomcat
50000- port for master slave in case I create slaves in future

To resume container: docker restart 
Logs: docker logs container-id
Inspect: docker inspect container-id
