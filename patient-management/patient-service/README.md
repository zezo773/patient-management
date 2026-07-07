# Patient Service

Java backend service for patient data management.

## Technology Stack

- **Java**
- **Spring Boot**
- **Maven (Wrapper included)**
- **Docker**

## Project Layout

- **`src/main`** – application source code
- **`src/test`** – tests
- **`pom.xml`** – Maven build configuration
- **`Dockerfile`** – container build instructions
- **`mvnw` / `mvnw.cmd`** – Maven wrapper scripts

## Run Locally

From this directory:

```bash
./mvnw spring-boot:run
```

Windows:

```powershell
mvnw.cmd spring-boot:run
```

## Test

```bash
./mvnw test
```

## Container Build

```bash
docker build -t patient-service:local .
```

## Engineering Standards

- Keep controller, service, and persistence concerns separated
- Add/maintain tests for each feature change
- Document endpoint changes in `../api-requests/patient-service`
