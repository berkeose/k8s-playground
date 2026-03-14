# kubectl Commands Cheat Sheet

## Cluster Information

```bash
kubectl cluster-info
kubectl get nodes
kubectl get namespaces

Pod Commands
kubectl get pods
kubectl get pods -o wide
kubectl describe pod <pod-name>
kubectl logs <pod-name>
kubectl delete pod <pod-name>

Apply and Delete Resources
kubectl apply -f <file>.yaml
kubectl delete -f <file>.yaml

Output Formats
kubectl get pods -o yaml
kubectl get pods -o json

kubectl-commands.md
```md
# File: README.md

## Skills Practiced

- Kubernetes fundamentals
- kubectl usage
- YAML manifest writing
- local cluster management
- workload inspection and debugging
- technical note-taking

'''
