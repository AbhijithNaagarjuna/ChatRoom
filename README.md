# ChatRoom
Chat Room Application Using Spring Boot WebSocket STOMP

# Introduction
This application is a simple chat room application developed using web-sockets in Java. The basic tasks users can perform are:

entering a room
sending messages
leaving the room
In the below sections, I will present an overview of the project components, what are the classes that make up the project and some few pointers on future scope.

# Web Socket
WebSocket is a communication protocol that makes it possible to establish a two-way communication channel between a server and a client.

# System Design
I will go through the important classes and their workings as well. Some additional html and xml files that complete the project and are essential are also explained.

# Message.java
Message is a model class. It is the message payload that will be exchanged between the client and the server.

# WebSocketChatServer.java
WebSocketChatServer is the controller class. It has below method implementations:-

onOpen:Establishes a connection between client and server

onMessage: Gets session and user information and sends messages.

sendMessageToAll: Sends the message to all connected users

onClose:Closes the connection

# WebSocketConfig.java
WebSocketConfig is the web socket configuration file which defines server endpoint exporter

# LoginController.java
LoginController is controller file to implement the login functionality and render the chat url

# WebSocketChatApplication.java
WebSocketChatApplication is the main class to boot the application

login.html
This view-page helps the user to login.

chat.html
This view-page shows the chat window where user can also type-in his\her message

pom.xml
Its the maven build file with dependency on spring-boot-starter-web, spring-boot-starter-websocket, spring-boot-starter-thymeleaf, jquery, fastjson.
