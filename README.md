# Title of the project #
registre Service (Eureka)

# Description of the project
Registre service is the microservice in which all the other microservices will register in order to make them available to the other microservices.

Note : it must be launched right after the configuration microservice (config-service) has been launched.


#Requirements
1. Java 17
2. Maven 3.8.6

#Build
command line : mvn clean install (see jenkinsfile)

#Packaging the application
command line : mvn clean package -DskipTests (see the project's jenkins file)

#Deploy
command line : mvn spring-boot:run