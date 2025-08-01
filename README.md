# API Gateway

This project is an API Gateway for a microservices-based online compiler system. It acts as a single entry point for
client requests and routes them to the appropriate backend services (such as Java, Python, C++, etc.).

## Features

- Centralized routing for multiple language compiler services
- CORS configuration for secure cross-origin requests
- Built with Spring Boot and Java
- Easy integration with Eureka Service Discovery

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

## License

This project is licensed under the MIT License.

