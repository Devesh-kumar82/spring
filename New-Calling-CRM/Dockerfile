# Use Maven with Java 17 installed
FROM maven:3.8.1-openjdk-17

# Set the working directory in the container
WORKDIR /OutboundCRM/

# Copy the Maven project files to the container
COPY . .

# Install the dependencies and build the project
#RUN mvn clean install -DskipTests
CMD ["mvn" , "clean" , "install" , "-DskipTests"]

# Set the command to run the Spring Boot application when the container starts
CMD ["mvn", "spring-boot:run", "-Dspring.profiles.active=prod"]

