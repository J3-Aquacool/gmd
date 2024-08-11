FROM openjdk:17-jdk-alpine
WORKDIR /javaapps-github
EXPOSE 8383
COPY /target/dockerrepo.jar /javaapps-github/dockerrepo.jar
ENTRYPOINT [ "java","-jar","/javaapps-github/dockerrepo.jar"]