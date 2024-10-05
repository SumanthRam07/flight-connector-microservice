# Flight Connection Microservice

**Author:** Sumanth Gollaprolu  
**Email:** [sgollaprolu2023@fau.edu](mailto:sgollaprolu2023@fau.edu)

---

## Overview

This repository contains the source code for an **Airport Flight Connection Builder**. The Flight Connection Builder is used to find all possible flights arriving at a particular city which can be connected with all flights departing from the same city.

For example, if you want to travel from **Mumbai (BOM)** to **New York (JFK)** via **London (LHR)**, the system finds all possible flights arriving in London from Mumbai that can connect with all flights departing from London to New York City. The application consists of multiple microservices:

- **Connection Builder Microservice**: Contains the business logic for building flight connections.
- **Master Data Microservice**: Manages data about airports, such as airport code, name, city, coordinates, and flight schedules between airports.
- **Spring Cloud API Gateway Microservice**: Manages routing and communication between microservices.
- **ReactJS Web Application**: Provides the frontend interface for the application.

## Architecture

This system uses **Event-Driven Architecture** facilitated by **RabbitMQ**, allowing microservices to remain loosely coupled. **Test-Driven Development (TDD)** is followed using **Mockito** for unit testing.

## Prerequisites

To run this application, ensure the following prerequisites are installed on your system:

- **Java SDK** (version 11 or higher)
- **Docker** and **Docker Compose**
- **RabbitMQ** (for event-driven communication)
- **Consul** (for service discovery and configuration)

## Running the Application Using Docker Compose

1. Clone the repository and navigate to the project's root directory:

   ```bash
   git clone <repository-url>
   cd <repository-directory>

Run the following command to build and start the application using Docker Compose:

docker-compose up --build 


## Installation
- **Clone the repository or download and extract the archive file to your local directory**
- **Build each SpringBoot microservice by running the command ./gradlew clean bootJar. This will create a modern cloud native fully self-contained JAR file**
- **Install the dependencies for the frontend by running npm install --legacy-peer-deps. The --legacy-peer-deps flag is used to solve a possible conflicting peer dependency error**
- **Start the frontend by running npm start.

## Important Steps Before Using the Application
Before searching for flight connections, make sure to perform the following:

- ** Create New Airports: Use the Master Data Microservice to register new airports with their respective codes, names, cities, and coordinates **
Add Flight Schedules: Add flight schedules between the registered airports to enable the flight connection builder to find potential routes **




## Let me know if you'd like any more modifications or if you want me to add additional sections





