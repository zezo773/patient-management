# Main Application Source (`src/main`)

Production code for the patient-service application lives here.

## Typical Contents

- Java application classes
- Spring configuration
- Domain models
- Service layer logic
- Persistence/repository layer
- Runtime resources (e.g., `application.yml` / `application.properties`)

## Standards

- Follow clear package boundaries (controller/service/repository/domain)
- Keep business rules in service/domain layers, not controllers
- Validate inputs consistently and return meaningful API responses
