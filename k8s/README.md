# Kubernetes Manifests

This directory contains Kubernetes configuration files for deploying the HTTP/3 application.

## Structure

```
k8s/
├── manifests/      # Kubernetes YAML files
│   ├── deployment.yaml
│   ├── service.yaml
│   └── ingress.yaml
├── helm/          # Helm charts (if used)
└── README.md
```

## Usage

Apply manifests to your Kubernetes cluster:

```bash
kubectl apply -f k8s/manifests/
```

## Security Note

**Never commit secrets or credentials!** 
- Use Kubernetes Secrets
- Use environment-specific configuration
- Keep sensitive data out of version control

## Getting Started

1. Set up a local Kubernetes cluster (minikube or kind)
2. Create deployment manifests
3. Configure services and networking
4. Test HTTP/3 connectivity
