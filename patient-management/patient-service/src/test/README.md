# Test Source (`src/test`)

Automated tests for patient-service.

## Purpose

Ensure correctness, reliability, and safe refactoring of the patient-service codebase.

## Test Strategy

- Unit tests for core business logic
- Integration tests for Spring components and API behavior
- Regression tests for fixed bugs

## Execution

Run from `patient-service` root:

```bash
./mvnw test
```

## Best Practices

- Name tests clearly around behavior
- Arrange test data for readability
- Keep tests deterministic and isolated
