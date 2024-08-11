FROM openjdk:11
COPY . .
RUN mvn clean package
FROM openjdk:11
WORKDIR /dockerrepo
COPY --from=build /javaapps-github/target/demopro.jar .
EXPOSE 8383
ENTRYPOINT ["java","-jar","/dockerrepo/demopro.jar"]