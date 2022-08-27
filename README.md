# Title of the project #
registre-Service (Eureka)

# Description of the project
Registre-service is the microservice in which all the other microservices will register in order to make them available to the other microservices.

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

#Full system deployment order

1. Deploy the MS config-service as indicated in the readme.md located the classpath of the config-service project.
2. Deploy the MS registre-service as indicated in the readme.md located the classpath of the registre-service project.
3. Deploy the MS gateway-service as indicated in the readme.md located the classpath of the gateway-service project.
4. Deploy the MS hopital-service as indicated in the readme.md located the classpath of the hopital-service project.
5. Deploy the MS reservation-service as indicated in the readme.md located the classpath of the reservation-service project.