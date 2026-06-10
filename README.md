# ArgoCD GitOps Platform

## Project Overview

This repository demonstrates a production-style GitOps workflow using ArgoCD and Kubernetes.

ArgoCD is deployed to a Kubernetes cluster and configured to continuously monitor the Git repository containing Kubernetes manifests. Any changes pushed to the repository are automatically reconciled by ArgoCD, keeping the cluster state aligned with the declared infrastructure and application configuration.

The project highlights:
- automated deployments with ArgoCD
- GitOps-driven application delivery
- Kubernetes application lifecycle management
- infrastructure-as-code best practices

## Repository Structure

- `manifests/` - Kubernetes manifests for the sample application and ArgoCD configuration
- `screenshots/` - visual artifacts documenting the deployment, login, sync, and validation stages

## Screenshots

The `screenshots/` folder contains visual documentation for the ArgoCD workflow. Each image is sized for effective display on GitHub.

<table>
  <tr>
    <td align="center"><img src="screenshots/01-project-structure.png" width="280" alt="Project structure"><br><strong>01</strong> Project structure</td>
    <td align="center"><img src="screenshots/02-minikube-running.png" width="280" alt="Minikube status"><br><strong>02</strong> Minikube status</td>
    <td align="center"><img src="screenshots/03-argocd-namespace.png" width="280" alt="ArgoCD namespace"><br><strong>03</strong> ArgoCD namespace</td>
  </tr>
  <tr>
    <td align="center"><img src="screenshots/04-argocd-pods-running.png" width="280" alt="ArgoCD pods running"><br><strong>04</strong> ArgoCD pods</td>
    <td align="center"><img src="screenshots/05-argocd-namespace-details.png" width="280" alt="Namespace details"><br><strong>05</strong> Namespace details</td>
    <td align="center"><img src="screenshots/06-argocd-login.png" width="280" alt="ArgoCD login"><br><strong>06</strong> ArgoCD login</td>
  </tr>
  <tr>
    <td align="center"><img src="screenshots/07-argocd-dashboard.png" width="280" alt="ArgoCD dashboard"><br><strong>07</strong> ArgoCD dashboard</td>
    <td align="center"><img src="screenshots/08-app-created.png" width="280" alt="Application created"><br><strong>08</strong> Application created</td>
    <td align="center"><img src="screenshots/09-app-created-details.png" width="280" alt="Application details"><br><strong>09</strong> Application details</td>
  </tr>
  <tr>
    <td align="center"><img src="screenshots/10-sync-success.png" width="280" alt="Sync success"><br><strong>10</strong> Sync success</td>
    <td align="center"><img src="screenshots/11-production-pods.png" width="280" alt="Production pods"><br><strong>11</strong> Production pods</td>
    <td align="center"><img src="screenshots/12-browser-validation.png" width="280" alt="Browser validation"><br><strong>12</strong> Browser validation</td>
  </tr>
</table>

## Usage

1. Deploy ArgoCD to a Kubernetes cluster.
2. Connect ArgoCD to this Git repository.
3. Create and synchronize the application from the ArgoCD dashboard.
4. Verify the application deployment and pod status in Kubernetes.

This README is intentionally concise and focused on the project deliverables. No personal or sensitive information is included.