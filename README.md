# Spring Boot Fusion MVC Skeleton

A lightweight application skeleton containing all boilerplate configurations needed to build a
[Spring Boot](https://spring.io/projects/spring-boot) REST (micro)service, designed for rapid feature development with
minimal setup.
Each feature is implemented as a self-contained module packaged as a JAR file, which is dynamically composed into the
application at runtime. 🧩

The primary goal of this project is to minimize configuration overhead in individual modules, allowing developers to
focus purely on implementing functionality.

## Key Goals

- **Zero-config module development** – just write your feature logic using familiar Spring annotations (e.g.,
  [@RestController](https://docs.spring.io/spring-framework/docs/current/javadoc-api/org/springframework/web/bind/annotation/RestController.html),
  [@Service](https://docs.spring.io/spring-framework/docs/current/javadoc-api/org/springframework/stereotype/Service.html)
  )
- **No compilation during image build** – modules are pre-built JARs simply copied into the container
- **Plug-and-play module architecture** – powered by Spring Boot auto-configuration and classpath scanning
- **Simple Docker packaging** – just include your modules in the image via configuration

## Application Features

- **Spring Boot Actuator** – provides production-ready observability features like metrics, health checks, and
  application info

## Build & Tooling Features

- **Maven Wrapper** – allows users to build the project without installing Maven locally
- **Versions Maven Plugin** – helps manage and update dependency versions easily

## Help

### Commands

#### Update Dependencies

```bash
./mvnw versions:update-parent
./mvnw versions:update-properties
```

## License

This project is licensed under the [Apache 2.0 License](LICENSE).
