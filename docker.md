# Docker Cheat Sheet

Remove all containers: `docker rm $(docker ps -a -q)`

Remove all images: `docker rmi $(docker images -q)`

Build docker image: `docker build -t someTag .`

Build nvidia-docker image: `nvidia-docker build -t someTag .`

Run Docker image: `docker run someTag`

Run Docker image and map volume: `docker run -v /localVolme:/dockerVolume thetag`
--Note: Can use $PWD for current directory on host
