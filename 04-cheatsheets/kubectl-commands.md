# kubectl Commands Cheat Sheet

## Cluster Information

`kubectl cluster-info`  
`kubectl get nodes`  
`kubectl get namespaces`

## Pod Commands

`kubectl get pods`  
`kubectl get pods -o wide`  
`kubectl describe pod <pod-name>`  
`kubectl logs <pod-name>`  
`kubectl delete pod <pod-name>`

## Apply and Delete Resources

`kubectl apply -f <file>.yaml`  
`kubectl delete -f <file>.yaml`

## Output Formats

`kubectl get pods -o yaml`  
`kubectl get pods -o json`

## Helpful Tip

`kubectl describe` is useful when a resource is created but not working as expected.  
It often shows events and scheduling-related errors.
