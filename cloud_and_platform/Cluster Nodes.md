## Cluster

A cluster is a group of nodes working together.

The cluster provides the infrastructure where applications run. Inside the cluster, there are different types of nodes, and the cluster hosts all pods and containers.

---

## Node

A node is a worker machine inside a cluster.

Nodes provide the resources required to run workloads, such as:

- CPU
- Memory (RAM)
- Storage
- Network connectivity

A node runs one or more pods.

---

## Pod

A pod is the smallest deployable unit in Kubernetes.

A pod is a wrapper around one or more containers that share:

- Network
- Storage
- Configuration

Pods do not run directly on the cluster; they run on nodes.

---

## Container

A container is the running instance of an image.

When a container runtime (such as containerd or CRI-O) receives instructions to start an image, it creates a container from that image.

Example:

Image → Container

```text
nginx:latest
        │
        ▼
Running Container