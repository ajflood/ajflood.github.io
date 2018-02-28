# Docker Cheat Sheet

Remove all containers
```docker docker rm $(docker ps -a -q)```

Remove all images
```docker docker rmi $(docker images -q)```

Build docker image
```docker docker build -t someTag .```

Build nvidia-docker image
```docker nvidia-docker build -t someTag .```

Run Docker image
```docker docker run someTag```
