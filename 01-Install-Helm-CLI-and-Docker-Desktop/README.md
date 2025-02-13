# Install Docker Desktop and HELM CLI
## Step-01: Introduction
  1. Install Docker Desktop
  2. Install Helm CLI on local desktop

## Step-02: Docker Desktop - Pricing, SignUp, Download
  [Docker Desktop Pricing](https://www.docker.com/pricing/)
  [Docker Hub SignUp](https://hub.docker.com/)
  [Download Docker Desktop](https://www.docker.com/products/docker-desktop/)

## Step-03: Install Docker Desktop
## Step-03-01: MACOS: Install Docker Desktop
# Install Docker Desktop
    Copy Docker dmg to Applications folder

    # Create Docker Hub Account
    https://hub.docker.com

    # Signin Docker Desktop 
    Open Docker Desktop and SignIn to Docker Hub

## Step-03-02: WINDOWS: Install Docker Desktop
# Download Docker Desktop
    https://www.docker.com/products/docker-desktop/

    # Install Docker Desktop on Windows
        Run the "Docker Desktop Installer.exe"

    # Create Docker Hub Account
    https://hub.docker.com

    # Signin Docker Desktop 
    Open Docker Desktop and SignIn to Docker Hub

    # Configure kubectl cli on Windows PATH
    C:\Program Files\Docker\Docker\Resources\bin

## Step-04: Enable Kubernetes Cluster
    Additional Reference: [Docker Desktop - k8s Cluster](https://docs.docker.com/desktop/features/kubernetes/)

## Step-05: Configure kubeconfig for kubectl for Docker Desktop k8s Cluster

# Verify if kubectl installed (Docker desktop should install kubectl automatically)
    which kubectl

    # Verify kubectl version
    kubectl version 
    kubectl version --short
    kubectl version --client --output=yaml

    # List Config Contexts
    kubectl config get-contexts

    # Config Current Context
    kubectl config current-context

    # Config Use Context (Only if someother context is present in current-context output)
    kubectl config use-context docker-desktop

    # List Kubernetes Nodes
    kubectl get nodes

## Step-06: Verify if our k8s Cluster is functional with a Sample Application




