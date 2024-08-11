FROM maven:3.8.8-openjdk-11 AS build
COPY . .
RUN mvn clean package
FROM openjdk:11
WORKDIR /dockerrepo
COPY --from=build /javaapps-github/target/demopro.jar .
EXPOSE 8383
ENTRYPOINT ["java","-jar","/dockerrepo/demopro.jar"]