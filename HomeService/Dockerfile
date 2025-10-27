# Start with a Maven image to build the project
FROM openjdk:17

EXPOSE 8080
ADD target/spring-boot-docker.jar spring-boot-docker.jar
# Run the application
ENTRYPOINT ["java", "-jar", "spring-boot-docker.jar"]