# Start with a Maven image to build the project
FROM openjdk:17

# Start with a Maven image to build the project
FROM maven:3.9.4-eclipse-temurin-17 AS build
# Copy the project files
COPY . .
# Build the project and package the JAR
RUN mvn clean package -DskipTests
# Expose port (change if your app uses a different one)
EXPOSE 8080

# Run the application
ENTRYPOINT ["java", "-jar", "spring-boot-docker.jar"]