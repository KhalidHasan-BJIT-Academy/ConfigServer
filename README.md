#  Config Server


## Overview

The Config Server is a central component of the system that manages configuration properties for various microservices. It is built using the Spring Cloud Config Server, providing a centralized configuration management solution.

## Configuration

The configuration for the Config Server is stored in the `application.yml` file, which is hosted on [GitHub](https://github.com/KhalidHasan-BJIT-Academy/ConfigServer.git). Here are the key configuration properties explained:

-   **`server.port`**: Specifies the port on which the Config Server will run. In this configuration, it is set to `8085`.
    
-   **`spring.application.name`**: Defines the name of the Spring application. In this case, it is set to `config-server`.
    
-   **`spring.cloud.config.server.git.uri`**: Specifies the URI of the Git repository where the configuration files are stored. In this example, it is set to `https://github.com/KhalidHasan-BJIT-Academy/ConfigServer.git`.
    
-   **`spring.cloud.config.server.git.clone-on-start`**: Determines whether the Config Server should clone the configuration repository on startup. If set to `true`, the server will fetch the latest configuration from the Git repository when it starts.
    

## Getting Started

To set up the Config Server locally, follow these steps:

1.  Clone this repository to your local machine.
    
    bashCopy code
    
    `git clone https://github.com/KhalidHasan-BJIT-Academy/ConfigServer.git` 
    
2.  Navigate to the project directory.
    
    bashCopy code
    
    `cd ConfigServer` 
    
3.  Ensure that you have Java and Maven installed.
    
4.  Run the Config Server.
    
    bashCopy code
    
    `mvn spring-boot:run` 
    
5.  The Config Server will start on the specified port (`8085` in this example).
    

## Usage

Once the Config Server is up and running, microservices can connect to it to retrieve their configuration properties. Configure your microservices to point to this Config Server for centralized configuration management.
