# Nile Commerce

## Summary
This Repo contains the back-end code of a mock E-Commerce site called Nile Commerce. The purpose of the code is to allow create a database that the front-end engineer can then access to add, delete and change the rows to the databases tables. It uses industry standards such as a RESTful API (Representational State Transfer) and CRUD (Create, Read, Update, Delete). in addition, sequelize, ORM and insomnia are used as well.

## Connection.js
This file is in charge of making the connection to sequelize and the "ecommerce_db" database and exports that connection to the server.js and the models folder with the exception of models/index.js.

## schema.js
The schema file simply drops the database if its used and creates new one.
## models
All models where made using sequelize and follow ORM technique. Each model was made as an extension of sequalize's Model and given its unique attributes as well as selecting sequelize's options. After that each class is exported to the index.js file in the models folder to define associations.

## Routes
This Folder takes care of all of the RESTful API endpoints and their CRUD operations and exports them to the index.js file that adds another layer to the url and sends them all to server.js to be used as a single package.

## Seeds
This folder simply populates the database, using "npm run seed", with mock data, this folder is not needed to use the backend.

## Server.js
Server.js connects to express.js and allows sequelize to sync all the data with the server.
## Walkthrough Video
https://drive.google.com/file/d/1k5oWKBWFdxqlcoZH0HsTvQEMqnR80OGi/view