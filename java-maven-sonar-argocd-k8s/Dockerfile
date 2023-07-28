#Use Java 11 image as the base image
FROM openjdk:17-ea-33-slim

# Define the parameter name and its default value (artifact path)
ARG artifact=target/spring-boot-web.jar

#Set the working directory in the container
WORKDIR /opt/app

# Copy the application code to the working directory
COPY ${artifact} app.jar

# Command will be executed upon running a container
ENTRYPOINT ["java","-jar","app.jar"]
