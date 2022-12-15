# :cinema: Cinema-Service :cinema:
# Project description
Simple REST API of cinema service for ordering tickets that supports authentication, registration and other CRUD operations.
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
- JDK 11
- JDBC
- Spring-Core
- Spring-Web
- Spring-Security
- Hibernate
- Tomcat 9.0.50
- MySQL 8.0
# Instructions to run my project
1. Clone this repository <br/>
2. Configure connection to your database in
> [cinema-app/src/main/resources/db.properties]

By changing driver, url to your database, username and password to your own. <br/>

3. Build project
```shell
mvn clean package
```
4. Run this in server. I am using Tomcat 9.0.50. <br/>
