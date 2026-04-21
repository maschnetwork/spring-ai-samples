# Spring AI Samples

A collection of sample projects demonstrating [Spring AI](https://docs.spring.io/spring-ai/reference/) capabilities. This is a multi-module Maven project that serves as a reference for building AI-powered applications with Spring Boot.

## Tech Stack

| Technology | Version |
|---|---|
| Java | 25 |
| Spring Boot | 4.0.5 |
| Spring AI | 2.0.0-M4 |
| Build Tool | Maven |

> **Note:** This project uses Spring AI `2.0.0-M4`, which is a milestone release. The Spring Milestones repository (`https://repo.spring.io/milestone`) is configured in the root `pom.xml` to resolve these dependencies.

## Modules

| Module | Description |
|---|---|
| [mcp-code-mode](mcp-code-mode) | Spring AI MCP (Model Context Protocol) Client sample application |

### mcp-code-mode

A Spring Boot application demonstrating the Spring AI MCP Client integration. It uses the `spring-ai-starter-mcp-client` starter to connect to MCP-compatible servers.

**Dependencies:**
- `spring-boot-starter` - Core Spring Boot support
- `spring-ai-starter-mcp-client` - Spring AI MCP Client auto-configuration
- `spring-boot-starter-test` - Testing support

## Prerequisites

- **Java 25** - Required by the project configuration. You can use [Amazon Corretto](https://docs.aws.amazon.com/corretto/latest/corretto-jdk25-ug/what-is-corretto-jdk25.html), [Eclipse Temurin](https://adoptium.net/), or any other compatible JDK distribution.
- **Maven 3.9+** - The project uses the Maven wrapper, so a local Maven installation is optional.

## Building

Clone the repository and build all modules:

```bash
git clone https://github.com/maschnetwork/spring-ai-samples.git
cd spring-ai-samples
mvn verify
```

To build a specific module:

```bash
mvn verify -pl mcp-code-mode
```

## Project Structure

```
spring-ai-samples/
├── pom.xml                  # Parent POM with shared configuration
├── mcp-code-mode/           # MCP Client sample module
│   ├── pom.xml
│   └── src/
│       └── main/
│           ├── java/        # Application source code
│           └── resources/   # Configuration files
├── .github/
│   └── workflows/
│       └── build.yml        # CI pipeline
└── LICENSE
```

## CI/CD

The project uses GitHub Actions for continuous integration. The [build workflow](.github/workflows/build.yml) runs on every push to `main` and on pull requests. It sets up Java 25 (Corretto distribution) with Maven caching and runs `mvn verify`.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

Copyright (c) 2025 Maximilian Schellhorn
