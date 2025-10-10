# Chama App GitOps Repository

This repository contains Kubernetes manifests for deploying the Chama application using ArgoCD.

## Structure

- `apps/base/` - Base application manifests
- `apps/staging/` - Staging environment overlays
- `apps/production/` - Production environment overlays
- `infrastructure/` - Infrastructure resources
- `argo-apps/` - ArgoCD Application definitions

## Deployment

ArgoCD automatically syncs:
- Staging: Automated sync from `apps/staging/`
- Production: Manual sync from `apps/production/`
