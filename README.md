# reverse-engineering

This application creates an authentication interface using passport npm package, express, express-session. 

The files and technologies within this application are listed below with their respective functions and definition. Below each explanation there is a link the website of the technology defined.

Middleware is software that acts as a liaison so to speak between an operating system and the
applications running on it. There are many forms of middleware technology which are used to transfer information from one program to another. 

An example: req(request),res(response) which are objects that are part of the function process in the applications request-response cycle.

In this case we are using "Passport" as our authentication middleware npm package. There are also other npm packages which are defined below.


Technologies:

Passport/Passport-Session: 

Passport is express compatible authenitcation for Node.js. This allows us to store and control login in data from the user and provide security for said data. We create and initialize our Passport login session using passport npm package.

https://www.npmjs.com/package/passport


Express: Express itself is comprised of wholly middleware functions. It's a web framework that let's you structure a web application to handle multiple different http requests at a specific url. By it's design it makes developing websites, web apps, & API's much easier.

https://www.npmjs.com/package/express



bcrypt: An npm package used as a secured way to store passwords in the database.

https://www.npmjs.com/package/bcryptjs


Sequelize: Sequelize is a ORM(Object-relational mapping) which is a programming technique for converting data between system types. It is also promise based npm package within Node. 

https://www.npmjs.com/package/sequelize


Here we will have a list of files used and their purpose within this application:


server.js file:

This file is where we link with all subsequent files needed to make the application function. It establishes our local PORT where we generate the file content. Express,Express-Passport, Passport, and Sequelize send user data to this file to generate after all necessary parameters are met. Server.js initializes the server.

Config folder: 

Hold files related to database configuration and authentication middleware i.e. (Passport) which protects users against unauthorized access to the application.

Models folder: 

Contains description on how user table should be designed. It also contains all validations. This folder contains user.js which utilizes bcryptjs for password security.


Public folder: 

Contains content like html,css,client side javascript. This is where we will do the general styling for the application on the frontend.

Routes folder: 

Contains api-routes.js and html-routes.js which allows for server and client side communication and application execution.


