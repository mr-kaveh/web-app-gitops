# GitOps Example Project with Helm and Argo CD

This repository demonstrates a simple GitOps project using Helm and Argo CD to manage a Kubernetes application.

## Directory Structure

- `argo-cd/`: Directory containing the Argo CD Application manifest.
  - `argo-application.yaml`: Argo CD Application manifest.
- `helm-chart/`: Directory containing the Helm chart for the application.
  - `Chart.yaml`: Helm chart metadata file.
  - `templates/`: Directory containing Kubernetes resource templates for the Helm chart.
    - `deployment.yaml`: Kubernetes Deployment template.
    - `service.yaml`: Kubernetes Service template.
  - `values.yaml`: Default configuration values for the Helm chart.

## Setup Instructions

1. Clone this repository to your local machine:

   ```sh
   git clone https://github.com/your-username/your-repo.git
   cd your-repo

Apply the Argo CD Application manifest:


    kubectl apply -f argo-cd/argo-application.yaml

Argo CD will automatically synchronize the Kubernetes cluster with the desired state defined in the helm-chart directory.

Access the Argo CD web UI to monitor the synchronization process:

    kubectl port-forward svc/argocd-server -n argocd 8080:443
