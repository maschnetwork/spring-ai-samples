# Spring AI Samples

A collection of sample projects demonstrating [Spring AI](https://docs.spring.io/spring-ai/reference/) capabilities with practical, runnable examples.

## Tech Stack

- **Java 25**
- **Spring Boot 4.0.5**
- **Spring AI 2.0.0-M4**
- **Maven** (multi-module project)

## Project Structure

```
spring-ai-samples/
├── mcp-code-mode/          # MCP Client sample using Spring AI
├── pom.xml                 # Parent POM with shared configuration
└── .github/workflows/      # CI pipeline
```

## Modules

### mcp-code-mode

A Spring Boot application demonstrating the **Model Context Protocol (MCP)** client integration with Spring AI. MCP enables standardized communication between AI models and external tools/resources.

**Dependencies:**
- `spring-boot-starter`
- `spring-ai-starter-mcp-client`

## Prerequisites

- **Java 25** (e.g., [Amazon Corretto](https://docs.aws.amazon.com/corretto/latest/corretto-jdk25-ug/what-is-corretto-jdk25.html))
- **Maven 3.9+** (or use the Maven wrapper if available)

## Getting Started

### Build

```bash
mvn clean verify
```

### Run a Module

```bash
cd mcp-code-mode
mvn spring-boot:run
```

## Configuration

Each module has its own `application.properties` under `src/main/resources/`. Refer to the [Spring AI documentation](https://docs.spring.io/spring-ai/reference/) for available configuration options.

## CI/CD

The project uses GitHub Actions for continuous integration. The workflow builds and verifies the project on every push to `main` and on pull requests.

## License

This project is licensed under the [MIT License](LICENSE).

## Author

Maximilian Schellhorn
