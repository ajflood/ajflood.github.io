# Docker Cheat Sheet

## Build/Run commands

Build docker image: `docker build -t someTag .`

Run Docker image: `docker run someTag`

Build nvidia-docker image: `nvidia-docker build -t someTag .`

Run Docker image and map volume: `docker run -v /localVolme:/dockerVolume thetag`

--Note: Can use $PWD for current directory on host


## Clean up commands

Remove all containers: `docker rm $(docker ps -a -q)`

Remove all unattached volumes: `docker volume prune`

Remove all images: `docker rmi $(docker images -q)`










