# gs-spring-boot
In this repository, I have used the https://github.com/spring-guides/gs-spring-boot.git repo to dockerize a spring boot application with multi-stage build.

# Build and Push Container

```bash
git clone https://github.com/MohamadEdris/gs-spring-boot.git
cd gs-spring-boot
docker build -t gs-spring-boot .
docker tag gs-spring-boot medris2796/gs-boot:latest
docker push medris2796/gs-boot:latest
```
![gs-boost](https://user-images.githubusercontent.com/73100170/177014284-60c3bbc7-21e8-40f9-aa85-67fae6ac6a56.PNG)

# Run Localy
#### To run the container, you can use the following commands:


```bash
git clone https://github.com/MohamadEdris/gs-spring-boot.git
cd gs-spring-boot
docker build -t gs-spring-boot .
docker run -d -p 8080:8080 gs-spring-boot
```
#### Alternatively, you can pull the image from the Docker Hub and run it:

docker pull medris2796/gs-spring-boot
docker run -d -p 8080:8080 medris2796/gs-spring-boot

