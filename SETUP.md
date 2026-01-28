# Development Setup Guide

## Cross-Platform Repository Setup

This guide helps you set up the HTTP/3 Kubernetes Masters thesis project on any platform.

## Prerequisites

### All Platforms
- Git (latest version)
- Text editor or IDE of your choice
- Docker Desktop (for containerization)
- kubectl (Kubernetes command-line tool)

### Installation Links

#### Git
- **Windows**: Download from https://git-scm.com/download/win
- **macOS**: `brew install git` or download from https://git-scm.com/download/mac
- **Linux**: `sudo apt-get install git` (Debian/Ubuntu) or `sudo yum install git` (RHEL/CentOS)

#### Docker
- **Windows/macOS**: Docker Desktop from https://www.docker.com/products/docker-desktop
- **Linux**: Follow instructions at https://docs.docker.com/engine/install/

#### kubectl
- All platforms: https://kubernetes.io/docs/tasks/tools/

## First-Time Setup

### 1. Clone the Repository

```bash
git clone https://github.com/david3453/HTTP3KubernetesMasters.git
cd HTTP3KubernetesMasters
```

### 2. Configure Git (One-time setup)

```bash
# Set your identity
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"

# Windows users: Configure line endings
git config --global core.autocrlf true

# Linux/macOS users: Configure line endings
git config --global core.autocrlf input
```

### 3. Verify Setup

```bash
git status
```

## Working Across Multiple Devices

### Syncing Changes

**On your first device (e.g., Windows laptop):**
```bash
# Make changes to your files
git add .
git commit -m "Describe your changes"
git push origin main
```

**On your second device (e.g., stationary PC):**
```bash
# Pull the latest changes
git pull origin main

# Continue working...
```

### Best Practices

1. **Always pull before you start working:**
   ```bash
   git pull origin main
   ```

2. **Commit frequently with meaningful messages:**
   ```bash
   git add .
   git commit -m "Added HTTP/3 server implementation"
   ```

3. **Push your changes when done:**
   ```bash
   git push origin main
   ```

4. **Use branches for experimental work:**
   ```bash
   git checkout -b experiment/new-feature
   # Work on your feature
   git push origin experiment/new-feature
   ```

## Platform-Specific Tips

### Windows
- **Recommended**: Use Windows Subsystem for Linux (WSL2) for Docker and Kubernetes
- **Alternative**: Git Bash or PowerShell for Git operations
- Line endings are automatically handled by Git configuration

### Linux/macOS
- Use the native terminal
- All commands work directly without modification

## IDE/Editor Support

The project includes `.editorconfig` which is supported by:
- Visual Studio Code (with EditorConfig extension)
- IntelliJ IDEA / PyCharm
- Sublime Text
- Atom
- Vim (with plugin)

## Troubleshooting

### Issue: Line Ending Problems
**Solution**: Ensure Git is configured correctly (see step 2 above)

### Issue: Permission Denied
**Solution**: Set up SSH keys for GitHub or use HTTPS with credentials

### Issue: Merge Conflicts
**Solution**: 
```bash
git pull origin main
# Resolve conflicts in your editor
git add .
git commit -m "Resolved merge conflicts"
git push origin main
```

## Additional Resources

- [Git Documentation](https://git-scm.com/doc)
- [Docker Documentation](https://docs.docker.com/)
- [Kubernetes Documentation](https://kubernetes.io/docs/home/)

## Next Steps

Once your environment is set up:
1. Review the project structure
2. Read through existing documentation
3. Start implementing your thesis components
4. Document your work as you go

Happy coding!
