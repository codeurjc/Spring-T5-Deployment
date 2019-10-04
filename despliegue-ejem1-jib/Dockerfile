# our base image
FROM maven:3-jdk-8-slim

COPY . /usr/src/app

WORKDIR /usr/src/app

RUN mvn package

# tell the port number the container should expose
EXPOSE 8080

# run the application
CMD ["java", "-jar", "/usr/src/app/target/despliegue_ejem1-0.0.1.jar"]