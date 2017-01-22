# A basic Flask App

## Build image
```
docker build -t hello-app .
```

## Run container background
```
docker run -d -p 5000:5000 --name hello-server hello-app
```

## Browse over the address
```
http://localhost:5000/
```

## Dockers containers not running
```
docker ps
```

## Dockers containers running
```
docker ps -a
```

## Stop the server
```
docker start hello-server
```

## Restart the server
```
docker start hello-server
```

## Enter to command in the docker
```
docker exec -it hello-server bash
```

## Remove containers
```bash
docker stop <containerid>
docker rm <containerid>
```

## Remove all containers
```bash
docker stop $(docker ps -a -q)
docker rm $(docker ps -a -q)
```

## Remove image
```
docker rmi hello-app
```
