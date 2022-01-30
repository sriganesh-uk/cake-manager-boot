Cake Manager Spring Boot Application
=======================================

Created the below APIs and added the functionality as below:
	1. On application start-up, loads all the cakes presented in cake.json (https://gist.githubusercontent.com/hart88/198f29ec5114a3ec3460/raw/8dd19a88f9b8d24c23d9960f3300d0c917a4f07c/cake.json) into in-memory DB.
	2. Accessing the root of the application (/), it opens index.html file and displays all the cakes currently in the system in Tabular format 
	3. When we click on "Add Cake" button, it takes to new addCake.html file in which we can enter the new cake details and submit. It adds the new cake into Database.
	4. An API with "/cakes" endpoint with GET, gets the cakes currently in the system as JSON data.
	5. An API with "/cakes" endpoint with POST and body, savs the cake into the DB.

	
* Added Test cases for all the endpoints in the application. Test cases exists in "src/test/java" folder.
* Added Dockerfile for Containerisation.


Software Stack used in the application
---------------------------------------
	Spring Boot
	Hibernate
	Thymeleaf
	Junit
	HSqlDB
	Tomcat
	Maven


Running the Project
=====================

Since, the spring boot application has in-built Tomcat server, execute the following commands too run a application locally:

	1. Run the Maven Install to generate jar file 
		`mvn clean install`
	2. Run the application by following command in (project root folder/targer)
		java -jar cake-manager.jar
	3. Access the application using the following URL:
		`http://localhost:8080/`

