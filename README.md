# Spring AI Samples

A multi-module Maven project containing Spring AI sample applications.

## Prerequisites

- Java 25
- Maven 3.9+

## Project Structure

```
spring-ai-samples/
├── pom.xml                  # Parent POM
├── mcp-code-mode/           # MCP Client sample module
│   ├── pom.xml
│   └── src/main/
│       ├── java/com/maschnetwork/mcpcodemode/
│       │   └── McpCodeModeApplication.java
│       └── resources/
│           └── application.properties
└── LICENSE
```

## Building the Project

```bash
mvn clean install
```

## Modules

### mcp-code-mode

A Spring AI MCP (Model Context Protocol) Client sample application. This module demonstrates how to use the Spring AI MCP Client starter to interact with MCP-compatible services.

**Dependencies:**

- `spring-boot-starter`
- `spring-ai-starter-mcp-client`
- `spring-boot-starter-test`

## Spring AI Milestone Repository

This project uses Spring AI `2.0.0-M4`, which is a milestone release. The Spring milestone repository (`https://repo.spring.io/milestone`) is configured in the parent POM to resolve these dependencies.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

Copyright 2025 Maximilian Schellhorn
