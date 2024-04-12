# Reddit Clone App on Multinode Kubernetes Cluster 
This project demonstrates how to deploy a Reddit clone app on Kubernetes and expose it to the world using Minikube as the cluster.

## Prerequisites
Before you begin, you should have the following tools installed on your local machine: 

- Docker
- Kubeadm master and worker node
- kubectl
- Git

## Installation
Follow these steps to install and run the Reddit clone app on your local machine:

1) Clone this repository to your local machine: `git clone https://github.com/harsh2478/reddit-clone-k8s.git`
2) Navigate to the project directory: `cd reddit-clone-k8s`
3) Build the Docker image for the Reddit clone app: `docker build -t reddit-clone-app .`
4) Clone the maifest repository : `git clone https://github.com/harsh2478/reddit-clone-k8s-manifests.git`
5) Navigate to this repository : cd `reddit-clone-k8s-manifests`
6) Deploy the app to Kubernetes: `kubectl apply -f deployment.yaml`
7) Deploy the Service for deployment to Kubernetes: `kubectl apply -f service.yaml`

## Automate With Jenkins
Follow these steps to create the ci/cd pipeline for automating this deployment.

1) Follow each step in this blog to set up a jenkins pipeline : 'https://harsh05.medium.com/streamlining-ci-cd-for-deploying-reddit-clone-on-a-multinode-kubernetes-cluster-51d5528c2c19' 



