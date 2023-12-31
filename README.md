﻿# Cinema Ticket Reservation
### Project description:
A simple simulator of cinema service for reservation tickets, that supports registration, authentication and CRUD operations

![](Cinema_UML.png)
### Features:
* registration
* authentication
* app have roles with different rights - admin/user
* create and find movies
* create and find available movie sessions
* create shopping cart
* add tickets to shopping cart
* complete an order

### Detailed API breakdown:
* POST: /register (all) - register new user;
* POST: /cinema-halls (admin) - add a new cinema hall;
* POST: /movies (admin) - add a new movie;
* POST: /movie-sessions (admin) - add a new movie session;
* POST: /orders/complete (user) - create a new order for current user;
* GET: /cinema-halls (user/admin) - get a list of all cinema halls;
* GET: /movies (user/admin) - get a list of all movies;
* GET: /movie-sessions/available (user/admin) - get available movie sessions by date;
* GET: /orders (user) - get a list of orders for current user;
* GET: /shopping-carts/by-user (user) - get shopping cart of current user;
* GET: /users/by-email (admin) - find user by email;
* PUT: /movie-sessions/{id} (admin/root) - update movie session;
* PUT: /shopping-carts/movie-sessions (user) - creates a ticket and adds it to the shopping cart of current user;
* DELETE: /movie-sessions/{id} (admin/root) - delete movie session.

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
