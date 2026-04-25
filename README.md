# Kubernetes README

## Overview
This project contains basic Kubernetes YAML files and commands for deploying applications in a Kubernetes cluster.

## Files Included
- pod.yml
- deployment.yml
- service.yml
- replicaset.yml
- namespace.yml
- configmap.yml
- secret.yml
- ingress.yml

## Kubernetes Objects

### Pod
Smallest deployable unit in Kubernetes.

### Deployment
Used to manage pods and rolling updates.

### Service
Used to expose applications inside or outside the cluster.

### ReplicaSet
Maintains the required number of pod replicas.

### Namespace
Used to separate resources logically.

### ConfigMap
Stores non-sensitive configuration data.

### Secret
Stores sensitive data like passwords.

### Ingress
Used to manage external access to services.

## Basic Commands

### Apply YAML Files

```bash
kubectl apply -f pod.yml
kubectl apply -f deployment.yml
kubectl apply -f service.yml
Check Resources
kubectl get pods
kubectl get deployments
kubectl get svc
kubectl get all
Describe Resource
kubectl describe pod pod-name
Delete Resource
kubectl delete -f deployment.yml
Logs
kubectl logs pod-name
Exec into Pod
kubectl exec -it pod-name -- /bin/bash
Deployment Strategies
Recreate
Rolling Update
Blue-Green
Canary
