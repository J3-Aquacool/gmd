FROM openjdk:11
EXPOSE 8383
COPY /target/dockerrepo.jar dockerrepo.jar
ENTRYPOINT [ "java","-jar","/dockerrepo.jar"]