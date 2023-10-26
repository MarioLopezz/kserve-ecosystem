# kserve-ecosystem

This repository houses Kubernetes YAML manifests to set up and deploy essential components forming part of the kserve ecosystem.

## Components included:

- **Istio**: A service mesh providing traffic routing, load balancing, and security policies for services in Kubernetes.
- **Kiali**: A user interface for observing the behavior of the Istio service mesh. It offers a detailed visual view of your architecture and how different microservices interact with each other.
- **Knative**: A Kubernetes platform for building, deploying, and managing modern serverless applications.
- **Kserve**: An extension of Knative providing machine learning model inference capabilities on Kubernetes.

## Installation Instructions

1. Clone this repository:
    ```bash
    git clone https://github.com/[your_username]/kserve-ecosystem.git
    cd kserve-ecosystem
    ```

2. Apply the manifests in the appropriate order:
    ```bash
    kubectl apply -f istio/
    kubectl apply -f kiali/
    kubectl apply -f knative/
    kubectl apply -f kserve/
    ```
