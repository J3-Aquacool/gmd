FROM openjdk:17-jdk-alpine
WORKDIR /javaapps-github
EXPOSE 8383
RUN mvn clean package
COPY --from=build /javaapps-github/target/demopro.jar /dockerrepo/demopro.jar
ENTRYPOINT ["java","-jar","/javaapps-github/demopro.jar"]