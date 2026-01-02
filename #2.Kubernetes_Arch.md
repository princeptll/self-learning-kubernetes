<img width="729" height="391" alt="image" src="https://github.com/user-attachments/assets/a3f9478d-f81e-4a6f-bf3d-f0c541fc02bf" />

## 🧠 Kubernetes Architecture

Kubernetes follows a **master–worker architecture**, divided into:

- **Control Plane/ Master Node** – Brain of the cluster  
- **Worker Nodes** – Where applications actually run  

---

## 🎛️ Control Plane (Master Node)

The Control Plane is responsible for **managing, scheduling, and maintaining the cluster state**.

### Key Components

### 1. API Server
- Entry point for all Kubernetes operations
- All commands (`kubectl`, UI, CI/CD tools) communicate with the API Server
- Validates and processes requests

### 2. etcd
- Distributed key-value database
- Stores the entire cluster state (pods, nodes, configs, secrets)
- If etcd is lost, the cluster state is lost

### 3. Scheduler
- Decides which pod runs on which worker node
- Considers CPU, memory, GPU, affinity, taints, and tolerations

### 4. Controller Manager
- Ensures the desired state matches the actual state

**Examples:**
- If a pod crashes, a new pod is created
- If replicas are fewer than desired, it scales up automatically

---

## 🖥️ Worker Nodes

Worker nodes are where **containers and applications actually run**.

### Key Components

### 1. Kubelet
- Agent running on every worker node
- Communicates with the API Server
- Ensures pods are running as defined

### 2. Container Runtime
- Responsible for running containers

**Examples:**
- containerd
- CRI-O
- Docker (deprecated but still seen)

### 3. Kube-Proxy
- Handles networking and service communication
- Manages traffic routing between pods and services
