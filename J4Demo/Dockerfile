FROM maven:3.9.8-amazoncorretto-17-al202 AS build
COPY . .
RUN mvn clean package
FROM openjdk:23-ea-17-slim
WORKDIR /dockerrepo
COPY --from=build /javaapps-github/target/demopro.jar .
EXPOSE 8383
ENTRYPOINT ["java","-jar","/dockerrepo/demopro.jar"]