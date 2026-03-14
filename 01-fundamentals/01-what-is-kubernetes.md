# What is Kubernetes?

## Definition

Kubernetes is a container orchestration platform used to deploy, manage, scale, and monitor containerized applications.

In simple terms, Docker helps run containers, while Kubernetes helps manage many containers in a more automated and organized way.

## Why Kubernetes Exists

Running a single container manually is easy.  
But in real environments, things become more complex:

- applications may need multiple containers
- containers may crash and need automatic restart
- traffic must be distributed across replicas
- updates should happen with minimal downtime
- applications must scale when demand increases

Kubernetes solves these kinds of operational problems.

## Main Idea

Kubernetes provides a system where you describe the desired state of your application, and Kubernetes works to keep the environment matching that state.

Example:

- you say: "I want 3 replicas of this application"
- Kubernetes tries to keep 3 replicas running
- if one fails, Kubernetes starts another one

## Key Benefits

- automatic restart of failed workloads
- scaling applications
- service discovery
- rolling updates
- declarative management using YAML
- better organization for containerized systems

## Docker vs Kubernetes

Docker:
- runs containers

Kubernetes:
- manages containerized applications at a larger scale

So Kubernetes does not replace containers.  
It manages them more effectively.

## My Understanding

My understanding so far is:

Kubernetes is the system that sits above containers and helps operate them reliably.  
Instead of manually starting and managing containers one by one, I define what I want, and Kubernetes tries to keep the system in that desired state.
