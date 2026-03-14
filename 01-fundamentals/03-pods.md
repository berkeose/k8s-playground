# Pods

## What is a Pod?

A Pod is the smallest deployable unit in Kubernetes.

It usually contains one container, but it can also contain multiple tightly coupled containers that need to work together.

## Why Not Just Containers?

In Kubernetes, containers are not usually managed directly.  
Instead, Kubernetes manages Pods.

A Pod provides a shared environment for its containers, including:

- shared network
- shared IP address
- shared ports
- shared storage volumes if defined

## Important Idea

Even if a Pod contains only one container, Kubernetes still wraps that container inside a Pod.

So in Kubernetes, we usually deploy Pods, not raw containers.

## Pod Characteristics

- Pods are relatively temporary
- if a Pod dies, Kubernetes may create a replacement
- Pods can be created manually, but usually higher-level objects like Deployments manage them

## Single-Container Pod

The most common beginner example is a Pod with one container, such as nginx.

## Multi-Container Pod

A Pod may also contain multiple containers when those containers are very closely related.

Example idea:
- main application container
- sidecar container for logging or helper tasks

## Example Use Case

If I want to run a simple nginx container in Kubernetes, I usually create a Pod manifest and apply it to the cluster.

## My Understanding

A Pod is Kubernetes' basic runtime unit.

Instead of thinking "I run a container", in Kubernetes I should think:
"I run a Pod, and that Pod contains one or more containers."

That mental shift is important.
