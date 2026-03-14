# Cluster Architecture

## What is a Kubernetes Cluster?

A Kubernetes cluster is a group of machines working together to run containerized applications.

A cluster usually consists of:

- control plane
- worker nodes

## Control Plane

The control plane is the brain of Kubernetes.

It makes decisions about the cluster, such as:

- scheduling Pods
- keeping track of cluster state
- responding when something fails

### Main Control Plane Components

#### API Server
The main entry point for Kubernetes.  
Commands like `kubectl apply` communicate with the API server.

#### etcd
The key-value store where Kubernetes keeps cluster state and configuration data.

#### Scheduler
Decides on which worker node a new Pod should run.

#### Controller Manager
Runs controllers that watch the cluster state and try to keep it aligned with the desired state.

## Worker Nodes

Worker nodes are the machines where application workloads actually run.

Each worker node typically includes:

- kubelet
- container runtime
- kube-proxy

### kubelet
The agent running on each worker node.  
It communicates with the control plane and makes sure Pods are running as expected.

### container runtime
Responsible for running containers.  
Examples include containerd.

### kube-proxy
Helps manage networking and traffic routing for Services.

## High-Level Flow

1. user applies a YAML file
2. API server receives the request
3. scheduler chooses a node
4. kubelet on that node starts the Pod
5. Kubernetes keeps checking whether the desired state is still true

## My Understanding

The control plane decides.  
The worker nodes execute.

So I can think of Kubernetes as a management layer where the control plane acts like the coordinator and the worker nodes do the actual application work.
