```
# Legacy EGP Application

A legacy Java EE (J2EE) enterprise application built with EJB 3.x, JSP/Servlets, and JPA. This multi-module Maven project represents a typical enterprise government portal (EGP) system from the mid-2000s era.

## Architecture

- **egp-core-ejb**: Core business logic with EJB 3.x stateless session beans, JPA entities, and DAOs
- **egp-portal-war**: Web presentation layer with JSP pages and servlets
- **egp-ear**: Enterprise Archive packaging both WAR and EJB JAR modules

## Modernization Plan

This modernization plan aims to bring the legacy EGP application up to current standards by implementing the following changes:

1. **Migration to Spring Boot**: Convert EJBs to Spring Beans, and migrate JSP/Servlets to Spring MVC.
2. **Use of JPA with Spring Data JPA**: Replace legacy JPA implementations with Spring Data JPA repositories.
3. **RESTful Services**: Replace servlets with RESTful APIs using Spring Web.
4. **Thymeleaf for View Layer**: Replace JSP with Thymeleaf templates.
5. **Dockerization**: Containerize the application using Docker for consistent development and production environments.
6. **Integration with CI/CD**: Implement a continuous integration and continuous deployment pipeline using GitHub Actions.

## Getting Started

### Prerequisites

- Java 17
- Maven 3.6+
- Docker
- Git

### Building the Project

1. Clone the repository:
    ```sh
    git clone https://github.com/BirlasoftCogitoai/legacy-codebasev1.git
    cd legacy-codebasev1
    ```

2. Build the project using Maven:
    ```sh
    mvn clean install
    ```

### Running the Application

1. Start the application using Docker Compose:
    ```sh
    docker-compose up
    ```

2. Access the application at `http://localhost:8080`.

## Contributing

We welcome contributions! Please read our [Contributing Guidelines](CONTRIBUTING.md) for more information.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
```