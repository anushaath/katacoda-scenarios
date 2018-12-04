## Data Containers

Data Containers are containers whose sole responsibility is to be a place to store/manage data.

`   docker create -v /config --name dataContainer busybox `

` docker cp config.conf dataContainer:/config/ `

` docker run --volumes-from dataContainer ubuntu ls /config `

### Export and Import a Data Container 

` docker export dataContainer > dataContainer.tar `


` docker import dataContainer.tar `
