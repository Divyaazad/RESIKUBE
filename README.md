

# 🚀 RESIKUBE

### Kubernetes Resilience, Monitoring & MTTR Validation Platform

## 📌 Overview

**RESIKUBE** is a DevOps/SRE-oriented project that demonstrates **monitoring, observability, and resilience testing** of containerized applications running on **Kubernetes**.

The project focuses on **Mean Time To Recovery (MTTR)** by monitoring system behavior during **controlled failure scenarios** and validating Kubernetes’ self-healing capabilities using **Prometheus and Grafana**.

---

## 🎯 Problem Statement

In real-world cloud-native systems, failures such as:

* Pod crashes
* Service disruptions
* Resource spikes

are inevitable.

While monitoring systems can detect failures, **resilience is validated only when failures are intentionally tested**.

**RESIKUBE addresses this by combining monitoring with controlled chaos experiments** to observe recovery behavior and reliability metrics.

---

## 🧠 Key Concepts Demonstrated

* Kubernetes architecture & self-healing
* Observability using metrics
* Chaos engineering fundamentals
* SRE reliability metric (MTTR)
* Containerized application deployment
* Monitoring pipelines in cloud-native systems

---

## 🛠 Tech Stack

| Category         | Tools                        |
| ---------------- | ---------------------------- |
| Containerization | Docker                       |
| Orchestration    | Kubernetes                   |
| Monitoring       | Prometheus                   |
| Visualization    | Grafana                      |
| Chaos Testing    | Manual Pod Failure Injection |
| CI/CD            | GitHub & Docker Hub          |

---

## 🏗 Architecture (High Level)

1. Application deployed as Kubernetes pods
2. Prometheus scrapes metrics from services and pods
3. Grafana visualizes real-time metrics
4. Pod failures are manually injected
5. Kubernetes recreates failed pods automatically
6. Metrics validate downtime and recovery time

---

## 📊 Features

* Real-time Kubernetes monitoring
* Pod & service health visualization
* Controlled pod failure simulation
* Automatic recovery validation
* MTTR observation using metrics
* Dockerized application images

---

## 🧪 Chaos Engineering Validation

**Failure Scenario:** Pod deletion

```bash
kubectl delete pod <pod-name>
```

**Observed Behavior:**

* Pod termination detected
* Kubernetes scheduler recreates pod
* Prometheus captures downtime
* Grafana dashboards show recovery trend

This validates **fault tolerance and resilience** of the system.

---

## 📸 Screenshots

Screenshots demonstrating:

* Kubernetes pods & services
* Prometheus targets & metrics
* Grafana dashboards
* Chaos injection & recovery
* Docker Hub images

(Available in the `screenshots/` directory)

---

## ⚙️ How to Run

### 1️⃣ Clone Repository

```bash
git clone https://github.com/ishasingh2704/RESIKUBE.git
cd RESIKUBE
```

### 2️⃣ Deploy Kubernetes Resources

```bash
kubectl apply -f k8s/
```

### 3️⃣ Deploy Monitoring Stack

```bash
kubectl apply -f prometheus/
kubectl apply -f grafana/
```

### 4️⃣ Access Grafana

```bash
kubectl port-forward svc/grafana 3000:3000
```

---

## 📈 Metrics Observed

* Pod availability
* Service uptime
* CPU & memory usage
* Failure detection time
* Recovery time (MTTR)

---

## 🎓 Learning Outcomes

* Hands-on Kubernetes monitoring
* Understanding of system resilience
* Practical chaos engineering exposure
* SRE reliability metrics
* Production-style observability setup

---

## 💼 Why This Project Is Relevant 

This project demonstrates:

* Practical Kubernetes usage
* Monitoring & observability skills
* Failure handling in distributed systems
* SRE mindset and reliability analysis

It goes beyond basic deployment by **testing how systems behave under failure**.

---


## 🚀 Future Enhancements

* Alerting with Alertmanager
* Automated chaos testing tools
* Horizontal Pod Autoscaling
* Log aggregation using Loki
* Cloud deployment (AWS/GCP)

---

## 👩‍💻 Author

**Divya Azad**
3rd Year CSE Undergraduate | Jaypee Institute of Information Technology,Noida,Sector-62

---

