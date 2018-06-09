# Get started with Docker
https://docs.docker.com/get-started

## Build the app

```
# Create a Docker image
# run from the app's top level directory:
$ docker build -t friendlyhello .

# See image in your local Docker image registry:
$ docker image ls
```

## Run the app
```
$ docker run -p 4000:80 friendlyhello

# Go to URL http://localhost:4000
```

**Note:** If you are using Docker Toolbox on Windows 7, use the Docker Machine IP instead of localhost.
For example, http://192.168.99.100:4000/.
To find the IP address, use the command `docker-machine ip`.


### Run the app in the background
```
# To run the app in detached mode:
$ docker run -d -p 4000:80 friendlyhello

# You can see the abbreviated container ID with
$ docker container ls
```

## End the process:
```
$ docker container stop ${CONTAINER ID}
```
