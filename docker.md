# Docker Cheat Sheet

## Build/Run commands

Build docker image:  
`docker build -t someTag .`

Run Docker image:  
`docker run someTag`

Build nvidia-docker image:  
`nvidia-docker build -t someTag .`

Run Docker image and map volume:  
`docker run -v /localVolme:/dockerVolume thetag`

--Note: Can use $PWD for current directory on host

## Other commands 

Enter a containers terminal: `docker exec -it <mycontainer> bash`


## Clean up commands

List all containers:  
`docker ps -a`

List all images:  
`docker images`

Remove all unattached volumes:  
`docker volume prune`

Remove container:  
`docker rm containerName`

Remove image:  
`docker rmi imageName`

THIS WILL DELETE EVERYTHING:
```
docker system prune -a
docker rm $(docker ps -a)
docker rmi $(docker images -a -q)
```








