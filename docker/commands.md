## // Some useful Docker commands

docker run -it ubuntu bash   // To run commands inside bash

echo <file-name> >> .dockerignore     // useful to ignore large files in docker build

## //HTMLContainer scripts

docker build -t webserver-image:v1 .

add to docker build "--no-cache=true" to disable cache

docker run -d -p 80:80 webserver-image:v1

curl -i http://docker

## // NODEContainer

docker build -t my-nodejs-app .

docker run -d --name my-running-app -e NODE_ENV=production -p 3000:3000 my-nodejs-app

curl http://docker:3000

## //Build container- Dockerfile commands

FROM <container_name>

COPY <src> <dest>

RUN <command>

EXPORT <port> <port>

CMD ["","",""]

or use ENTRYPOINT

ONBUILD RUN ....   // Can be used when it should run as a base image
