# Course structure

## Session 1

* Introduction
* Architecture
![K8s Architecture](https://d33wubrfki0l68.cloudfront.net/2475489eaf20163ec0f54ddc1d92aa8d4c87c96b/e7c81/images/docs/components-of-kubernetes.svg)
![K8s Architecture](https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2018/07/1-7.png)
* Installation
* Basics
* Kubects Commands
* Imperative vs Declarative

## Session 2: Services and Scheduling

* Manual Scheduling
* Labels and Selectors
* [Taints and Tolerations](Module - 2/Scheduling/taints-tolerations/toleration-pod.yaml)
* Node Selectors
* Node Affinity
* Taints and Tolerations vs Node Affinity
* Resource Requirements and Limits
* Controllers
  * ReplicaSets
  * Deployments
  * StatefulSets
  * DaemonSets
* Services
* Multiple Schedulers
* Configuring Kubernetes Scheduler

## Session 3 : Application Lifecycle Management and Storage

* ALM
  * Rolling Updates and Rollbacks
  * Configure Environment Variables in Applications
  * Configuring ConfigMaps in Applications
  * Configure Secrets in Applications
  * Multi Container PODs
* Storage
  * Volumes
  * PV
  * PVC

## Session 4 : networking

* Basics
  * Switching Routing
  * DNS
  * Network Namespaces
  * Docker Networking - CNM
  * CNI
  * Cluster Networking
* Pod Networking
* CNI in kubernetes
* CNI weave
* IP Address Management - Weave
* Service Networking
* DNS in kubernetes
* CoreDNS in Kubernetes
* Ingress

## Session 5 : Security

* Kubernetes Security Primitives
* Authentication
  * TLS Introduction
  * TLS Basics
  * TLS in Kubernetes
  * TLS in Kubernetes - Certificate Creation
* View Certificate Details
* Certificates API
* KubeConfig
* API Groups
* Role Based Access Controls
* Cluster Roles and Role Bindings
* Image Security
* Security Contexts
* Network Policy

## Session 6 : Maintenance and Troubleshooting

* Maintenance
  * OS Upgrades
  * Kubernetes Software Versions
  * Cluster Upgrade Process
  * Backup and Restore Methods
* Troubleshooting
  * Application Failure.
  * Control Plane Failur
  * Worker Node Failure.

## Session 7 : Logging and Monitoring the Cluster

* Monitor Cluster Components
* Managing Application Logs.
* Kubernetes Prometheus monitoring

## Session 8 : Kubernetes on AWS (EKS) overview

## backup

* Init Container
* Static Pods
