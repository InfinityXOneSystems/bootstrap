# Infinity Platform Validator

This repository contains the `platform-validator.ps1` PowerShell script, designed to validate the Infinity XOS platform. It includes functionalities for validating Python code, patching health endpoints for FastAPI applications, and healing missing directory structures.

## Features

- **Python Code Validation**: Checks Python files for compilation errors.
- **FastAPI Health Endpoint Patching**: Automatically adds `/health` and `/ready` endpoints to FastAPI applications if they are missing.
- **Directory Healing**: Creates essential directory structures like `services`, `services/agents`, `services/memory`, `.github`, and `.github/workflows` if they do not exist.

## Usage

The script can be run with different modes:

```powershell
./platform-validator.ps1 -Mode validate
./platform-validator.ps1 -Mode patch
./platform-validator.ps1 -Mode heal
./platform-validator.ps1 -Mode full
```

- `validate`: Only performs Python code validation.
- `patch`: Only patches FastAPI health endpoints.
- `heal`: Only heals missing directory structures.
- `full`: Performs all validation, patching, and healing operations.

## Development

### Prerequisites

- PowerShell
- Python 3.x (for Python code validation)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
