FROM openjdk:17-jdk-alpine
WORKDIR /javaapps-github
EXPOSE 8383
COPY /target/demopro.jar /javaapps-github/demopro.jar
ENTRYPOINT [ "java","-jar","/javaapps-github/demopro.jar"]