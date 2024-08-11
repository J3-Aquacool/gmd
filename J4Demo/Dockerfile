FROM maven:3-amazoncorretto-17-al2023 AS build
WORKDIR /javaapps-github
COPY . .
RUN mvn clean package && ls -l /javaapps-github/target
FROM openjdk:17-jdk-alpine
WORKDIR /dockerrepo
COPY --from=build /javaapps-github/target/demopro.jar .
EXPOSE 8383
ENTRYPOINT ["java","-jar","/dockerrepo/demopro.jar"]