{
  "name": "Custom DevOps Container",
  "build": {
    "dockerfile": "Dockerfile"
  },
  "features": {
    "ghcr.io/devcontainers/features/docker-in-docker:2": {}
  }
}
FROM mcr.microsoft.com/devcontainers/javascript-node:20

# Install extra tools
RUN apt-get update && apt-get install -y \
    kubectl \
    helm \
    jq \
    && rm -rf /var/lib/apt/lists/*
