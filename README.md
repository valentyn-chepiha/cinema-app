# Cinema-app

## Description
Cinema-app is the server side of an online ticket booking application. 
Based on REST API.
This project made to show my skills in Spring, Spring security, Exception handler, Hibernate, REST, OOP, SOLID, data layers. 
In this project I used basic CRUD operations.
One-to-one, one-to-many, and many-to-many relationships are used in databases.

## Technologies
- Java 11
- Spring
    - Spring security
    - Exception handler
    - Hibernate validator
- Hibernate
- MySQL
- Swagger 2
- TomCat 9.0.50

## How to use
- First, run the project. 
- To DB inserted roles: USER and ADMIN
- You can then create an account to log into the app
- use "GET: /swagger-ui.html" to access the Swagger UI
- After that, you can perform CRUD operations with movies, cinema halls, movie sessions and tickets

## REST API
    POST: /register - ACCESS: all
    GET: /cinema-halls - ACCESS: user/admin
    POST: /cinema-halls - ACCESS: admin
    GET: /movies - ACCESS: user/admin
    POST: /movies - ACCESS: admin
    GET: /movie-sessions/available - ACCESS: user/admin
    POST: /movie-sessions - ACCESS: admin
    PUT: /movie-sessions/{id} - ACCESS: admin
    DELETE: /movie-sessions/{id} - ACCESS: admin
    GET: /orders - ACCESS: user
    POST: /orders/complete - ACCESS: user
    PUT: /shopping-carts/movie-sessions - ACCESS: user
    GET: /shopping-carts/by-user - ACCESS: user
    GET: /users/by-email - ACCESS: admin

## Setup
- Clone this project
- Create the required tables using file resources/init_db.sql
- Add your db configurations in resources/db.properties (username, password, url)
````-
    db.url=url connection string to DB
    db.user=USERNAME
    db.password=PASSWORD
````
- Config TomCat
- Run project using TomCat
