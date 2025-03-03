Kubernetes Course
Course Overview
This course is designed to give participants a deep understanding of Kubernetes, covering everything from the basics to advanced topics like Affinity, StatefulSets, Helm, and Kubernetes security. The course includes hands-on YAML exercises from the repository to reinforce learning.

Syllabus
Foundation: Kubernetes Core Concepts
Goal: Learn Kubernetes fundamentals, its architecture, and how to deploy workloads

Introduction to Kubernetes

What is Kubernetes?
Pros and cons
Imperative vs. declarative
Kubernetes architecture overview (etcd, scheduler, API, etc.)
Key Kubernetes Components

Pods, Deployments, and ReplicaSets
Hands-on: Deploy a simple pod and a deployment
Services and Endpoints
Hands-on: Expose your deployment via a Service
YAML Basics for Kubernetes

YAML syntax and structure
Writing manifests for Pods, Deployments, and Services
Hands-on: Create a simple canary deployment
Namespaces and Resource Management

Why use namespaces?
Creating and managing namespaces
Assigning resource quotas and limits
Hands-on: Define namespaces and apply limits
Workload Orchestration & Scheduling
Goal: Learn how Kubernetes manages and schedules workloads for high availability and scalability

Deployments and Rolling Updates

Creating and managing deployments
Rolling updates and rollbacks
Hands-on: Perform an update and rollback with kubectl rollout undo
StatefulSets and Persistent Storage

Difference between Deployments and StatefulSets
Persistent Volumes (PVs) and Persistent Volume Claims (PVCs)
Storage Classes
Hands-on: Deploy MySQL and Redis with persistent storage
Advance Scheduling

Node Selector
Node and Pod Affinity rules
Required vs. preferred scheduling
Taint and toleration
Hands-on: Modify Affinity rules in Affinity/03/all-in-one.yaml
Kubernetes Networking & Traffic Management
Goal: Learn how Kubernetes handles network communication and traffic routing

Kubernetes Networking

Networking model and CNI plugins
Pod-to-Pod and Pod-to-Service communication
Network Policies for isolation
Hands-on: Secure a web app with MySQL using Network Policies
Services and Endpoints

ClusterIP, NodePort, LoadBalancer
Linking services to pods with endpoints
Hands-on: Deploy web-with-redis.yaml and test connectivity
Ingress Controllers and Resources

When to use Ingress
Setting up an Ingress controller
Routing traffic using Ingress rules
Hands-on: Deploy an Ingress resource to expose an app
Hands-on: Implement canary using Ingress annotations
Application Lifecycle & Helm
Managing Applications with Helm

Helm basics: Charts, Repositories, and Templating
Installing Helm and deploying applications
Advanced Helm: Custom Helm charts, values templating
Hands-on: Deploy a Helm chart and modify templates
Multi-Container Pods

Sidecar, Ambassador, and Adapter container patterns
Hands-on: Deploy a multi-container pod and test inter-container communication
Pod Lifecycle, Init Containers, and Probes

Pod phases and restarts
Init Containers for dependency management
Readiness, Liveness, and Startup Probes
Hands-on: Apply health probes to an existing application
Kubernetes CronJobs & Automation

Automating tasks with CronJobs
Hands-on: Deploy a CronJob for periodic tasks
Advanced Kubernetes & DevOps
Goal: Learn production-grade scaling, security, and Kubernetes CI/CD workflows

Auto-Scaling Applications

Horizontal vs. Vertical Pod Autoscaler (HPA, VPA)
Cluster Autoscaler concepts
Hands-on: Configure HPA for an application workload - https://github.com/elevy99927/k8s/tree/main/hpa
Kubernetes Permissions

Kubernetes RBAC (Role-Based Access Control)
Securing Pods (non-root users, capabilities, secrets management)
Hands-on: Implement RBAC and Network Policies
Advance Hands-on: SSO using pinniped and github
Troubleshooting and Debugging Kubernetes Applications

Common failure patterns and diagnostics approaches
Using kubectl describe, logs, and events effectively
Debugging Pod startup issues and container crashes
Hands-on: Troubleshoot various application failure scenarios
Kubernetes Observability

Setting up basic monitoring with Prometheus and Grafana
Centralized logging approaches
Resource usage tracking and optimization
Hands-on: Deploy monitoring stack and configure basic alerts
Package Management

Node.js: Covers dependency management using package.json
Python: Utilizes requirements.txt and virtual environments
Maven: Demonstrates Java project management with pom.xml
Gradle: Explores build automation with build.gradle
GitOps and CI/CD with Kubernetes

CI/CD basics
Introduction to GitOps principles
First pipeline using Jenkins
Using ArgoCD for declarative deployments
Hands-on: Set up a basic GitOps using ArgoCD
Final Project
Goal: Integrate all Kubernetes concepts with a CI/CD-driven deployment

Capstone Project: Deploy a Multi-Tier Kubernetes Application

Combine all concepts: Deployments, Kubernetes, Jenkins and GitOps
Section 5.1: Continuous Integration

Create a secure application
Use multistep Docker Image
Section 5.2: Continuous Delivery

Write a Jenkins pipeline
Create unit tests
Create security scan gate
Deploy your application (using ArgoCD)
Section 5.3: Continuous Deployment

Create Canary deployment using flagger, your new application should be installed, only in case of 95% success rate
Open in Google Cloud Shell
You can directly open this repository in Google Cloud Shell to start exploring the examples:

Open in Google Cloud Shell

https://shell.cloud.google.com/cloudshell/editor?cloudshell_git_repo=https://github.com/elevy99927/k8s
