FROM maven:3-amazoncorretto-17-al2023 AS build
COPY . .
FROM openjdk:17-jdk-alpine
WORKDIR /dockerrepo
COPY /target/demopro.jar .
EXPOSE 8383
ENTRYPOINT ["java","-jar","/dockerrepo/demopro.jar"]