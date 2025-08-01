# API Gateway

This project is the heart of a microservices-based online compiler system. The API Gateway acts as a single entry point
for all client requests, routing them to the appropriate backend language services (Java, Python, C++, etc.). It
provides centralized routing, security, and cross-origin resource sharing (CORS) configuration, making the system
scalable and easy to manage.

## What Does This Project Do?

The API Gateway simplifies client interaction with multiple language compiler microservices by:

- Exposing a unified API endpoint for code compilation and execution requests
- Routing requests to the correct language service (Java, Python, C++, etc.)
- Handling CORS and security policies
- Integrating with Eureka Service Discovery for dynamic service registration and discovery
- Providing a foundation for future enhancements like authentication, rate limiting, and monitoring

## Features

- **Centralized Routing:** All client requests are routed through a single gateway.
- **CORS Configuration:** Secure cross-origin requests for frontend-backend communication.
- **Service Discovery:** Seamless integration with Eureka for dynamic service management.
- **Scalability:** Easily add or remove language services without changing the client.
- **Extensibility:** Ready for future features like authentication, logging, and monitoring.

## Technologies Used

- **Spring Boot**: For building the API Gateway and microservices
- **Spring Cloud Gateway**: For routing and filtering requests
- **Eureka (Netflix OSS)**: For service discovery
- **Gradle**: For project build and dependency management
- **Java 17**: Main programming language

## Microservices in the System

- [Eureka Server](https://github.com/kratikpal/compiler_eureka_server)
- [C++ Service](https://github.com/kratikpal/cpp_service)
- [Java Service](https://github.com/kratikpal/java_service)
- [Python Service](https://github.com/kratikpal/python_service)

## Demo

Watch a demo of the system in action:

[Demo Video](https://github.com/user-attachments/assets/493fd599-5ae1-455a-8f99-9a7ee41ca601)

## Project Structure

- `src/main/java/com/compiler/apigateway/` - Main application source code
- `src/main/resources/application.yml` - Application configuration
- `build.gradle` - Build configuration

## Getting Started

### Prerequisites

- Java 17 or higher
- Gradle

### Running the API Gateway

1. Clone the repository.
2. Navigate to the `ApiGateway` directory.
3. Build the project:
   ```sh
   ./gradlew build
   ```
4. Run the application:
   ```sh
   ./gradlew bootRun
   ```

The API Gateway will start on the default port (configured in `application.yml`).

### Configuration

- Update `application.yml` to change ports, routes, or other settings as needed.
- Integrate with Eureka by enabling service discovery in your configuration.

