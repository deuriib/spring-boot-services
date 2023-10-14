# Spring Boot Services

This repository contains a set of Spring Boot services that showcase different functionalities and interactions.

## Prerequisites

Before you start working with this project, ensure the following prerequisites are met:

- Java 17 Development Kit (JDK)
- Maven
- Your favorite Integrated Development Environment (IDE)

## Getting Started

Follow these steps to set up and run the project:

1. Clone the repository:

    ```bash
    git clone https://github.com/deuriib/spring-boot-services.git
    ```

2. Navigate to the project directory:

    ```bash
    cd spring-boot-services
    ```

3. Build each service using Maven and paketo-buildpacks:

    ```bash
    cd {service-name}
    ```

4. Run the desired service:

    ```bash
    ./mvnw spring-boot:build-image
    ```

5. Run all the services with Docker Compose:

    ```bash
    docker compose up -d
    ```

Replace `{service-name}` with the specific service you want to run.

## Services

### Events Service

Rest API that allows users to retrieve information about events using PostgreSQl as data storage.

### Registration Service

Rest API that allows users to create registration for an event from Events Service through RestClient using mongoDB as
data storage.

...

## Usage

Each service has its autuator endpoints enabled. You can access them by navigating to `http://localhost:{port}/actuator`
where `{port}` is the port of the service you want to access.

