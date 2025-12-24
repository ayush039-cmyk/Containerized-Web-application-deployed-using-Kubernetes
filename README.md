# Containerized-Web-application-deployed-using-Kubernetes
Project Overview

    Complete DevOps pipeline from frontend code to Kubernetes deployment

    Amazon frontend clone deployed on Minikube Kubernetes cluster

    Demonstrates Docker containerization, Kubernetes orchestration, and local development workflow

    
 Features

    Dockerized frontend application

    Kubernetes Deployment with rolling updates capability

    Service exposure via NodePort (port 30080)

    ReplicaSet for high availability (3 replicas)

    Local development environment using Minikube

    Complete YAML configurations for all K8s resources

    Frontend:    HTML5, CSS3, JavaScript
    Container:   Docker
    Orchestration: Kubernetes (Minikube)
    Manifests:   YAML
    Registry:    Docker Hub

    # Clone the project to your local machine
    (https://github.com/ayush039-cmyk/Containerized-Web-application-deployed-using-Kubernetes.git)

# Pull Docker Image from DockerHub
docker run dockerayus039/myfirstimage


# Build the Docker image from Dockerfile
docker build -t yourusername/amazon-clone:latest .

# Steps for Minikube deployment
minikube start --driver=virtualbox (or docker if you prefer)
// To pod
kubectl create -f pod-definition.yml

//To Run ReplicaSet
kubectl create -f replicaset-definition.yml

//To Deploy
kubectl create -f deployment-definition.yml

//To Start service
kubectl create -f service-definition.yml

//To Check IP of the running containter
minikube service myapp --url

