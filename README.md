# Strataform

Strataform is a streaming data platform project

## Prerequisites

Strataform has prerequisites on the following components, which need to be configured in the Kubernetes cluster:

- A Kubernetes (EKS) v1.18+ cluster with 5 nodes.
- [Cert-manager](https://cert-manager.io) installed in the cluster.

### Deploy a Kubernetes cluster

Run the following commands to deploy a Kubernetes (EKS) cluster into AWS:

```shell
eksctl create cluster -f cluster/development.yaml
```

### Install cert-manager

We'll follow the official [instructions](https://cert-manager.io/docs/installation/kubernetes/) to install cert-manager:

```shell
kubectl apply -f https://github.com/jetstack/cert-manager/releases/download/v1.1.0/cert-manager.yaml
```

