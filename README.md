# docker-commands-


| Command | Description |
| ------- | ----------- |
|sudo docker images | see images in locallly
|sudo docker container ls  |ee running container
|sudo docker ps  |see running process
|sudo docker container -a | see all stopped containers
|sudo docker image pull hamza6552/portfolio | pull image from dockerhub
|sudo docker run --name nginx -p 8080:80 -d -t nginx:latest | build and run image in container
|sudo docker exec -it nginx:latest sh | goto running container
|sudo docker start nginx | start stopped conatiner
|sudo docker images prune --all --force  |force fully remove all images
|sudo docker container prune | delete all stopped container
|sudo docker run -t nginx:latest | -t tag used for which image version/tag we use.
|sudo docker run --name nginx -t -d -p 8080:80 | --name use for put conatiner name . -d tag used for running in background. -p tag used for put port in container systemPort:ContainerPort
|sudo docker build -t myapplication:latest | this command used for build our appliaction all file in image
|sudo docker run --name nginx -p 8080:80 -d -v /home/application:/apps/usr/nginx/html -t nginx:alpine | -v tag used for mounting folder and files  


### docker used for our application are containerized.

## Dockerfile



| Command | Description |
| ------- | ----------- |
| FROM | nginx:latest
| WORKDIR | /usr/share/nginx/html
| COPY | . .
| EXPOSE | 80
| CMD | ["echo","Hello Hamza"]







