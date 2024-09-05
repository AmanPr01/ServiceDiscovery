# Service Discovery

## Overview

The Service Discovery service is implemented using Netflix Eureka. It allows services to register themselves and discover other services in the system.

## Application Configuration

- **Port**: 8761
- **Eureka Configuration**:
  - `eureka.client.register-with-eureka`: `false`
  - `eureka.client.fetch-registry`: `false`

## Dependencies

- **Spring Cloud Starter Netflix Eureka Server**: Provides the Eureka server functionality for service registration and discovery.
- **Spring Boot DevTools**: Enhances development experience with features like automatic restarts and live reload.
- **Spring Boot Configuration Processor**: Enables support for metadata generation for configuration properties.
- **Lombok**: Simplifies code by reducing boilerplate code such as getters, setters, and constructors.
- **Spring Boot Starter Test**: Provides dependencies for testing Spring Boot applications.

## Additional Notes

- The Service Discovery service is essential for the dynamic registration and discovery of services in a microservices architecture.
- Ensure that other services are configured to register with this Eureka server for proper service discovery and communication.

## Related Services

- **[Product Service](https://github.com/AmanPr01/E-Commerce)**: Manages product information and operations.
- **[User Service](https://github.com/AmanPr01/UserService)**: Manages user authentication and authorization.
- **[Payment Service](https://github.com/AmanPr01/PaymentService)**: Manages payment processing and transactions.
- **[Email Service](https://github.com/AmanPr01/EmailService)**: Handles asynchronous email notifications.
