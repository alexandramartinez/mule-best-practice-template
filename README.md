# Mule Best Practice Template

A Mule 4 application template demonstrating best practices for configuration management and HTTP API development.

## Features

- Environment-specific configuration using YAML files
- HTTP listener with JSON response
- Global configuration management
- Maven-based project structure

## Project Structure

```
src/
├── main/
│   ├── mule/
│   │   ├── global.xml           # Global configurations
│   │   └── mule-best-practice-template.xml  # Main application flow
│   └── resources/
│       ├── local-properties.yaml  # Local environment properties
│       └── dev-properties.yaml    # Development environment properties
└── test/                         # Test resources
```

## Prerequisites

- Mule 4.x Runtime
- Maven 3.6.x or later
- Java 8 or later
- Cursor IDE (Download from [cursor.com](https://cursor.com))
- Anypoint Code Builder (Anypoint Extension Pack)

### Installing Cursor

1. Visit [cursor.com](https://cursor.com)
2. Download the appropriate version for your operating system
3. Follow the installation instructions for your platform:
   - Windows: Run the downloaded .exe file
   - macOS: Drag Cursor to your Applications folder
   - Linux: Extract the downloaded package and run the installer

### Installing Anypoint Code Builder

1. Open Cursor
2. Go to Extensions (Ctrl+Shift+X or Cmd+Shift+X)
3. Search for "Anypoint Extension Pack"
4. Click Install
5. After installation, you'll need to:
   - Sign in to your Anypoint Platform account
   - Configure your Mule runtime
   - Set up your Anypoint Platform credentials

## Configuration

The application uses environment-specific YAML files for configuration:

- `local-properties.yaml`: Local development environment
- `dev-properties.yaml`: Development environment

## Testing the API

Once the application is running, you can test the API endpoint:

```bash
curl http://localhost:8081/hello
```

Expected response:
```json
{
    "message": "hello world"
}
```

## Environment Configuration

The application uses the following environment variables:
- `env`: Specifies the environment (local/dev)

---

*P.S. This README was generated using Cursor too! 🚀* 