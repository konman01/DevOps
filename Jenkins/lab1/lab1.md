# Lab1 - Create Jenkins Docker Container

## Using Dockerfile

### create the Dockerfile with file name Dockerfile and paste the below commands
```
FROM jenkins/jenkins:lts
EXPOSE 5000
```

### Start the Docker

```
# First create a image

docker build -t konman01/jenkins -f Dockerfile.dev build .

# Start the container
docker run -p 8080:8080 konman01/jenkins

```

## Using the Docker Compose

### create docker volume
```
	docker volume create jenkins_home
```

### Create Docker Compose file with filename docker-compose.yml and paste the following command

```
version: '3'
services:
  jenkins:
    build: 
      dockerfile: Dockerfile
    expose:
      - 5000
    ports:
      - "8080:8080"
      - "5001:5000"
    volumes:
      - jenkins_home:/var/jenkins_home
    restart: on-failure
volumes:
  jenkins_home:
```

### start the docker compose 

```
docker compose up
```

### stop the container

```
docker compose down
```

### Access the Jenkins in Port 8080
```
http://localhost:8080/
```
