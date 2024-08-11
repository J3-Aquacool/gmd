FROM openjdk:17-jdk-alpine
WORKDIR /javaapps
COPY target/JavaApp.jar /javaapps/JavaApp.jar
ENTRYPOINT ["java", "-jar", "JavaApp.jar"]