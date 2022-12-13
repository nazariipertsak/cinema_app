# :cinema: Cinema-Service :cinema:
# Project description
Simple simulation of cinema service for ordering tickets that supports authentication, registration and other CRUD operations.
# Features
- registration or login as user
- create(only for user with role Admin) and find movies
- create(only for user with role Admin) and find available movie-sessions
- create shopping cart
- add tickets to shopping cart
- complete an order
- get order history for current user
- find user by email(only for user with role Admin)
- delete movie-sessions(only for user with role Admin)
# Project structure
Project uses 3-tier architecture:
1. Data access tier -> handled by DAO;
2. Business logic tier -> handled by Service;
3. Presentation tier -> handled by Controllers and Spring.
   <img src="structure.png" width="75%">
# Technologies
- Maven
- Java programming language (JDK 11)
- JDBC
- Spring
- Spring-Web
- Spring-Security
- Hibernate
- Tomcat 9.0.50
- MySQL 8.0
# Instructions to run my project
Copy content of it and then paste it to your DBMS query. I am using mySQL. <br/>
1. Configure connection to your database in
> [cinema-app/src/main/resources/db.properties]

By changing driver, url to your database, username and password to your own. <br/>
2. Run in console [mvn clean package] for project to build up. <br/>
3. Run this in server. I am using Tomcat 9.0.50. <br/>
