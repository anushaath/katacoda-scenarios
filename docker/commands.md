// Run commands inside bash

docker run -it ubuntu bash

//HTMLContainer scripts
docker build -t webserver-image:v1 .

docker run -d -p 80:80 webserver-image:v1

