# Academy2023 Python API dockerize

### Build application
Build the Docker image manually by cloning the Git repo.
```
$ git clone https://github.com/canogluonur/FBI-Flask-API-Docker.git
$ docker build -t akademi2023 .
```
Note: akademi2023 can be replaced with any name.
```
### Run the container
Create a container from the image.
```
```
$ docker run -d -p 5000:5000 akademi2023 
```

Now visit http://localhost:5000

And you can check the container status

```
$ docker ps -a 
```


Also you can run from Docker Hub;
```
$ docker pull onurcanoglu/akademi2023:latest
```
```
$ docker container run -p 5000:5000 onurcanoglu/akademi2023:latest
```
