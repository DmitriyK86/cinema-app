# Cinema-Service
### Project description:
A simple simulator of cinema service for reservation tickets, that supports registration, authentication and CRUD operations

### Features:
* registration
* authentication
* app have roles with different rights - admin/user
* create and find movies
* create and find available movie sessions
* create shopping cart
* add tickets to shopping cart
* complete an order

### Project structure:
#### Project has a 3-layer architecture:
* the data access layer;
* the application logic layer;
* the presentation layer.

### Used technologies:
* Java 17
* MySql 8.0.22
* Tomcat 9.0.73
* Spring MVC 5.3.20
* Hibernate 5.6.14
* Maven

### Instructions for running the application:
* Clone this repo to your IDE
* Replace YOUR_DRIVER, YOUR_DATABASE_URL, YOUR_LOGIN, YOUR_PASSWORD in db.properties on your own
* Install and configure Tomcat 9.0.73
* Run the application