# Use a multi-architecture base image for OpenJDK
FROM --platform=linux/amd64 openjdk:17-jdk-slim

# Set the working directory in the container
WORKDIR /app

# Copy the built JAR file from the target directory into the container
COPY target/flight-management-backend-0.0.1-SNAPSHOT.jar app.jar

# Expose port 8080 for the application
EXPOSE 8080

# Set the entry point for the container to run the Spring Boot application
ENTRYPOINT ["java", "-jar", "app.jar"]
