# App-Development-with-Backstage
onboard services onto the platform using developer portals with Backstage plugins 


# Architectural Flow Overview

The diagram (flow chart) below represents the automated "Golden Path" for provisioning new microservices from inception to production.


```text
[Backstage Portal Template]
     | (Developer triggers "New Microservice")
     ▼
[GitHub Repository]
     | (Contains app code, Dockerfile, & Terraform)
     ▼
[GitHub Actions / Azure Pipeline]
     | ──► Runs Security Scan (CodeQL / Trivy)
     | ──► Deploys Azure Infrastructure (via Terraform)
     ▼
[Azure Kubernetes Service (AKS)]
```


