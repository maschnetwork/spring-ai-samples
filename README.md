# Spring AI Samples

A collection of sample projects demonstrating [Spring AI](https://docs.spring.io/spring-ai/reference/) capabilities, built with Spring Boot 4 and Java 25.

## Project Structure

```
spring-ai-samples/
├── mcp-code-mode/          # MCP Client Code Mode sample
├── .github/workflows/      # CI/CD pipeline
├── pom.xml                 # Parent POM (multi-module)
└── LICENSE
```

## Modules

### mcp-code-mode

A Spring Boot application showcasing the [Model Context Protocol (MCP)](https://modelcontextprotocol.io/) client integration with Spring AI. It uses the `spring-ai-starter-mcp-client` starter to connect to MCP-compatible tool servers.

## Tech Stack

| Technology    | Version      |
|---------------|--------------|
| Java          | 25           |
| Spring Boot   | 4.0.5        |
| Spring AI     | 2.0.0-M4     |
| Maven         | 3.9+         |

## Prerequisites

- **JDK 25** (e.g., [Amazon Corretto 25](https://docs.aws.amazon.com/corretto/latest/corretto-25-ug/what-is-corretto-25.html) or any compatible distribution)
- **Maven 3.9+** (or use the Maven wrapper if provided)

## Building

Clone the repository and build all modules:

```bash
git clone https://github.com/maschnetwork/spring-ai-samples.git
cd spring-ai-samples
mvn verify
```

> **Note:** This project depends on Spring AI milestone releases. The Spring Milestones repository (`https://repo.spring.io/milestone`) is already configured in the parent POM, so no additional repository setup is required.

## Running a Sample

Each module is a standalone Spring Boot application. To run the MCP Code Mode sample:

```bash
cd mcp-code-mode
mvn spring-boot:run
```

## CI/CD

The project uses GitHub Actions for continuous integration. The pipeline runs on every push to `main` and on pull requests:

- Checks out the code
- Sets up Java 25 (Corretto)
- Builds and verifies with `mvn verify`

## License

This project is licensed under the [MIT License](LICENSE).

Copyright (c) 2025 Maximilian Schellhorn
