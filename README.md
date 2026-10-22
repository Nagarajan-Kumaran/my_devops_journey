# 🚀 My DevOps Journey via Omarchy Arch

Welcome to my personal DevOps engineering roadmap repository! This project tracks my hands-on learning journey across core infrastructure engineering, automation, containerization, cloud, and infrastructure as code (IaC)—all built on top of **Omarchy Arch Linux**.

---

## 🛠️ The Foundation: Why Omarchy Arch?

[Omarchy Arch](https://omarchy.org) provides a lean, optimized, and transparent Linux playground. By building everything from the terminal up, I gain a deep understanding of standard OS primitives, kernel performance, and package compilation (`pacman` and `AUR`) before deploying automated systems.

---

## 🗺️ Roadmap & Curriculum

| Milestone | Core Topics & Tooling | Hands-On Target Labs |
| :--- | :--- | :--- |
| **01. Linux & Systems** | File system tree, Systemd, LVM, Processes (`top`/`htop`), User/Group ACLs, Package Management (`pacman`). | Implement automated backup crons, build custom log-rotation daemons. |
| **02. Bash Scripting** | Variables, Loops, Conditionals, Stream redirection (`stdout`/`stderr`), `sed`, `awk`, `grep`. | Write automated log analysis scripts and OS resource monitoring utilities. |
| **03. Networking** | OSI Model, TCP/UDP, DNS, IP routing, Subnetting, Tooling (`ip`, `ss`, `netstat`, `dig`, `iptables`/`nftables`). | Setup a secure firewall, reverse-engineer packet flows using `tcpdump`. |
| **04. Docker** | Image layers, Dockerfiles, Networking (Bridge/Host), Storage Volumes, Docker Compose. | Containerize a multi-tier microservice app (React + Node + PostgreSQL). |
| **05. Terraform** | HCL Syntax, Providers, State management, Variables, Modules, Outputs, Remote backends. | Spin up structured VPCs, EC2 clusters, and IAM configurations via IaC. |
| **06. Amazon Web Services** | Identity (IAM), Compute (EC2, Lambda), Networking (VPC, Subnets, IGW, NAT), Storage (S3, EBS). | Deploy a highly available, load-balanced application architecture. |
| **07. Kubernetes** | Pods, Deployments, Services, Ingress, ConfigMaps/Secrets, Persistent Volumes, Architecture (Control Plane). | Setup a local `minikube` or `k3s` environment with rolling zero-uptime updates. |

---

## 📂 Repository Structure

```text
.
├── 01-linux-systems/       # Core Arch configs, systemd unit files, LVM notes
├── 02-bash-scripting/      # System automation and parsing scripts
├── 03-networking/          # Nftables rules, traffic captures, DNS lab setups
├── 04-docker/              # Dockerfiles, Compose YAMLs, network setups
├── 05-terraform/           # Infrastucture-as-code configuration modules
├── 06-aws/                 # AWS architecture diagrams, CLI scripts, configuration
└── 07-kubernetes/          # YAML manifests for Deployments, Services, and Ingress
```

---

## ⚡ Quick Start & Commands for Arch

To help maintain this repository and environment from an Arch terminal, use the following core reference snippets:

### 1. Synchronise Repositories and Update System
```bash
sudo pacman -Syu
```

### 2. Install Required DevOps Tooling
```bash
sudo pacman -S docker docker-compose terraform aws-cli kubectl minikube openbsd-netcat bind
```

### 3. Manage the Docker Daemon
```bash
sudo systemctl enable --now docker
sudo usermod -aG docker $USER
newgrp docker
```

---

## 📈 Goals & Progress Tracking

* [ ] Mastery of Linux systems administration & low-level user namespaces.
* [ ] Full automation of environments via secure Bash tooling.
* [ ] 100% cloud resource provisioning strictly using Terraform pipelines.
* [ ] Production-grade cluster multi-tenancy management in Kubernetes.

---

*“Simplicity is the ultimate sophistication. Arch Linux teaches you how things work underneath the abstractions.”*




