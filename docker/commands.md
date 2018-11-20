// Run commands inside bash

docker run -it ubuntu bash

//HTMLContainer scripts

docker build -t webserver-image:v1 .

add to docker build "--no-cache=true" to disable cache

docker run -d -p 80:80 webserver-image:v1

curl -i http://docker

//Build container

FROM <container_name>

COPY <src> <dest>

RUN <command>

EXPORT <port> <port>

CMD ["","",""]

or use ENTRYPOINT
