## Networking the Containers

` $ docker run -d --name redis-server redis `

Linking the Redis to alpine:

` $ docker run --link redis-server:redis alpine env `
