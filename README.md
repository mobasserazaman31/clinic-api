# Clinic API

Spring Boot REST API scaffold using Java 21, Maven, PostgreSQL, Spring Data JPA,
Flyway, validation, Spring Security OAuth2 resource server, and springdoc OpenAPI.

## Prerequisites

- Java 21 or newer
- Maven 3.9+
- PostgreSQL

## Configure and run

Create a PostgreSQL database named `immunization`, or set these environment
variables to match your database:

| Variable | Default |
| --- | --- |
| `DATABASE_URL` | `jdbc:postgresql://localhost:5432/immunization` |
| `DATABASE_USERNAME` | `postgres` |
| `DATABASE_PASSWORD` | `postgres` |

Start the application with:

```sh
mvn spring-boot:run
```

Build and run tests with:

```sh
mvn test
```

OpenAPI UI is available at `http://localhost:8080/swagger-ui.html` after the
application starts. Add database migrations under
`src/main/resources/db/migration` using Flyway's `V<VERSION>__<description>.sql`
naming convention.