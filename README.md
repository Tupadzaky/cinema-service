﻿# Cinema-Service:

### Project description:
RESTful web app that supports user authentication, authorization and as well as various CRUD operations. Supports roles of user and admin. Does not have UI, interaction happens through postman.

## Table of Contents

[Functionality](#functionality)

[Endpoints](#endpoints)

[Project Structure](#project-structure)

[Technologies Used](#technologies-used)

[To run the project](#to-run-the-project)

## Functionality

  #### Admin Functionality:
  - adding, updating and deleting movies/cinema-halls/movie-sessions.
  - finding users by email.

  #### User Functionality: 
  - registration/login.
  - view movies/cinema-halls/movie-sessions.
  - search for available movie-sessions.
  - buy tickets as user.
  - view shopping cart.
  - view and complete orders.

## Endpoints

  #### Admin-only Endpoints
  - POST:   /cinema-halls - add a new cinema hall.
  - POST:   /movies - add a new movie.
  - POST:   /movie-sessions - add a new movie session.
  - PUT:    /movie-sessions/{id} - update a movie session by id.
  - DELETE: /movie-sessions/{id} - delete a movie session by id.
  - GET:    /users/by-email - find a user by email.

  #### User-only Endpoints
  - GET:  /orders - view your orders.
  - POST: /orders/complete - complete your order.
  - PUT:  /shopping-carts/movie-sessions - update the shopping cart with movie sessions.
  - GET:  /shopping-carts/by-user - view your shopping cart.
  
  #### User and Admin Endpoints
  - POST: /register - registrater a new user.
  - GET:  /cinema-halls - view cinema halls.
  - GET:  /movies - view movies.
  - GET:  /movie-sessions/available - view available movie sessions.

## Project Structure
- `src/main/java`: Contains all the source code for the application
- `src/main/resources`: Contains configuration files and resources

## Technologies used
- Java 17
- Spring 5.3.20
- Spring-Web 5.3.20
- Spring-Security 5.6.10
- Hibernate 5.6.14.Final
- MySQL 8.0.22
- Tomcat 9.0.76
- Maven 3.1.1

## To run the project
1. Clone this project from GitHub to your PC.
2. Install Apache Tomcat version 9.0.xx.
3. Install MySQL 8 or higher.
4. Install Postman.
5. Configure field values to your specific properties in the [db.properties](src/main/resources/db.properties)
6. Run the project and use Postman for convenient interactions.
