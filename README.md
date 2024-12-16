# DocumentServiceApp

## 📌 Introduction

DocumentServiceApp is a microservices-based application developed using the Spring framework. Its primary purpose is to manage documents by enabling users to upload, update, and delete them in various databases. The project incorporates JWT authentication for secure access and utilizes the Saga pattern for reliable distributed transactions.

The system consists of four main microservices:

- DocumentService: Serves as the API gateway of the application, providing a user-facing interface for receiving requests.
- DocumentData: Handles document processing and stores them in a PostgreSQL database before passing the documents to another service.
- DocumentDataMongo: Stores documents in a MongoDB database for additional persistence.
- DocumentAuth: Manages user registration, generates JWT tokens for authentication, and stores user information in a PostgreSQL database.

To facilitate communication between the microservices, RabbitMQ is used as the message broker. Each microservice is containerized using Docker for ease of deployment and scalability.

## 🛠 Technologies Used

Main
- Java
- SpringFramework(boot, security, web, data)
  
Database
- PostgreSQL
- MongoDB
  
ORM
- Hibernate
  
Tests
- JUnit/Mockito
  
Tools
- Maven
- Docker/Docker-compose
- RabbitMQ
- JWT

## 📁 Repositories

API microservice
- https://github.com/freshhuk/DocumentService
  
Postgres microservice
- https://github.com/freshhuk/DocumentData
  
Mongo microservice
- https://github.com/freshhuk/DocumentDataMongo
  
Authorization microservice
- https://github.com/freshhuk/DocumentAuth
