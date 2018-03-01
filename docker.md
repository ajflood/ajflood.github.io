# Docker Cheat Sheet

Remove all containers
```bash
docker rm $(docker ps -a -q)
```

Remove all images
```docker rmi $(docker images -q)```

Build docker image
```docker build -t someTag .```

Build nvidia-docker image
```nvidia-docker build -t someTag .```

Run Docker image
```docker run someTag```
