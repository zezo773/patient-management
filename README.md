# Patient Management

A professional, production-ready backend workspace for managing patient records and related API workflows.

## Overview

This repository currently contains:

- **`patient-service`**: Java-based backend service (Spring Boot + Maven wrapper)
- **`api-requests`**: HTTP request collections for quickly testing service endpoints

The project is structured so development, testing, and API validation are cleanly separated.

## Repository Structure

```text
patient-management/
├── api-requests/
│   └── patient-service/
└── patient-service/
    ├── src/
    │   ├── main/
    │   └── test/
    ├── Dockerfile
    ├── pom.xml
    ├── mvnw
    └── mvnw.cmd
```

## Quick Start

### 1) Navigate to the service

```bash
cd patient-management/patient-service
```

### 2) Run the application (Maven Wrapper)

```bash
./mvnw spring-boot:run
```

On Windows:

```powershell
mvnw.cmd spring-boot:run
```

### 3) Run tests

```bash
./mvnw test
```

## Docker

A `Dockerfile` is provided in `patient-service` for containerized builds and deployment.

Example build (from `patient-service`):

```bash
docker build -t patient-service:local .
```

## API Testing

Use the `.http` files under `api-requests/patient-service` to test key patient operations:

- create patient
- list patients
- update patient
- delete patient

These request files are ideal for IDE HTTP clients (e.g., IntelliJ HTTP Client, VS Code REST client-compatible workflows).

## Development Notes

- Keep domain and business logic inside `patient-service/src/main`.
- Keep tests mirrored in `patient-service/src/test`.
- Keep endpoint examples in `api-requests` in sync with controller contracts.
- Prefer environment variables for runtime configuration in production.

## Contribution Guidelines

1. Create a feature branch
2. Implement and test changes locally
3. Update request examples and docs as needed
4. Open a pull request with a clear summary

## License

No license file is currently defined for this repository. Add one if you plan to distribute externally.
