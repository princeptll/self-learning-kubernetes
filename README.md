# ☸️ Kubernetes Learning Topics

## 🧠 Core Concepts
- Monolithic vs Microservices Architecture
- Kubernetes Architecture
- Local Kubernetes Setup
  - kubectl
  - kubeadm
  - kind
- kubectl Basics & Commands
- Pods
- Namespaces (ns)
- Labels
- Selectors
- Annotations

---

## ⚙️ Workloads
- Deployments
- StatefulSets
- DaemonSets
- ReplicaSets
- Jobs
- CronJobs

---

## 🌐 Networking
- Cluster Networking
- Services
  - ClusterIP
  - NodePort
  - LoadBalancer
- Ingress
  - NGINX Ingress Controller
  - Gateway API
- Network Policies
  - Calico

---

## 💾 Storage & Configuration
- Persistent Volumes (PV)
- Persistent Volume Claims (PVC)
- Storage Classes
- ConfigMaps
- Secrets
- KEDA (Kubernetes Event-Driven Autoscaling)

---

## 📈 Scaling & Scheduling
- HPA (Horizontal Pod Autoscaler)
- VPA (Vertical Pod Autoscaler)
- Node Affinity
- Taints and Tolerations
- Resource Quotas
- Resource Limits and Requests
- Probes
  - Liveness
  - Readiness
  - Startup

---

## 🚀 GPU in Kubernetes
- What is a GPU in Kubernetes context
- Installing GPU support on Kubernetes nodes
- NVIDIA GPU driver installation
- Driver, CUDA, and container compatibility
- Validating GPU on host using `nvidia-smi`
- Kernel modules and reboot handling
- NVIDIA device plugin
- GPU resource allocation to pods
- Multi-Instance GPU (MIG) basics

<p align="center">
  🚀 <i>"Kubernetes: Where your app crashes in pods, not in production… hopefully."</i> 😄  
  <br/>
  <b>Keep calm, trust YAML, and let the cluster handle it.</b>
</p>
