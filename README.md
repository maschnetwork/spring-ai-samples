# Spring AI Samples

A multi-module Maven project containing Spring AI sample applications.

## Prerequisites

- Java 25
- Maven 3.9+ (or use the included Maven Wrapper `./mvnw`)

## Project Structure

```
spring-ai-samples/
├── mcp-code-mode/   # Spring AI MCP Client sample
└── pom.xml          # Parent POM
```

## Modules

### mcp-code-mode

A sample application demonstrating the Spring AI Model Context Protocol (MCP) Client. This module uses `spring-ai-starter-mcp-client` to interact with MCP-compatible servers.

## Building the Project

Using the Maven Wrapper:

```bash
./mvnw clean install
```

Or with a locally installed Maven:

```bash
mvn clean install
```

## Spring AI Milestone Repository

This project uses Spring AI 2.0.0-M4, which is a milestone release. The required Spring Milestones repository (`https://repo.spring.io/milestone`) is already configured in the parent POM, so no additional repository setup is needed.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

Copyright 2025 Maximilian Schellhorn
