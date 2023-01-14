# 🐳 Kubernetes Course 🐳
This repository contains the set of artifacts created by doing the course [Kubernetes Hands-On - Deploy Microservices to the AWS Cloud](https://www.udemy.com/course/kubernetes-microservices/).

## Overview
Kubernetes (K8s) is an open source product used to automate deploying, scaling, and managing containerized applications.

My goal is learn Kubernetes to apply on my job delivering new microservices more efficiently. This Readme file will be a notebook with a lot of annotations.

### Pod
- Pod is a wrapper for a Docker container.
- Pod controls the container making sure it is running and healthy, monitoring hardware resources like CPU, memory and storage.
- **Pods aren't visible outside the cluster.**
- Pods are volatile. They are stoping and starting all the time.

### Service
- Service gives to Pods an external IP address.
- There are 3 types: Cluster IP, Node Port and Load Balancer.
  - Cluster IP: only visible inside the cluster.
  - Node Port: exposes a port throught the Node/Cluster.
  - Load Balancer: *I don't know yet...*

![image](https://user-images.githubusercontent.com/31314944/207205834-8ea36aec-d093-4d52-b329-4992fe6749a9.png)

### Replica set
- Replica sets can manage a group of identical pods at any time;
- One interisting feature is the min pod definition. When 2 replicas is defined, the replica set will detected and recreate dead pods.

### Deployments
- Deployments is a type of replica set versioning;
- When a new deployment is made, a new replica set will be created. When the new one is responding the requests (or is healthy) the old one will have the replica number replaced to 0;
- Is possible to make rollbacks to old replica sets easily.
