# Use an official Java runtime as the base image
FROM openjdk:17-jdk-slim

# Set working directory
WORKDIR /app

# Copy the Spring Boot JAR file to the container
COPY target/flight-management-backend-0.0.1-SNAPSHOT.jar flight-management-backend.jar

# Expose the port your Spring Boot application runs on
EXPOSE 8080

# Run the Spring Boot application
ENTRYPOINT ["java", "-jar", "flight-management-backend.jar"]
