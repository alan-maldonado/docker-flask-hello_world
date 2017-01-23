# A basic Flask App

## Build image
```bash
docker build -t hello-app .
```

## Run container background
```bash
docker run -d -p 5000:5000 --name hello-server hello-app
```

## Browse over the address
```
http://localhost:5000/
```

## Dockers containers not running
```bash
docker ps
```

## Dockers containers running
```bash
docker ps -a
```

## Stop the server
```bash
docker start hello-server
```

## Restart the server
```bash
docker start hello-server
```

## Enter to command in the docker
```bash
docker exec -it hello-server bash
```

## Remove containers
```bash
docker stop hello-server
docker rm hello-server
```

## Remove all containers
```bash
docker stop $(docker ps -a -q)
docker rm $(docker ps -a -q)
```

## Display images
```bash
docker images
```

## Remove image
```bash
docker rmi hello-app
```

# Using host folder in container
```
docker run -d -p 80:80 -v /opt/docker-flask-hello_world:/opt/hello-app --name hello-server hello-app
```
