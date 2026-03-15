# Lab 03 — Labels and Selectors

## Goal

Understand how labels are attached to Pods and how selectors can be used to filter them.

## What I Will Practice

- creating a Pod with labels
- listing labels with kubectl
- filtering Pods using selectors

## Useful Commands

Show labels:

`kubectl get pods --show-labels`

Filter Pods by label:

`kubectl get pods -l app=nginx`

Describe a Pod:

`kubectl describe pod nginx-label-pod`

Delete the Pod:

`kubectl delete -f pod-with-labels.yaml`

## What This Lab Teaches

- how labels are defined in YAML
- how selectors work in practice
- how Kubernetes groups resources using labels

## My Understanding

This lab shows that labels are not just extra metadata.

They are used by Kubernetes to connect and organize resources in a practical way.
