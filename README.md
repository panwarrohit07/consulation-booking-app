Project Title
Book my consulting API serves backend services to manage doctors appointment. It has been built on Spring platform using spring-boot framework.

Getting Started
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

Prerequisites
You need following softwares before running this applic ation.

Java 8 SDK
Apache Maven 3.3 build tool
MySQl version 8.14
Your favorite IDE such as Intellij/Eclipse (optional)
Postman Client for REST APIs testing (optional)
Installing and Deployment
A step by step guide that helps you get a development env running

Create database named consultation with associated owner root and execute the SQL commands in the file /src/main/resources/DBLoadScript.sql

Checkout repo

Go to the folder where the above project has been checked out

update the user name password in the appliaction.properties file

   spring.datasource.username={uname}
   spring.datasource.password={pwd}
Build the project using maven command mvn clean install -DskipTests. First time build will consume time as it downloads all dependencies. ```

start the application using command mvn spring-boot:run

Access the following healthcheck url http://localhost:8080/actuator/health that should result in following output

{
    "status": "UP"
}
Use the postman collection in the repo bookmyconsultation.postman_collection.json

Best wishes!
