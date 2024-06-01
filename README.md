# K8s-K9s


- minikube tunnel=> access port inside cluster


Install K9s 


-> k9s
show pods in default 

- ?: show all helps
- :svc => show all services
- :deploy => show all deployments
- :pods => show all pods
- d: describe a Pods
- s: go to shell of the pods
- l: logs the pod
- ctrl + k: Kill, but if it has replias, it will automatically revive
- shift + f: forward port => f shows all forward ports of the pod, ctrl + d on the port will delete

## Cluster:

A Kubernetes cluster is a set of nodes (machines) that run containerized applications. Minikube creates a single-node cluster on your local machine for development and testing purposes.
Nodes:

## Nodes
are the individual machines (virtual or physical) that make up the cluster. Each node runs pods and is managed by the master node.

## Namespace:

Namespaces are a way to divide cluster resources between multiple users or applications. They provide a scope for names within the cluster. You can think of namespaces as virtual clusters within your cluster.
## Pod:

A pod is the smallest and simplest Kubernetes object. It represents a single instance of a running process in your cluster. Pods can contain one or more containers (usually one).
## Service:

Services in Kubernetes are used to expose your pods to the network. They provide stable IP addresses and DNS names for pods, allowing them to be accessed consistently.
## Deployment:

Deployments manage the deployment and scaling of a set of pods. They ensure that the desired number of pods are running and handle updates to the pods' container images.
## ReplicaSet:

A ReplicaSet ensures that a specified number of pod replicas are running at any given time. Deployments use ReplicaSets to manage pod scaling.
## StatefulSet:

StatefulSets are used for applications that require stable, persistent storage and unique network identifiers, such as databases.
## DaemonSet:

A DaemonSet ensures that all (or some) nodes run a copy of a pod. They are typically used for logging, monitoring, or other node-specific tasks.
## Job and CronJob:

Jobs create one or more pods and ensure that a specified number of them successfully terminate. CronJobs manage time-based jobs, similar to cron jobs in Linux.
## ConfigMap and Secret:

ConfigMaps are used to pass configuration data to pods. Secrets are used to manage sensitive information, such as passwords and API keys, securely.
## PersistentVolume (PV) and PersistentVolumeClaim (PVC):

PVs are storage resources in the cluster, and PVCs are requests for storage by users. They abstract the underlying storage systems and allow for persistent storage for pods.
## Ingress:

Ingress manages external access to the services in your cluster, typically HTTP and HTTPS. It provides load balancing, SSL termination, and name-based virtual hosting.
