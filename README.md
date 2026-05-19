# Spring AI Samples

A collection of sample projects demonstrating [Spring AI](https://docs.spring.io/spring-ai/reference/) capabilities and integrations.

## Prerequisites

- **Java 25** or later
- **Maven 3.9+** (or use the included Maven Wrapper)

## Project Structure

```
spring-ai-samples/
├── mcp-code-mode/          # MCP Client sample application
├── pom.xml                 # Parent POM (Spring Boot 4.0.5, Spring AI 2.0.0-M4)
└── README.md
```

## Building the Project

Using the Maven Wrapper:

```bash
./mvnw clean install
```

Or with a locally installed Maven:

```bash
mvn clean install
```

## Modules

### mcp-code-mode

A Spring AI MCP (Model Context Protocol) Client sample application. This module demonstrates how to integrate with MCP servers using the `spring-ai-starter-mcp-client` dependency, enabling your application to interact with AI models through the standardized Model Context Protocol.

**Key dependencies:**

- `spring-boot-starter`
- `spring-ai-starter-mcp-client`

**Main class:** `McpCodeModeApplication`

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
