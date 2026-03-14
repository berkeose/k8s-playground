# Lab 02 — First Pod

## Goal

Create the first Pod using a YAML manifest and inspect it with kubectl.

## YAML File

The Pod manifest is stored in:

```bash
---

# 9) `02-labs/lab-02-first-pod/pod.yaml`

```yaml
apiVersion: v1
kind: Pod
metadata:
  name: nginx-pod
  labels:
    app: nginx
spec:
  containers:
    - name: nginx-container
      image: nginx:latest
      ports:
        - containerPort: 80
pod.yaml
