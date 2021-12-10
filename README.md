# Local K8s

This repo defines a set of resources for running services inside a local K8s
cluster. Some options are:

- minikube - https://minikube.sigs.k8s.io/docs/
- Rancher Desktop - https://rancherdesktop.io/
- Docker Desktop - https://www.docker.com/products/kubernetes
- K3s - https://k3s.io/

This specific configuration has only been tested on the Mac version of 
Rancher Desktop 

## Setup

- install rancher desktop. Select the correct release for your OS from the
  releases page. https://github.com/rancher-sandbox/rancher-desktop/releases
- install helmfile - https://github.com/roboll/helmfile#installation
- ensure the rancher Desktop cluster is running and the correct context is
  selected.
  ```
  kubectl config use rancher-desktop
  ```
- apply the charts using helmfile - `helmfile apply`
