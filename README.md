# E-Commerce Platform with Microservices and Serverless Architecture

This project demonstrates how to build a simplified **E-Commerce Platform** using **Microservices Architecture** and **Serverless Technology**. The platform includes three core services: **Product Service**, **User Service**, and **Order Service**, running independently in a containerized environment.

## Features

- **Product Management Service**: Handles product details, categories, and inventory.
- **User Management Service**: Handles user authentication, profile management, and session management.
- **Order Processing Service**: Handles order placements, status tracking, and payment processing.

## Architecture

- **Microservices**: Each service (product, user, and order) is a standalone Spring Boot application.
- **Azure Functions**: Serverless operations for processing specific tasks such as notifications or batch jobs.
- **Cosmos DB**: NoSQL database for storing product details and order history.
- **Docker & Kubernetes**: Services are containerized and can be orchestrated using Kubernetes for scaling.
- **CI/CD Pipeline**: Continuous integration and deployment using GitHub Actions or Azure DevOps.

## Getting Started

### Prerequisites
- Install Docker on your machine.
- Clone this repository to your local machine.
- Ensure you have **Docker** and **Docker Compose** installed.

### Running the Project Locally
1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/e-commerce-platform.git
    cd e-commerce-platform
    ```

2. Build and start the services using Docker Compose:
    ```bash
    docker-compose up --build
    ```

3. Once the services are up and running, visit the following URLs:
    - **Frontend**: [http://localhost:3000](http://localhost:3000)
    - **Product Service**: [http://localhost:8081/products](http://localhost:8081/products)
    - **Order Service**: [http://localhost:8083/orders](http://localhost:8083/orders)

## Technologies Used

- **Spring Boot**: For building the backend services.
- **Azure Functions**: For serverless computation and handling specific tasks.
- **Cosmos DB**: As the primary database for storing product and order information.
- **Docker**: For containerizing the services.
- **Kubernetes**: For managing the services and scaling.
- **GitHub Actions/Azure DevOps**: For Continuous Integration and Continuous Deployment (CI/CD).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
