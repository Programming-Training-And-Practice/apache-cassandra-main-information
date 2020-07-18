# Apache Cassandra Main Information.





## Contents at a Glance.
* [About](#about)
* [Documentation.](#documentation)
* [Pros.](#pros)
* [Cons.](#cons)
* [Run in Docker.](#run-in-docker)
* [Help](#help)





## About.





## Documentation.





## Pros.
* High availability.
* Partition tolerance and scaling.
* Amount of available resources.





## Cons.
* Connecting new nodes is not simple.
* We must know what query will be previously executed.





## Run in Docker.
`docker pull datastax/dse-server:latest`
`docker pull datastax/dse-studio:latest`
`docker run -p 9042:9042 -e DS_LICENSE=accept -memory 4g --name my-dse-server -d datastax/dse-server -g -s -k`
`docker run -p 9091:90p1 -e DS_LICENSE=accept -memory 1g --name my-dse-studio -d datastax/dse-studio --link my-dse-server`

`docker stop my-dse-studio`
`docker stop my-dse-server`

`docker start my-dse-studio`
`docker start my-dse-server`





## Help.
