FROM openjdk:17-jdk-alpin
WORKDIR /javaapps
COPY target/JavaApp.jar /javaapps/JavaApp.jar
ENTRYPOINT ["java", "-jar", "JavaApp.jar"]