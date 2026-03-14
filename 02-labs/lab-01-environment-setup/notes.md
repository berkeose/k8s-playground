
# Lab 01 — Environment Setup

## Goal

Prepare the local machine for Kubernetes practice.

## Tools Planned

- kubectl
- minikube
- Docker Desktop

## Why This Setup?

This setup is enough for beginner and intermediate Kubernetes practice on a local machine.

- `kubectl` is needed to talk to the cluster
- `minikube` provides a local Kubernetes cluster
- Docker Desktop helps provide the container environment

## Commands to Verify Later

```bash
kubectl version --client
minikube version
docker version

Expected Outcome

After setup is complete, I should be able to:
	•	start a local Kubernetes cluster
	•	check cluster status
	•	list nodes
	•	apply YAML manifests

Personal Notes

This lab is the foundation of the entire repository.
If the environment is clean and stable, the rest of the practice becomes much easier.
```text
# Terminal Commands to Run on Mac

brew install kubectl
brew install minikube

kubectl version --client
minikube version

minikube start

kubectl get nodes
kubectl get pods -A



minikube start

kubectl get nodes
kubectl get pods -A


