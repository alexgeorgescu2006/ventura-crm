# Ventura CRM

Ventura CRM is a REST API backend for Customer Relationship Management, built on the Spring Boot framework. The project provides a reliable foundation for data persistence, API documentation, and testing.

##  Tech Stack

* **Framework:** Spring Boot 3.2.5
* **Language:** Java 17
* **Database & ORM:** Spring Data JPA with a PostgreSQL runtime driver for production environments
* **Testing Database:** H2 In-Memory Database
* **Validation:** Spring Boot Bean Validation
* **API Documentation:** Swagger UI integrated via Springdoc OpenAPI 2.5.0
* **Developer Tools:** Spring Boot DevTools
* **Build Tool:** Apache Maven

##  Getting Started

You do not need to install Maven locally to build or run this application. Instead, you can use the included Maven Wrapper scripts.

**To run the application on Linux/macOS:**
```bash
./mvnw spring-boot:run
📂 Project Configuration
Dependencies:
 Defined in the pom_2.xml file, which includes standard Spring Boot starters (Web, Data JPA, Validation, Test) alongside OpenAPI[cite: 41].
It explicitly overrides the <license> and <developers> elements inherited from the Spring Boot parent POM.

Source Control Management:
The repository includes a .gitignore_2 customized for IDEs like Spring Tool Suite (STS), IntelliJ IDEA, NetBeans, and VS Code.
It ignores Maven's target/ directory and .mvn/wrapper/maven-wrapper.jar.
Line endings are enforced via .gitattributes_2 (LF for mvnw, CRLF for *.cmd).

Code Quality Analysis:
The project is configured to use Qodana via the qodana.yaml file, utilizing the qodana.starter profile
and the jetbrains/qodana-jvm:2026.2 linter image in the CI/CD pipeline.   
