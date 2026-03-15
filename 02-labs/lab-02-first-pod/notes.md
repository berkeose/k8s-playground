# Lab 02 — First Pod

## Goal

Create the first Pod using a YAML manifest and inspect it with kubectl.

## YAML File

The Pod manifest is stored in: `pod.yaml`

## Apply the Manifest

`kubectl apply -f pod.yaml`

## Useful Commands

Check Pods:

`kubectl get pods`

Detailed Pod information:

`kubectl describe pod nginx-pod`

See logs:

`kubectl logs nginx-pod`

Delete Pod:

`kubectl delete -f pod.yaml`

## What This Lab Teaches

- how a basic Pod manifest looks
- how to create a Pod with YAML
- how to inspect Pod state
- how Kubernetes tracks a running workload

## My Understanding

This lab helped me understand that Kubernetes resources are usually created declaratively with YAML.

Instead of manually starting a container, I define a Pod object and apply it to the cluster.
