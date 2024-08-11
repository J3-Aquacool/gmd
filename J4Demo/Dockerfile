FROM openjdk:24-jdk-oracle
COPY . .
RUN mvn clean package
FROM openjdk:24-jdk-oracle
WORKDIR /dockerrepo
COPY --from=build /javaapps-github/target/demopro.jar .
EXPOSE 8383
ENTRYPOINT ["java","-jar","/dockerrepo/demopro.jar"]