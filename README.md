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
