# Choice of base Image
I choose to use Official Node.js image for backend as base image because application is built on node.

## Dockerfile directives used in the creation and running of each container 
 I used the following directives for both backend and client:
 1. FROM: to specify the abse image to use
 2. WORKDIR: to set the working directory for the container
 3. COPY: to copy application files from the host machine to the container
 4. RUN: to install the required depedencies for the application
 5. CMD: the command to run the container when it starts


## Docker compose Networking 
 I allocated ports to each service and i used bridge network to connect the services.
 i used 5000 for backend service and 300 foe the client service

## Docker-Compose volumes definition and usage 
 I defined a volume for backend service to store the data in the Mongo Db database to persist the data even when container is restarted.

## Git workflow used to achieve the tasks
 1. cloned the original repository to my local machine.
 2. Created an online github repository on my account.
 3. Added/ set remote origin to pint to my repository url.
 4. made changes to the applicateion.
 5. Added the changes to staging area.
 6. committed the changes.
 7. Pushed the changes to my online repository.

 ### Successfully running of the application
 I tested the application by running command: sudo docker-compose up:
 this command built images, started the containers and attached them to bridge network.
 I accessed the application via http://localhost:3000