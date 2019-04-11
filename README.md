# Kubernetes
https://www.udemy.com/learn-kubernetes/

# Overview

 ![Alt Text](https://github.com/duozhanggithub/Kubernetes/blob/master/Kubernets%20architecture.png)

Nodes: A node is a machine, physical or virtual on which Kubernetes is installed. A node is a worker machine and that is where containers will be launched by Kubernetes.

Cluster: a set of nodes grouped together, if one node fails, the application still accessible, multiple nodes also help sharing loads

Master: another node with Kubernetes installed in it and is configured as a Master.The master watches over the nodes in the cluster and is responsible for the actual orchestration of containers on the worker nodes.

# Basic concepts

POD: A pod is a single instance of an application, it is the smallest object that you can create in Kubernetes. Usually have one to one relationship with the containers.

Create Pods using YAML (refer to https://github.com/duozhanggithub/Kubernetes/blob/master/pod-definition.yml)

![Alt Text](https://github.com/duozhanggithub/Kubernetes/blob/master/YAML%20for%20pod.png)

pod-definition.yml: contains four fields, apiVersion, kind, metadata, spec

Replication controller: prevent fail situation, load balancing and scaling
![Alt Text](https://github.com/duozhanggithub/Kubernetes/blob/master/replicationcontroller.png)

Replica set: has different apiVersion, also has selector, use labels to identify which pod to monitor
![Alt Text](https://github.com/duozhanggithub/Kubernetes/blob/master/replicaset.png)

# Minikube

![Alt Text](https://github.com/duozhanggithub/Kubernetes/blob/master/Minikube.png)

# Kubeadm

![Alt Text](https://github.com/duozhanggithub/Kubernetes/blob/master/Kuberadm.png)
