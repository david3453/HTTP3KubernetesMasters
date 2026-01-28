# Contributing to HTTP3 Kubernetes Masters Thesis

## Development Environment Setup

This project is designed to work seamlessly across different platforms, including Windows and Linux/macOS.

### Prerequisites

- Git configured on your machine
- Docker (for containerization)
- Kubernetes cluster access (minikube, kind, or cloud provider)
- Your preferred IDE or text editor

### Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/david3453/HTTP3KubernetesMasters.git
   cd HTTP3KubernetesMasters
   ```

2. The repository uses `.editorconfig` to maintain consistent code formatting across different editors. Most modern IDEs support this automatically.

3. Create a new branch for your work:
   ```bash
   git checkout -b feature/your-feature-name
   ```

### Platform-Specific Notes

#### Windows Development
- Use Git Bash, PowerShell, or WSL2 for command-line operations
- WSL2 is recommended for Docker and Kubernetes development
- Ensure line endings are handled correctly (configured via `.editorconfig`)

#### Linux/macOS Development
- Standard terminal should work for all operations
- Ensure Docker and kubectl are properly installed

### Code Style

- Follow the `.editorconfig` settings for consistent formatting
- Use meaningful commit messages
- Keep commits atomic and focused

### Committing Changes

1. Stage your changes:
   ```bash
   git add .
   ```

2. Commit with a descriptive message:
   ```bash
   git commit -m "Brief description of changes"
   ```

3. Push to your branch:
   ```bash
   git push origin feature/your-feature-name
   ```

### File Organization

- Keep configuration files in `/config` or `/k8s` directories
- Keep source code organized by component
- Document any platform-specific requirements

## Questions?

For questions or issues with the development environment setup, please create an issue in the repository.
