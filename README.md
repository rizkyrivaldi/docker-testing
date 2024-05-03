# docker-testing
testing docker

## Install Docker Debian
```
cd ~/Downloads
curl -fsSL https://get.docker.com -o get-docker.sh
sh ./get-docker.sh
```

## Choose the docker app directory
```
cd [Directory]
```

## Build the image
```
docker build -t [image name]:[version] .
```

## Check built image
```
docker images
```

## Run the container based on image
```
# Run in the background, detached
docker run -dp [forwarded port]:[container port] [image name]:[version]

# Run in the terminal without detach
docker run -p [forwarded port]:[container port] [image name]:[version]
```

## Check the detached container
```
docker ps
```

## Stop detached container
```
docker stop [container ID]
```

