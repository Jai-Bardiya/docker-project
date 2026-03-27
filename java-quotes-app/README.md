# Java Motivational Quotes App

This project is a simple Java-based HTTP server that serves random motivational quotes via a REST API. The quotes are externalized to a `quotes.txt` file for easy customization.

## Features
- Serves random motivational quotes in JSON format.
- Uses an external `quotes.txt` file for configurable quotes.
- Lightweight HTTP server using `com.sun.net.httpserver.HttpServer`.
- Dockerized for easy deployment.

## Requirements
- Java 17+
- Maven (if building from source)
- Docker (optional, for containerized deployment)

## File Structure
```
project-root/
│── src/
│   └── Main.java
│── quotes.txt
│── Dockerfile
│── README.md
│── target/
│   └── myapp.jar (if using Maven build)
```











