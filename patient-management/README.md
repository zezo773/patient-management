# patient-management Directory

This directory hosts the core workspace for the Patient Management project.

## Contents

- **`patient-service/`** – Java backend service implementation
- **`api-requests/`** – ready-to-use HTTP request files for endpoint testing
- **`.gitignore`** – repository ignore rules for this workspace

## Purpose

This layer separates the project’s runnable backend service from API testing assets, keeping implementation and validation workflows clean and maintainable.

## Recommended Workflow

1. Implement service changes in `patient-service`
2. Validate behavior with request files in `api-requests`
3. Keep request payloads and URLs aligned with service contracts
