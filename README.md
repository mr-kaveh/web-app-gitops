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
# web-app-gitops
