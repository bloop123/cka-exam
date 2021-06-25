# Course structure

## Session 1

* Introduction
* [Architecture](Architecture/README.MD)
* Installation
* Basics
* Kubects Commands
* Imperative vs Declarative

## Session 2: Services and Scheduling

* Kubectl commands
  * exec
  * logs
* Labels and Selectors
* [Node Selectors](Module-2/Scheduling/node-selector.yaml)
* [Taints and Tolerations](Module-2/Scheduling/taints-tolerations/toleration-pod.yaml)
  * 
  * key : value : effect
  * NoSchedule
  * PreferNoSchedule
  * NoExecute
* [Node Affinity](Module-2/Scheduling/nodeaffinity/nginx-nodeaffinity.yaml)
* Taints and Tolerations vs Node Affinity
  * taints allow only tolerant pods to run on nodes, but the pods can run on any other node as well
  * Affinity allows only scheduling of podes on desired nodes, but other nodes can also be scheduled.
  * Combination of Taints/Tolerations and NodeAffinity makes nodes and pods mutually exclusive
* [Resource Requirements and Limits](Module-2/Scheduling/resource-limit/cpu-request-limit.yaml)
* Controllers
  * [ReplicaSets](Module-3/Controllers/replicaset)
  * [Deployments](Module-3/Controllers/deployments/app1.yaml)
  * [DaemonSets](Module-3/Controllers/daemonset/daemonset.yaml)
* [Services](Module-2/Services/README.md)

## Session 3 : Application Lifecycle Management and Storage

* ALM
  * [Rolling Updates and Rollbacks](Module-3/Controllers/deployments/rollout_rollbacks.cmd)
  * [Environment Variables](Module-4/env_vars.md)
  * [ConfigMaps and Secrets](Module-4/cm-secret/README.md)
  * Multi Container PODs
* Storage
  * [Volumes](Module-4/storage/hoststorage.yaml)
  * [PV](Module-4/storage/pv.yaml)
  * [PVC](Module-4/storage/pvc.yaml)

## Session 4 : networking
[masterReadme](Networking)

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
* ![Service Networking](https://user-images.githubusercontent.com/17488415/123072311-0e1af380-d433-11eb-8176-15265cf68027.png)

* DNS in kubernetes
* CoreDNS in Kubernetes
* [Ingress](Ingress/ingress.md)

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

* Maintenance(ClusterMaintainance/Upgrade-Kubernetes.MD)
  * OS Upgrades
  * Kubernetes Software Versions
  * Cluster Upgrade Process
  * Backup and Restore Methods
* Troubleshooting
  * Application Failure.
  * Control Plane Failure
  * Worker Node Failure.
* Multiple Schedulers
* Configuring Kubernetes Scheduler

## Session 7 : Logging and Monitoring the Cluster

* Monitor Cluster Components
* Managing Application Logs.
* Kubernetes Prometheus monitoring

## Session 8 : Kubernetes on AWS (EKS) overview

## backup

* Init Container
* Static Pods
* Manual Scheduling
* StatefulSets
