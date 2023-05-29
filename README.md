# jira_minikube
An attempt to run JIRA on local k8s cluster

## Prerequesites

- HELM
- PV
- Deployment
    - ???
- Service
- Ingress

## Deploy

### PV

Persistence Volume

### HELM

    1. Add repo:
        ```bash
        helm repo add atlassian-data-center https://atlassian.github.io/data-center-helm-charts
        ```
    2. Install helm chart:
        ```bash
        helm install jira813 atlassian-data-center/jira --namespace jira --create-namespace --version 1.12.0 --values values.yaml
        ```