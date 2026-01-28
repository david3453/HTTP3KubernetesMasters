# Scripts

This directory contains utility scripts for development, testing, and deployment.

## Common Scripts

Add scripts here for:
- Building Docker images
- Deploying to Kubernetes
- Running benchmarks
- Automating tests
- Data collection

## Platform Compatibility

When writing scripts:
- Use `#!/usr/bin/env bash` for Bash scripts (cross-platform)
- Test on both Windows (Git Bash/WSL) and Linux/macOS
- Consider creating both `.sh` and `.ps1` versions for Windows PowerShell if needed

## Example

```bash
#!/usr/bin/env bash
# build.sh - Build Docker image

docker build -t http3-server:latest ./src/server
```
