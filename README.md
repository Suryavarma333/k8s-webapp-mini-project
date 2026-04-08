# k8s-webapp-mini-project
Kubernetes mini project using Namespace, Deployment, Service, ConfigMap, Secret and PVC

# Kubernetes Mini Project – Simple Web App Deployment

## Project Overview
This is a Kubernetes mini project where I deployed a simple nginx-based web application using core Kubernetes objects.

The goal of this project is to practice and demonstrate real Kubernetes resource usage in a structured DevOps workflow.

---

## Kubernetes Resources Used

- Namespace
- ConfigMap
- Secret
- PersistentVolume (PV)
- PersistentVolumeClaim (PVC)
- Deployment
- Service (NodePort)

---

## Project Architecture

The application is deployed inside a dedicated namespace called:

project-dev

### Components:
- **Namespace** → isolates project resources
- **ConfigMap** → stores non-sensitive environment variables
- **Secret** → stores sensitive values like DB credentials
- **PV/PVC** → provides persistent storage
- **Deployment** → runs the nginx web application
- **Service** → exposes the application using NodePort

---

## Files in this Project

- `namespace.yaml`
- `configmap.yaml`
- `secret.yaml`
- `pv.yaml`
- `pvc.yaml`
- `deployment.yaml`
- `service.yaml`

---

## Deployment Steps

### 1. Create Namespace
```bash
kubectl apply -f namespace.yaml
