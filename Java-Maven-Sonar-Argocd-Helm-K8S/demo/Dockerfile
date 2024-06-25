# Use the correct base image for Java 17
FROM openjdk:17-alpine

# Define the path to the artifact as a build argument
ARG artifact=target/demo-0.0.1-SNAPSHOT.jar

# Set the working directory inside the container
WORKDIR /opt/app

# Copy the Spring Boot JAR file into the container
COPY ${artifact} app.jar

# Define the entry point for the container
ENTRYPOINT ["java", "-jar", "app.jar"]
