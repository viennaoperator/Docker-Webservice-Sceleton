# Webservice 2.0
## Needed
 - Java 8
 - Maven
 - Docker

If you are using Windows 7 Install "Docker Toolbox on Windows"
https://docs.docker.com/toolbox/toolbox_install_windows/

## Start Application
```sh
mvn package
java -jar target/webservice-0.0.1.jar
```

## Build Docker Container
```sh
mvn install dockerfile:build
```
if you are facing problems under windows 7 use the "containerbuild.bat" file. 

## Start Docker Container
```sh
docker run my/webservice2 -p 11111:11111
```
command could vary due to your port settings. {HOST_PORT}:{APPLICATION_PORT}

## Docker REST-API Documentation
http://localhost:11111/swagger-ui.html#/

## Useful Links
- https://spring.io/guides/gs/spring-boot-docker/
- https://docs.docker.com/toolbox/toolbox_install_windows/