# Patient Management System

Monorepo for a microservices-style **patient management** backend, built while following a course on **Java, Spring Boot, Docker, and Kafka**.

## Stack

- Java 21, Spring Boot 4.x  
- Maven  
- PostgreSQL (where configured) / H2 for local development (see `patient-service`)  
- Docker and Docker Compose (planned for the full system)  
- Kafka (planned for event-driven flows)

## Repository layout

| Path | Description |
|------|-------------|
| `patient-service/` | Patient domain API and persistence |

More services can be added alongside `patient-service/` as the course progresses.

## Prerequisites

- JDK 21  
- Maven (or use the Maven Wrapper inside each service)  
- Docker Desktop (when you add containers / Kafka / Postgres via Compose)

## Run `patient-service` locally

```powershell
cd patient-service
.\mvnw.cmd spring-boot:run
```

Default URL is typically `http://localhost:8080`. Check `patient-service/src/main/resources/application.properties` for port, datasource, and H2 console settings.
